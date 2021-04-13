# Aliases

### refresh
Make current branch up-to-date with remote
```
git config --global alias.refresh '!git fetch origin $(git branch --show-current) && git reset --hard origin/$(git branch --show-current)'
```

### pu
Push current branch to remote repository
```
git config --global alias.pu '!git push origin $(git branch --show-current)'
```

### amend
Amend all changes to previous commit
```
git config --global alias.amend '!git add . && git commit --amend'
```

### please
Push with `force-with-lease` current branch
```
git config --global alias.please '!git push origin --force-with-lease $(git branch --show-current)'
```
