# GitHub-Exercises

### Git Basics Exercise:

1-Create a folder called learn_git_again.<br>
**mkdir learn_git_again**<br>
2-cd into the learn_git_again folder.<br>
**cd learn_git_again**<br> 
3-Create a file called third.txt.<br>
**touch third.txt**<br>
4-Initialize an empty git repository.<br>
**git init**<br>
4-Add third.txt to the staging area.<br>
**git add third.txt**<br>
5-Commit with the message "adding third.txt".<br>
**git commit -m "adding third.txt"**<br>
6-Check out your commit with git log.<br>
**git log**<br>
7-Create another file called fourth.txt.<br>
**touch fourth.txt**<br>
8-Add fourth.txt to the staging area.<br>
**git add fourth.txt**<br>
9-Commit with the message "adding fourth.txt"<br>
**git commit -m "adding fourth.txt"**<br>
10-Remove the third.txt file.<br>
**rm third.txt**<br>
11-Add this change to the staging area.<br>
**git add third.txt**<br>
12-Commit with the message "removing third.txt". <br>
**git commit -m "removing third.txt"**<br>
13-Check out your commits using git log. <br>
**git log**<br>
14-Change your global setting to core.pager=cat - you can read more about that here.<br>
**git config --global core.pager "cat"**<br>
15-Write the command to list all of the global configurations for git on your machine. You can type git config <br>--global to find out how to do this<br>

**- git config --global --list**<br>

### GitHub Basics Exercise

1-Create a local repository and add and commit some files
**mkdir learning && cd learning**<br>
**touch first.txt**<br>
**git init**<br>
**git add**<br>
**git commit -m "initial commit"**<br>
2-Create a remote repository and push your code from the local repo to the remote<br>
Head to GitHub and create a repository<br>
In your terminal type git remote add origin URL_OF_YOUR_REPO<br>
**git push -u origin master**<br>
3-Fork the repo https://github.com/rithmschool/git_practice - clone it and submit a pull request<br>
4-Create a new branch locally and push it to GitHub<br>
5-Submit a pull request with your new branch against the master branch on the git_practice repo.<br>

# Git Branching + Merging Exercise

### Part I

Answer the following questions:

- What does `git clean` do? **git clean removes files that have not been staged yet**
- What do the `-d and -f` flags for `git clean` do? **Remove untracked directories in addition to untracked files. If an untracked directory is managed by a different Git repository, it is not removed by default. Use -f option twice if you really want to remove such a directory.**
- What `git` command creates a branch? **git checkout -b**
- What is the difference between a fast-forward and recursive merge? **fast forwards can only happen if there have not been commits on the original branch while the new branch is being worked on**
- What `git` command changes to another branch? **git checkout**
- How do you remove **modified or deleted** files from the working directory? **git checkout**
- What `git` command deletes a branch? **git branch -D**
- What does the `git diff` command do? **shows you a difference between two different commits**
- How do you remove files from the staging area? **git reset HEAD name_of_file** or **git rm --cached name_of_file**
- How do merge conflicts happen? **When Git can not determine what file or folder to choose when merging since there have been different commits with changes to the same file**



 #### Stashing.
 
**git stash** - stash your commits (same as git stash save)<br>
**git stash list** - show the list of stashed changes<br>
**git stash apply** - move the latest stashed change back into the working directory, but keep it on the list<br>
**git stash pop** - move the latest stashed change back into the working directory and remove it from the list<br>
**git stash show** - show the latest stash<br>
**git stash show stash@{number}** - show a specific stashed chan<br>

<hr>

<hr>
