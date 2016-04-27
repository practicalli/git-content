# Magit Git Log


[![](images/emacs128x128icon.png)](http://emacsformacosx.com/)[![](images/git-logo-vertical.png)](http://4.bp.blogspot.com/-SAdRyX6xiDw/T2ENelQF52I/AAAAAAAAGKs/F1VH7LPiJEk/s1600/git-logo-vertical.png)In [part one](http://blog.jr0cket.co.uk/2012/12/driving-git-with-emacs-pure-magic-with.html) I showed how easy it is to version a project using Git from within Emacs, using the Magit package.  This time we look at the git log within Magit.

Working with the log gives you a lot more detail about your changes, helps you compare local and remote repo commits.  All of which helps you understand when you should push your code. 

## Git logs with Magit

On the command line you can use git log to see your change history, although it can be a bit fiddly to set up git to give you a pretty view of those logs.  In Magit you can just get on a explore the logs

Inside the Magit buffer, press **l** to show the log menu and then either **l** for the short for log or **L** for the long form of the log.

**l l** - short log  
**l L** - long log

[![](images/Emacs-git-log-menu.png)](http://4.bp.blogspot.com/-0QAfewaMsLw/UN-KyXzkaqI/AAAAAAAAI0I/SXTUvdWTyWY/s1600/Emacs-git-log-menu.png)

Figure 1:  **l** - the Magit log menu 

  
Selecting the short log details allows you to see more commits, but you only see the commit message and not the files that have changes.

In the following examples both the remote (github repository) and local repository are at the same commit - e447b51.  So you can easily tell if there are any local commits you have not pushed to Github.

[![](images/Emacs-git-log-short.png)](http://4.bp.blogspot.com/-ABVkJoYeq34/UN-VZ1ROTxI/AAAAAAAAI1Q/UNohWmIcPYQ/s1600/Emacs-git-log-short.png)

Figure 2:  **l**** l** - the Magit log short listing

  
Selecting the long log output, **l L**, you see more details of each commit, including the files changed, author and timestamp.

[![](images/Emacs-git-log-uptodate.png)](http://1.bp.blogspot.com/-0fxK4fEU8nQ/UN-KzcmzocI/AAAAAAAAI0M/jS9noFeIR5Q/s1600/Emacs-git-log-uptodate.png)

Figure 3:  **l**** L** - the Magit log short listing 

  
To see the changes within a commit, move the cursor over a commit number in the log and press **space**.  This brings up another buffer which you can scroll through.  You don't even need to switch to this new buffer as if you keep pressing **space** it will scroll through the text of the change.

[![](images/Emacs-git-log-commit-details.png)](http://2.bp.blogspot.com/-H5qNZ0NxDu4/UN-OaayK6mI/AAAAAAAAI0w/qoJt89QCdik/s1600/Emacs-git-log-commit-details.png)

Figure 4:  **l L space** - use the log to see the changes in a commit

  


## Comparing Commits (diff) with Magit 

In the following example, the local repository is ahead of the Github repository by one commit.  The magit log can be used to compare commits.

Move the cursor over the first commit and press **.** (full stop).  Then put the cursor over the second commit and press **=**.

[![](images/Emacs-git-log-short-commit-contents.png)](http://2.bp.blogspot.com/-3yRc4uinS9Q/UOAkTMBO-EI/AAAAAAAAI1w/-zguUhcRcME/s1600/Emacs-git-log-short-commit-contents.png)

Figure 5:  **l l . =**  - compare two commits using the Magit short log

  
To exit buffer that opened the diff, simply press **q** in the Magit buffer****.

## Summary of Magit log

I tend to just use the short form of the log and compare commits every now and again.  If I havent pushed a few commits up to Github for a while, its a handy way to check if I should push and what I am pushing.

Of course if I write good commit messages and commit often to my local repo, then its much easier to tell what I am pushing from the short log :)



