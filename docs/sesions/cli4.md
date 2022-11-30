```bash
# remotes
git remote add origin https://github.com/[USER_ORGANIZATION]/[REPO_NAME].git
git remote
git push -u origin main
git status

# agregar un fichero de licencia LICENSE en editor remoto
git status
git fetch
git diff origin/main
git diff ...origin/main
git merge
git diff origin/main
git status

# conflictos
# Hacer un cambio en le fichero de licencia en el servidor
# hacer un cambio local
git commit -a -m "chore: descripción package"
# intentar subir
git push
git status
git fetch
git diff ...origin/main
git merge
git status
git push
git status
git checkout -b release/sprint-2
npm run release
git checkout -
git tag
git push --tags

# gitflow

# recipes

```
