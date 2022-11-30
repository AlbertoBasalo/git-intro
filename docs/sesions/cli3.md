```bash
git log --oneline
git switch main
git log --oneline
git merge feature/1-crear-index-html
git log --oneline
# meter un cambio en el index.html
git add -A
git commit -m "docs: placeholder para la lista"
git switch feature/1-crear-index-html
# meter un cambio en el index.html
git add -A
git commit -m "feat: cabecera de listado"
git switch main
git merge feature/1-crear-index-html
# Arreglar el conflicto eliminando el placeholder
git add -A
git commit -m "feat: eliminar placeholder"
git branch -d feature/1-crear-index-html

# stash
# nueva feature crear listado de actividades
git checkout -b feature/2-listado-actividades
# mientras lo creamos aparece fix de pone los meta en el head
git stash
git checkout main
git checkout -b fix/3-metas-head
# modificar el index html
git commit -a -m "fix: add metas to head"
git switch main
git merge fix/3-metas-head
git switch feature/2-listado-actividades
git merge main
git stash apply
# termino la modificación
git commit -a -m "feat: listado actividades"
# mezclo en main
git switch main
git merge feature/2-listado-actividades
git branch
git branch -d feature/2-listado-actividades
git branch -d fix/3-metas-head
git log --graph --oneline

# tags
git tag sprint-1
git tag
git log --graph --oneline
git checkout d41da13
git checkout sprint-1
git checkout main

npm init -y
# gitignore .vscode node_modules
git add .\.gitignore
git commit -m "chore: add gitignore exceptions"

npm i -D standard-version
git add
git commit -a -m "chore: install and configure standard-version"

git branch release/sprint-1
git switch release/sprint-1
npm run release
git switch main
git merge release/sprint-1
git log --oneline --graph
# mirar el fichero changelog

# alias
git log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --branches

code "C:\Users\[USER_NAME]\.gitconfig"

[alias]
  lg = log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --branches
  co = checkout
  ci = commit
  st = status
  ma = checkout main

```
