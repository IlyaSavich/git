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
Resets last commit
```
git config --global alias.undo '!git reset --hard HEAD~1'
```

### `git clean`
Remove all changes from working directory
```
git config --global alias.clean '!git reset --hard'
```

### `git fbranch <branch name>`
Re-create branch from current
```
git config --global alias.fbranch '!git branch -D $1 && git checkout -b'
```
