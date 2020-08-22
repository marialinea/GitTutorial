# Git tutorial for n00bs

This is a easy tutorial for using various git commands in terminal mode, assuming you already have a GitHub user.

When you meet the following
```console
trolololol
```
you're supposed to write "trolololol" in your terminal window (and obviously press enter).

## Download git software

#### For MacOS:
1. Install homebrew (package manager for mac)
```console
  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

2.
```console
brew install git
```

#### For Linux and visual studio code (Windows)

1.
```console
sudo apt install git
```

## Configure git
1.
```console
git config --global user.name insertyournamehere
```
2.
```console
git config --global user.email insertyouremailhere
```
3.
```console
git config --global helper.store insertyourpasswordhere
```

Now you have successfully installed and configured git on your computer.

Below follows some useful git commands

## Branching

#### Making a new branch

```console
git checkout -b insertyourbranchnamehere
```

#### Switch between branches

```console
git checkout branchyouwanttoswitchto

```

#### Listing (local) branches
```console
git branch

```
Below is an example output:
```console
* barackobama
  master
```

The star indicates which branch you're currently on.

## Push your work to your branch

If you have made any changes to files in your git repo the following commands will push your work up to the server.

1. Stage changes
```console
git add --all
```
2. Commit and add a comment
```console
git commit -m "insert comment here"
```
3. Push that shit
```console
git push origin yourbranchname
```

## Merge your branch with the master branch
Before pushing to the master branch, make sure your files are pushed to your branch(!).

1. When you have switched branch to the master branch, pull from the master branch to make sure that you are up to date (meaning that there are no conflicts between the master branch up in the clouds and your local master branch).
```console
git pull origin master
```

2.
```console
git pull origin yourbranchname
```

3.
```console
git push origin master
```

4. Now gtfo of the master branch
```console
git checkout yourbranchname
```
