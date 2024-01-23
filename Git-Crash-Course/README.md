## Git Hidden folder

There is a hidden folder called `.git` which tells you that our project is a git repo. 

If we want to create a git repo in a new project we create the folder an initializar that repo using `git init`

```
mkdir /workspaces/tmp/new-project
cd /workspaces/tmp/new-project
git init
touch Readme.md
open Readme.md
git status
git add Readme.md
# makes changes to readme.md
git commit -a -m "add readme file"
```

## cloning

We can clone 3 ways , https , ssh github cli 

Since we are using github code spaces we will create temporary directory in our workspace 

```sh
mkdir /workspace/tmp
cd /workspace/tmp
```

## HTTPS

```sh
git clone https://github.com/SebastianZxs/Github-Examples.git
cd Github-Examples
```
## Commits


## Branches


## Remotes


## Stashing


## Merging

## Add

when we want to stage changes that will be included in the commit

```
git add Readme.md
git add .
```


## Reset

Reset allows you to move from stage are to unstaged area.
this is usefull when you want to revert all files not to be commited

```
git add .
git reset 
```
> git reset will revert a git add . 

## Git status

Git status shows you what files will or will not be comited

When we want to commit code we write git commit which will open up the commit edit message in the editor of choice. 

```sh
git commit
```

set the global editor
```
git config --global core.editor emacs
```

## Gitconfig file
the gitconfig file is what stores your global configurations for git such as email , name , editor and more .


Showing the contents of our  .gitconfig file
```
git config --list
```

when you first install git on a machine you are suppose to set up
your name and mail

```sh
git config --global user.name "john Doe"
git config --global user.email 
```

Make a commit and commit message whitout opening and editor
```sh
 git commit -m "add another exclamation"
```

## log 

git log will show recent git commands

## push 

when we want to push a repo to our remote origin
```sh
 git push
```