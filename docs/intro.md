```bash
echo "balidea" | git hash-object --stdin
git init
git branch -M main
echo "balidea git" | git hash-object --stdin -w
# persisted at .git/objects folder
git cat-file 1d005f33a185fc47c836ec7a1750654191c382c4 -t
git cat-file 1d005f33a185fc47c836ec7a1750654191c382c4 -p

git status
git add ./src/index.html
git status
git commit -m "first commit"
git log
git cat-file -p a880fd07cde3431ec411cbad6fd30a085fc56285
git cat-file -p 5530367abf45321d6172a92d47d2c2aa589dedb2

git branch
# persisted at .git/ref/heads folder
git branch ideas
cat .git/HEAD
```
