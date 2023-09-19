# Github Best Practices

## Setting up a Github Repo

1. Log into Github
2. in the top right corner there is a + icon click that and then "New Repository"
3. Put the repository name in and then click Create Repository (do not click Initialize this repository with a README)
4. You will then be taken to a page which gives you two options: 1. create a new repository on the command line or 2. push an existing repository from the command line

Choose Create new repository on the command line

5. Go to your folder where you have your code already in the command line

```
cd /location/of/the/code
```

5. run the commands from this section in your command line tool
   ex.

```
git init
git add .
git commit -m "first commit"
git remote add origin git@github.com:userName/IDM-project.git // This will be unique to your repo
git push -u origin main
```

6. Your Github repo will now be set up
7. Make changes to your code and push up the code as you are working

```
git add .
git commit -m "commit message"
git push origin main
```

## Participating in the Code Base (Advanced)

All push requests should be:

1. Restricted to a single feature
2. Be small and focused
3. Always be code reviewed before being merged

You should follow this flow when creating a branch, this way you can keep your branch cleaner:

(`branch-name` should be specific to the feature you are adding)

```
git remote update
git checkout --no-track -b feature/branch-name origin/master
```

...do a bunch of commits

```
git remote update
git rebase -i origin/main
```

- this will open an interactive rebase in vim
- all commits will say "pick" next to them
- keep the first one as "pick", change all the others to "s" which stands for squash
- after you are done with that

```
git push origin feature/branch-name
```
