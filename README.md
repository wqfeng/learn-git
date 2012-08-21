learn-git
================
Some notes about git and github.

configuration
--------------------
* `git config --global user.name "wqfeng"`
* `git config --global user.email "qunfengw@gmail.com"`

* git aliases
    `git config --global alias.co checkout`
    `git config --global alias.br branch`
    `git config --global alias.ci commit`
    `git config --global alias.st status`
    `git config --global alias.unstage 'reset HEAD --'`
    `git config --global alias.last 'log -1 HEAD'`

work with remote repository(eg.github)
------------------------------------
* `git remote -v`
list the remote repo

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

* `git commit -a -m 'a comment'`
automatically stage every file tracked and commit.

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

* `git rm`
remove it from staging area and commit, also remove from working directory.

* `git rm -f`
remove for modified files

* `git rm --cached`
keep the files in working directory.

* `git mv`
rename

* `git log`
show the change history.

* `git commit --amend`
amend the last commit

* `git reset HEAD README.md`
unstage a staged file

* `git checkout -- README.md`
unmodify a modified file

* `git tag`
list available tags

* `git tag -a v0.1 -m 'the initial version'`
create an annotated tag

* `git show v0.1`
show the tag data

* `git push origin v0.1`
push tag to the remote server


Tips
---------------
* `git add .`
track all

* `git commit -a -m 'a comment'`
add and commit all modified files(*but not new ones*)

Reference
---------
[1] https://help.github.com/articles/set-up-git#platform-linux 

[2] http://git-scm.com/book

[3] http://git-tips.heroku.com/#1

[4] http://www.sbf5.com/~cduan/technical/git/

[5] http://rogerdudler.github.com/git-guide/

[6] http://www-cs-students.stanford.edu/~blynn/gitmagic/

[7] http://www.codeschool.com/courses/try-git

[8] http://sandofsky.com/blog/git-workflow.html
