# Command Line Cheat Sheet (Mac)

_not an exhaustive list_

## Moving through the file system

### cd

`cd` is the primary command for navigating throughout your file system.

```js
# Go to the root of your file system
cd /

# Go to a place in the current folder you are in
cd ./

# Go UP a level in your file system
cd ../
```

### ls

`ls` allows you to view the files that are at your current place in your file system. This is useful if you need to check where you are or where you might want to go.

```js
# List all files/folders at your current location in the file system
ls
```

## Git commands

There are quite a few commands you can use with git as your version control but I will outline the simplest way to get information from your machine stored into your Github repository.

### Committing code

```js
# Add the changes to the git history
git add .

# Commit the changes you added with a message
git commit -m "Message describing your changes"

# Push your changes to the remote repository
git push origin main
```

### Creating a new repo

Once in a while (or 8 times in this course...) you will make a new repository to push code to. The easiest way to approach this is:

1. to go into Github and click New Repository on the top nav,
2. add a repository name and click `Create Repository`,

- Ensure the repo is public for DynWeb purposes

3. You will then be served with a "Quick Setup" page with the instructions to create a new repository on the command line.

It should look like this:

```
git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:zzz/zzz.git
git push origin main
```

The important line to note is the zzz/zzz.git which will be `username/repo-name`. So for example, for my exercise one repo that command will be this for me:

```
git remote add origin git@github.com:jayres/exercise-one.git
```
