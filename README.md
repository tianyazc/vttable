# Vlang Term Table

### How to install 
#### use vpm
```golang
v install tianyazc.vttable
```
#### use vpkg
```golang
vpkg get github.com/tianyazc/vttable
```
### How to use
```golang
module main

import tianyazc.vttable 
fn main() {
    tdata := [
       ["name","source","sex","age"],
       ["Meter","80","man",""],
       ["Peter","92","man","21"],
       ["xiaoming","86","woman","18"]
   ]
    t := vttable.Table{
                    data:tdata,
                    position:"right",
                    // style: "simplicity"
                    }
    t.tables()
}
//out
$ v run table_t.v
+---------+-------+------+----+
|     name| source|   sex| age|
+---------+-------+------+----+
|    Meter|     80|   man|    |
+---------+-------+------+----+
|    Peter|     92|   man|  21|
+---------+-------+------+----+
| xiaoming|     86| woman|  18|
+---------+-------+------+----+
```
---
```golang
module main

import tianyazc.vttable
fn main() {
    tdata := [
       ["name","source","sex","age"],
       ["Meter","80","man",""],
       ["Peter","92","man","21"],
       ["xiaoming","86","woman","18"]
   ]
    t := vttable.Table{
                    data:tdata,
                    // position:"right",
                    style: "simplicity"
                    }
    t.tables()
}
//out
$ v run table_t.v
+---------+-------+------+----+
|name     |source |sex   |age |
+---------+-------+------+----+
|Meter    |80     |man   |    |
|Peter    |92     |man   |21  |
|xiaoming |86     |woman |18  |
+---------+-------+------+----+
```
