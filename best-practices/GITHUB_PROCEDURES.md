# Github Best Practices

## Participating in the Code Base

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
git rebase -i origin/master 
```

- this will open an interactive rebase in vim
- all commits will say "pick" next to them
- keep the first one as "pick", change all the others to "s" which stands for squash
- after you are done with that

```
git push origin feature/branch-name
```