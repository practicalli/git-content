# Global Ignore

[![](images/git-logo-vertical1.png)](http://4.bp.blogspot.com/-SAdRyX6xiDw/T2ENelQF52I/AAAAAAAAGKs/F1VH7LPiJEk/s1600/git-logo-vertical.png)

Lots of developers are using git, especially when working on projects together.  However there is not one single developer tool that every one uses, so there is potential for a lot of unwanted files to end up in your project.

Rather than pollute the .gitignore file for the project with every development tool under the sun, its much more effective to add development tool specific files to your own global ignore file **~/.gitignore_global**.

## Creating my own global ignores 

In the ~/.gitconfig of my home directory I have a section called [core] where a global excludes file is defined

[core]  
    excludesfile = /Users/jstevenson/.gitignore_global

By adding file name patters to the .gitignore_global file for Emacs, I can add my own personal excludes without adding unnecessary stuff to each project I work on.  It also means its one less thing to remember when I am working with git projects.  
In the root of your home directory, simple create or update the file **.gitignore_global** with all the file names and patterns that relate to the tools you use.

## Ignore patterns 

To help you out, here are some ignore patterns for some of the most common developer tools.  There are lots of ignore patterns on the [Git Ignore github repository](https://github.com/github/gitignore/tree/master/Global)

[![](images/emacs128x128icon.png)](http://1.bp.blogspot.com/-PLeobToC6lc/TzFJCfBSLPI/AAAAAAAAEbE/zSx1cOgHzZE/s1600/emacs128x128icon.png)

### Emacs ignore patterns

*~  
\#*\#  
/.emacs.desktop  
/.emacs.desktop.lock  
.elc  
auto-save-list  
tramp  
.\#*

  
# Org-mode  
.org-id-locations  
*_archive

### Vi / Vim  


.*.s[a-w][a-z]

*.un~

Session.vim

.netrwhist

*~

  
  


### 

### IntelliJ ignore patterns

*.iml  
*.ipr  
*.iws  
.idea/  


  

### [![](images/netbeans-logo.jpg)](http://2.bp.blogspot.com/-EjfbbP6MpJo/URUV9U3X4ZI/AAAAAAAAJCY/RagOD9XWMZs/s1600/netbeans-logo.jpg)Netbeans ignore patters

nbproject/private/  
build/  
nbbuild/  
dist/  
nbdist/  
nbactions.xml  
nb-configuration.xml

[![](images/Eclipse_Icon_by_flosweb.png)](http://1.bp.blogspot.com/-RmrjIrvG7dE/URUVuk2P5QI/AAAAAAAAJCQ/RGcprIpBxjc/s1600/Eclipse_Icon_by_flosweb.png)

### Eclipse ignore patters

*.pydevproject   
.project   
.metadata   
bin/**   
tmp/**   
tmp/**/*   
*.tmp   
*.bak   
*.swp   
*~.nib   
local.properties   
.classpath   
.settings/   
.loadpath

  
# External tool builders   
.externalToolBuilders/

  
# Locally stored "Eclipse launch configurations"   
*.launch

  
# CDT-specific   
.cproject

  
# PDT-specific   
.buildpath
