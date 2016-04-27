# Interactive staging

  While you can use `git diff` to see what changes you have to stage, if there are many then using `git add` in an interactive mode will let you step through each change, one by one.


```
git add -p 

git add -p filename
```

## Hunks 

  Git groups changes into a fairly logical grouping called a **Hunk**.
  
  When you are interactively adding changes, git shows you the next hunk and asks if you wan to add or skip it.  Sometimes a hunk contains more changes line that you want to include, so you can split the hunk.
  
  
