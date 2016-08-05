# Introduction how to use git with R and RStudio

This tutorial in the context of the **Reproducible Research Workshop** provides you with the first steps on how to use git with R and RStudio.

The repository provides you with a step by step tutorial, that you are reading right now and is at the same time the repository you _play_ with to create your first git project in R.

## Motivation

R in combination with the distributed version control system _Git_ provides a convenient setup to make your research project reproducible. Git allows you to track and share your code and analysis. 

Some reasons to use version control are:

* It makes sharing of your projects _easy_ (once it's setup, you'll get there)
* It facilitates collaboration. People can contribute to your project and vis-versa. Also you can report errors (bugs) or suggest new additions (features).
* You can revert back to a previous version, if you find errors or accidently deleted something.
* You can _see_ what changes between different version of your code, analysis or written text!
* In R it makes sharing of your packages easy. And you can install development packages of others with two lines of code. `install.packages("devtools"); devtools::install_github("username/packagename")` (Development of R packages is more advanced in R, but is a well structured well to keep your projects tidy see: [R Packages by Hadley Wickahm](http://r-pkgs.had.co.nz/))

[Github](https://github.com/) is a user-friendly webservice that allows you to store your project repository remotely. Alternatives are [gitlab](https://about.gitlab.com/) and [bitbucket](https://bitbucket.org/).

RStudio integrates support for git and svn, hence we are going to use the widely used combination _R + Git + RStudio_.

## Installation and setup

To get started you need the following software installed on your computer:

**Git**  

* [Git](https://git-scm.com) ([Download Git](https://git-scm.com/downloads)). 
* Optional Git clients: [SourceTree](https://www.sourcetreeapp.com) or [GitHub Desktop](https://desktop.github.com) (use with care).

**R + RStudio**: If your are new to R you additionally have to install R and RStudio. Check if your current R + RStudio installation is up to date.

* [R](https://www.r-project.org) ([Download R](https://cloud.r-project.org))
* [Rstudio](https://www.rstudio.com) ([Download RStudio Desktop](https://www.rstudio.com/products/RStudio/#Desktop))

**GitHub**: On [Github](https://github.com/) create yourself a free GitHub account.    
If you haven't already followed the GitHub introduction to Git, follow the 15 min tutorial to get a quick interactive tutorial on Git. [TryGit Tutorial](https://try.github.io)

### Setup Git in RStudio

Tell RStudio where to find the Git installation

* Open RStudio and go to _Tools > Global Options..._ click on _Git/SVN_
* Check _Enable version control interface for RStudio projects_
* Set the path to the Git executable, that you just installed.

![**Figure:** RStudio: Global Options for Git/SVN](figures/RStudio-setup-git.png)

### Git setup

Configure Git and set your _user name_ and _email_ (The email address you use to register on GitHub). You can directly open the Git prompt from within RStudio. This needs to be set only once.
Go to _Tools > Shell_ to open the Git Shell to tell Git your username and GitHub email.

```
git config --global user.name 'Jane Doe'
git config --global user.email 'jane.doe@geo.uzh.ch'
```

![**Figure:** RStudio: Git Shell](figures/Rstudio-GitShell.png)


## Some other stuff
Commands to change repository "destination"

show current remote repository
> git remote -v show

remove the remote "origin" repository (origin is rather a convention than a command)
> git remote rm origin

add new repository 
> git remote add origin https://github.com/314a/rr-rstudio-git-mine.git
> git push -u origin master

now you can commit/push/pull your own project..!!

but:
http://stackoverflow.com/questions/10298291/cannot-push-to-github-keeps-saying-need-merge

use:
> git push -f origin master
> git push -u origin master

then push/pull should not be greyed out on rstudio again..

but 
https://landeco2point0.wordpress.com/2014/07/22/things-i-forget-pushpull-greyed-out-in-rstudio/

## Spell checking

https://support.rstudio.com/hc/en-us/articles/200551916-Spelling-Dictionaries
https://pages.github.com/

## Recommended literature

[1] L. Brundsdon, Chris; Comber, An Introduction to R for Spatial Analysis & Mapping. London: Sage Publications Ltd, 2015.    
[2] J. Paulson, “Version Control with Git and SVN,” 2016. [Online]. Available: https://support.rstudio.com/hc/en-us/articles/200532077-Version-Control-with-Git-and-SVN.   
[3] H. Wickham, “Git and GitHub,” R packages, 2015. [Online]. Available: http://r-pkgs.had.co.nz/git.html.    
[4] www.codeschool.com, “tryGit Tutorial.” [Online]. Available: https://try.github.io.
[5] K. Broman, “git/github guid.” [Online]. Available: http://kbroman.org/github_tutorial/.    