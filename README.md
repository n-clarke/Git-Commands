# Git Commands
**Help**
```
git help
git help <command-name>
```
# Directory
**Display the current directory**
```
pwd
```
**Initiate Location Path**
```
cd ~/dir/
```
# Initialized Empty Git Repository
> Once your in the chosen file directory / or project directory enter either
```
git init <project-name>
or 
git init 
```
> To See hidden files: Command + Shift + .
# Create New Git Branch:
```
git branch <branch-name>
```
# Change Git Directory:
```
git checkout <name> 
e.g.
git checkout master
git checkout <branch-name>
```
## Configuration Commands
**Git Config (Global/User-level) Syntax**
```
git config --global setting value
```
**Configure User and Email**
```
git config --global user.name "Your Name"
git config --global user.email "you@someplace.com"
```
**Listing All Global Configuration Settings**
```
git config --global --list
```
**Seeing Git's User-based Config file**
```
cat ~/.gitconfig
```
# File Uploading and Changes
**Upload All Files (Everything)**
```
git add .
git commit -m “Comment”
git push origin Branch-Name
```
**Upload Cherry-Picking (Single File)**
```
git add <file-name>
git commit -m “Comment”
git push origin <branch-name>
```
**Upload Everything (The Force)**
```
git add .
git commit -m “Comment”
git push origin <branch-name> --force
 ```
**Unstage File**
> This command will "unstage" the specified file from Git's staging area (aka index).
```
git reset HEAD <file-name>
```
**Backout Working Directory Changes**
> This command backs out any changes made to the specified file and replace it with the version last committed in Git
```
git checkout -- <file-name>
```
**Remove Files**
```
git rm <FileName>
git commit -m “removing file”
```
**Moving Files**
```
git mv <FileName> <NewLocation/FolderName>
git commit -m “Moving File”
```
# Tracability
**Check the log of commits author and date**
```
git log
```
**Display the changes between commits, current commit and working tree**
```
git diff
```
# Remote Connection
**Init Remote Connection to a Git Repository**
```
git remote add origin url
git remote -v
git push -u origin <branch-name>
```
**Send Changes to Remote**
```
git push -u remote-name <branch-name>
git push remote-name <branch-name>
```
**Receive Changes from Remote**
```
git pull remote-name <branch-name>
```
# Merging
**Merge**
```
git checkout <receiving>
git pull
git merge <branch-name> where <branch-name>
```
# Rebasing
Rebases the current branch onto the specified branch
```
git checkout <current-branch-name>
git rebase <rebase-branch-name>
```
Changing Multiple Commit Messages (interactive rebasing tool)
```
git rebase -i <branch-name>
```
Squash several commits into a single commit
```
pick c1f3f6a changed variable name
squash 110237a updated README formatting
squash b1c1b0f added file
```
Modify the Most Recent Commit
```
git commit --amend
```
