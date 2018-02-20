# git-cheatsheet

## Create
Create a new local repository with the specified name
```
git init [project-name]
```
Download a project and its entire version history
```
git clone [url]
```

## Config
Define the author's name and email to be used for all commits by the current user
```
git config --global user.name [name]
git config --gloval user.email [email]
```
Create shortcut for a Git command. E.g. `alias.glog log --graph --oneline` will set `git glog` equivalent to `git log --graph --oneline`
```
git config --global alias.[alias-name] [git-command]
```
Set text editor used by commands for all users on the machine. `[editor]` arg should be the command that launches the desired editor (e.g., vim)
```
git config --system core.editor [editor]
```
Open the global configuration file in a text editor for manual editing
```
git config --global --edit
```

## Remote Repositories
Create a new connection to a remote repo. After adding a remote, you can use `[name]` as a shortcut for `[url]` in other commands.
```
git remote add [name] [url]
```
Fetches a specific `[branch]`, from the repo. Leave off `[branch]` to fetch all remote refs.
```
git fetch [remote] [branch]
```
Fetch the specified remote’s copy of current branch and immediately merge it into the local copy.
```
git pull [remote]
```
Push the branch to `[remote]`, along with necessary commits and objects. Creates named branch in the remote repo if it doesn’t exist.
```
git push [remote] [branch]
```

## Local Changes

## History
