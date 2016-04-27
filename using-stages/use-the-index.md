# Use the Index

  It can be tempting to just commit all using `git commit -am "Commit all the things"`, however there can be lots of changes that you dont want to include.

  When you are busy it is easy to forget changes you made that are not relevant.  A good approach is to consider a stage every time you save the file you are working on.

```
git add filenames
```

You can add the same filename over and over again as you create more changes in your editor.

  
## Adding changes to the Index are easy to undo 

  Its very easy to remove a change from staging

```
git reset HEAD filenames
```

As all this command does is unstage the file (or files) from the index, then there is very little impact.  Your editor most likely has all this information in its history.

<hr />
