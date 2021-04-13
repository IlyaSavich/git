# Aliases

### `git refresh`
Make current branch up-to-date with remote
```
git config --global alias.refresh '!git fetch origin $(git branch --show-current) && git reset --hard origin/$(git branch --show-current)'
```

### `git pu`
Push current branch to remote repository
```
git config --global alias.pu '!git push origin $(git branch --show-current)'
```

### `git amend`
Amend all changes to previous commit
```
git config --global alias.amend '!git add . && git commit --amend'
```

### `git please`
Push with `force-with-lease` current branch
```
git config --global alias.please '!git push origin --force-with-lease $(git branch --show-current)'
```

### `git draft`
Commits with draft message
```
git config --global alias.draft '!git commit -am "$(git branch --show-current) draft"'
```

### `git undo`
Commits with draft message
```
git config --global alias.undo '!git reset --hard HEAD~1'
```
