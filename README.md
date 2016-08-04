# rr-rstudio-git
Reproducible research workshop RStudio and git demo repository



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


## Recommended literature

[1] L. Brundsdon, Chris; Comber, An Introduction to R for Spatial Analysis & Mapping. London: Sage Publications Ltd, 2015.
[2] J. Paulson, “Version Control with Git and SVN,” 2016. [Online]. Available: https://support.rstudio.com/hc/en-us/articles/200532077-Version-Control-with-Git-and-SVN.
[3] H. Wickham, “Git and GitHub,” R packages, 2015. [Online]. Available: http://r-pkgs.had.co.nz/git.html.
[4] www.codeschool.com, “tryGit Tutorial.” [Online]. Available: https://try.github.io.
[5] K. Broman, “git/github guid.” [Online]. Available: http://kbroman.org/github_tutorial/.