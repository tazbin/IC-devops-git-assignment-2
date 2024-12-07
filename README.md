# IC DevOps Git Assignment 1

This repository contains the second assignment for the **Version Controll System** module.

### Git commands for this assignment:

Intialize empty git repo & add origin
```
git init

git remote add origin git@github.com:tazbin/IC-devops-git-assignment-2.git
```

Add `README.md` file, commit & push
```
touch README.md

git add .

git commit -m "Initial commit"

git push --set-upstream origin master
```

Create `feature-1` branch, add a file, commit & push
```
git branch feature-1

git checkout feature-1

touch file-1.txt

git status

git add .

git commit -m "Add file file-1.txt"

git push --set-upstream origin feature-1
```

Checkout to `master branch`
```
git checkout master
```

Create & checkout to `feature-2` branch, add file, commit & push
```
git checkout -b feature-2 

touch file-2.txt

git status

git add .

git commit -m "Add file file-2.txt"

git push --set-upstream origin feature-2
```

Rebase & merge `feature-1` branch to `master` branch

The branch is rebased using Github UI from pull request section selecting the **Rebase & merge** option

Update `feature-2` branch with `master`
```
git checkout feature-2

git pull --rebase origin master

git push -f
```

Rebase & merge `feature-2` branch to `master` branch

The branch is rebased using Github UI from pull request section selecting the **Rebase & merge** option

View linear history of `master` branch
```
git checkout master

git pull

git log --oneline
```

The Linear commit log is:
```
69401a8 (HEAD -> master, origin/master) Add file file-2.txt
c8d7875 Add file file-1.txt
98c55ac Intial commit
```