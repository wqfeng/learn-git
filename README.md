learn-git
================
Some notes about git and github.

configuration
--------------------
* `git config --global user.name "wqfeng"`
* `git config --global user.email "qunfengw@gmail.com"`

work with remote repository(eg.github)
------------------------------------
* `git remote add origin https://github.com/wqfeng/learn-git.git`
creates a remote named "origin" pointing at your github repo

* `git push origin master`
sends your commits in the "master" branch to "origin"(your github repo)

* `git clone https://github.com/wqfeng/learn-git.git`
clone the remote repo into the locale machine

* `git remote add upstream https://github.com/wqfeng/learn-git.git`
assign the original repo to a remote called "upstream"

* `git fetch upstream`
pulls in changes not in your local repo, _without_ modifying your files.

* `git merge upstream/master`
merge any changes fetched into your woking files.

* `git pull upstream`
pull commits from "upstream", _automatically merges_ the commits without letting you review them first.

the most commonly used commands
--------------------------------
* `git status`
show the working tree status

* `git add README.md`
add file contents to the index

* `git init`
create a git repository

* `git commit -m 'a comment'`
record the changes to the repository.

* `git branch mybranch`
create a new branch called "mybranch"

* `git checkout mybranch`
make "mybranch" the active branch

* `git checkout -b mybranch`
create a new branch and makes it the active branch

* `git branch -d mybranch`
delete the "mybranch" branch

* `git diff`
show exactly what changed



Reference
---------
[1] https://help.github.com/articles/set-up-git#platform-linux 

[2] http://git-scm.com/book
