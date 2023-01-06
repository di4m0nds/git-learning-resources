# Commands list
- `git config`
- `git config --list`
- `git config --list --show-origin`
- `git config --global user.name "Some Name"`
- `git config --global user.email "example@test.com.ar"`
- `git init`
- `git status`
- `git log <file>`
- `git log --all --decorate --oneline --graph`
- `git log --pretty=format:"%cn hizo un commit %h el dia %cd`
- `git log shortlog`
- `git log > log.txt` save logs ina file (txt in this case)
- `git log --after=“2018-1-2” --before=“today”` by date
- `git log --author=“Name Author”` by author
- `git show <file>`
- `git diff <commit number tag #1> <commit number tag #2>` compare differences
- `git status`
- `git add .` or `git add <relative-path-file>`
- `git commit -m "Some description"`
- `git commit -am "Some description"` Add and commit at the same time
- `git clone <url>`
- `git fetch`
- `git merge`
- `git pull` Simplifly "git fetch" & "git merge"
- `git push` Push your local commits
- `git rm <file>`
- `git rm --cached <file>` remove from staging area
- `git rm --force <file>` remove HDD
- `git reset --soft` back to staging
- `git reset --mixed` back to working directory
- `git reset --hard` delete everything
- `git reset HEAD` remove changes from staging 
- `git checkout <commit-id> <file>` OPTIONAL FILE
- `git checkout <branch-name>` back to lastest commit/changes
- `git branch <branch-name` create a new branch
- `git branch -l` list branches
- `git merge <branch-name>` make a commit with a merge
- `git remote add origin <url>` add remote
- `git remote -v` list remote origin
- `git push origin <branch-name>` push the a branch to origin (that is our remote branch)
- `git pull origin master --allow-unrealated-histories` merge remote history branch to local branch