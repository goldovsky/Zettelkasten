# GIT

## ADD  
### Add everyfile except one
```bash
git add -- . :!path/to/file1
```

### Add everyfile and commit at the same time
```bash
git commit -am "" # TODO verify
```

## COMMIT  
### supprime un commit local
```bash
# soft: keep the current code | x is the number of commits 
git reset --soft HEAD~x
# hard: remove the corresponding code | x is the number of commits
git reset --hard HEAD~x
# then
git push origin -f # or git push origin HEAD --force
```

### Ajouter les dernieres modifs au dernier commit (sans un recreer un nouveau)
```bash
git add .
git commit --amend --no-edit
# pour aussi changer le message du dernier commit
git commit --amend -m "New commit message"
```

### Récupérer un commit en particulier
```bash
git cherry-pick <hash-in-question>
```

## ELSE  
### rebase 
```bash
git pull origin develop --rebase
# if necessary
git rebase --continue
# then
git push --force-with-lease
```

### Tag
```bash
git tag vx.x.x
git push --tags --no-verify
```
