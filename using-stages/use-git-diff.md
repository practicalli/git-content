# Use git diff

  The `git diff` command will show you which lines have changed, comparing the working copy with the commits in the local repository.  You can also just show the changes for a particular file.
  
```
git diff 

git diff filename
```  

You can see more specific changes

```
git diff --word-diff

git diff --word-diff filename
```  

This will show you the specific words on each line that have changed.  This is really good for picking up small changes, so its worth adding an alias for this to your git configuration, `~/.gitconfig`


## Comparing the Index 

  The `git diff` command also has an option for comparing the Index with the commits in the local repository.  This is a very useful tool to run before you create a new commit, to help check that you have added all the changes you want and none that you do not.
  
```
git diff --cached

git diff --cached filename 
```

