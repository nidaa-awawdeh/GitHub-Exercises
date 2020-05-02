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
**git stash pop/apply stash@{number}** to retrieve a specific stashed change.

<hr>

### Advanced Git Exercises.

#### Part I

1-What is the difference between git reset and git revert. When would you use one over the other? <br>
**When working with others, git revert is much safer as it undoes a commit, but it also generates a new commit that undoes all of the changes introduced in a previous commit and applies it to the current branch. Git reset simply undoes a commit which can be difficult to reconcile when working with others** <br>

2-What is the difference between git merge and git rebase. When would you use one over the other?<br>
**They are both essential when working on a team. Rebasing is helpful to maintain a cleaner commit history, but should never be done on a branch that has others working on it (since you can easily mess up their commit history).** <br>

3-What is the difference between git stash pop and git stash apply. When would you use one over the other?<br>
**git stash pop will return the latest value from the stash, but will remove it. Git stash apply will return the latest value but still maintain it in the stash.** <br>

4-What kinds of things can you do in interactive mode when rebasing?<br>
**You can amend commit messages, edit commits, squash or combine commit messages, remove commits and even execute shell commands**<br>

<hr>
