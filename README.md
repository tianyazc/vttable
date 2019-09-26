# Vlang Term Table

### How to install 
```vlang
```
### How to use
```vlang
module main
 
import table

fn maxs() {
    tdata := [
       ["name","sosurdace","2121","d"],
       ["Meterdasd","8s0","213",""],
       ["Peter","92dasa","322","qweeeee"],
       ["Peter","92dasa","322","qweeeee"]
   ]
    t := table.Table{
                    data:tdata,
                    position:"right",
                    // style: "simplicity"
                    }
    t.tables()
}

fn main() {
    maxs()
}
```