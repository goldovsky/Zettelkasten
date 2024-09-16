# GIT

## supprime un commit local
- git reset --soft HEAD~1

## Add everyfile except one
git add -- . :!path/to/file1

## rebase 
```
git pull origin develop --rebase

# then
- force push --force-with-lease
```