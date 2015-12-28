# 2015 December 28  
 
## Trying Meld  
Decided to start using Meld for diff and merging.

Downloaded and installed version 3.14.2 from the official [website](http://meldmerge.org/).  

### Setup of GIT to use Meld   
Setting Meld as default merge-tool was done using the command-line interface:  
```
$ git config --global merge.tool "meld"  
$ git config --global mergetool.meld.path "C:\Program Files (x86)\Meld\Meld.exe"  
```

### Setup of SourceTree to use Meld  
These settings are based on [this](http://stackoverflow.com/a/21144229/686720) answer at stackoverflow.com.
- Start SourceTree  
- Goto Tools -> Options -> Diff tab  
- Choose Custom in external diff tool  
- Enter the path to Meld in Diff command i.e. C:\Program Files (x86)\Meld\meld.exe and enter $LOCAL $REMOTE in Arguments  
- Choose Custom in Merge Tool
- Enter the path to Meld in Diff Command i.e. C:\Program Files (x86)\Meld\meld.exe and $LOCAL $MERGED $REMOTE in Arguments  




