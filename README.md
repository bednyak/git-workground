# Git commands

- Push new local project to Git repository
```
git init
git status
git add .
git commit -m "First commit"
git remote add origin git@github.com:imtred/nodejs-sample.git
git push origin master
```

- Merge branches
```
git checkout master
git branch new-branch
git checkout new-branch
# ...develop some code...
git add .
git commit –m "Some commit message"
git checkout master
git merge new-branch
```

- Commit all changes
```
git status
git add .
git commit -m "First commit"
git push origin master
```

- Cancel 'git add' before commit
```
git reset HEAD~1
git status
```

- Commit specific folder/file
```
git status
git add ./<filename>
git commit -m "First commit"
git push origin master
```

- Create git ignore file
```
touch .gitignore
```

- Untrack file which was cached
```
git rm --cached <filename>
```

- Removed accidentally commited .idea in git
```
git rm -r --cached .idea
git commit -m 'Remove .idea folder'
git push origin master
```

- Check git log
```
git log
git log --oneline
git reflog --oneline
q
```

- Revert commit
```
git reflog --oneline
q
git revert 9a98ea0
git add .
git commit -m "Reverted commit 9a98ea0"
git push origin master
```

- Revert commit unpushed to origin
```
git reset --hard HEAD~
```

- Move project from one repository to another with all branches
```
git clone --mirror <url_of_old_repo>
cd <name_of_old_repo>
git remote add new-origin <url_of_new_repo>
git push new-origin --mirror
```

- Git push via username:password credentials
```
git push https://bednyak:github105@github.com/bednyak/lets-play-with-git.git master
```

- Create new branch
```git checkout -b [name_of_your_new_branch]
git push origin [name_of_your_new_branch]
```

- If old branch was broken - change it with new one (fixed)
```
git push -f origin <new branch>:<old branch>
```

