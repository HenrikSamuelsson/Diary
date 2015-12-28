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
- Go to Tools -> Options
- Choose the General tab and make sure that the option Allow SourceTree to modify your global Git and Mercurial config files is checked.  
- Choose the Diff tab  
- Choose Custom in external diff tool  
- Enter the path to Meld in Diff command i.e. C:\Program Files (x86)\Meld\meld.exe and enter $LOCAL $REMOTE in Arguments  
- Choose Custom in Merge Tool
- Enter the path to Meld in Diff Command i.e. C:\Program Files (x86)\Meld\meld.exe and $LOCAL $MERGED $REMOTE in Arguments  

### Launching Meld diff view from within SourceTree  
Right click on the file that have changed in SouceTree. Choose External Diff in the pop-up menu. This will launch Meld and the differences in the file compared to the previous version can be viewed.  
