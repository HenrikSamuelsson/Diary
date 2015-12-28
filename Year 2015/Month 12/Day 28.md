## Trying Meld
Decided to start using Meld for diff and merging.

Downloaded and installed version 3.14.2 from the official [website](http://meldmerge.org/).  

** Setup of GIT **  
Setting Meld as default merge-tool was done using the command-line interface:  
```
$ git config --global merge.tool "meld"
$ git config --global mergetool.meld.path "C:\Program Files (x86)\Meld\Meld.exe"
``` 