# Git Commands
**Help**
```
git help
git help <command-name>
```
## Configuration Commands
**What's the current directory (present working directory)?**
```
pwd
```
**Git Config (Global/User-level) Syntax**
```
git config --global setting value
```
**Configure User and Email**
General Syntax:
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
# Initiate Location Path:
```
cd ~/dir/
```
# Current Location:
```
pwd
```
# Initialized empty Git repository
After you’re in the chosen file directory / or project directory enter either
```
git init <project-name>
or 
git init 
```
See hidden files: Command + Shift + .

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
# Upload All Files (Everything)
```
git add .
git commit -m “Comment”
git push origin Branch-Name
```
# Upload Cherry-Picking (Single File)
```
git add <file-name>
git commit -m “Comment”
git push origin <branch-name>
```

# Upload Everything (The Force)
```
git add .
git commit -m “Comment”
git push origin <branch-name> --force
 ```
# Unstage File
```
git reset HEAD <file-name>
```
Following the above command will "unstage" the specified file from Git's staging area (aka index).
# Backout Working Directory Changes
```
git checkout -- <file-name>
```
Following the above command will back out any changes made to the specified file and replace it with the version last committed in Git
# Check the log of commits author and date
```
git log
```
# Remove Files
```
git rm <FileName>
git commit -m “removing file”
```
# Moving Files
```
git mv <FileName> <NewLocation/FolderName>
git commit -m “Moving File”
```
# Init Connection to a GIT repo
```
git remote add origin url
git remote -v
git push -u origin <branch-name>
```
# Send Changes to Remote
```
git push -u remote-name <branch-name>
git push remote-name <branch-name>
```
# Receive Changes from Remote
```
git pull remote-name <branch-name>
```
# Merge
```
git checkout <receiving>
git pull
git merge <branch-name> where <branch-name>
```
