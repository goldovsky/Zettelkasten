# GIT

## supprime un commit local
```bash
git reset --soft HEAD~1
```

## Add everyfile except one
```bash
git add -- . :!path/to/file1
```

## rebase 
```bash
git pull origin develop --rebase
# then
git push --force-with-lease
```

## Tag

```bash
git tag vx.x.x
git push --tags --no-verify
```
