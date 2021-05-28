## help
```bash
git help
git help config
```
## alias 
```bash
git config --global alias.lg "log --oneline --decorate --all --graph"
git config --global alias.s "status -s"
```
## user config
```bash
git config --global user.name "user_name"
git config --global user.mail mail_address
git config --global user.name "user_name"
```
## commit
```bash
git commit -m "commit message"
```
add changes from trached files and commit
```bash
git commit -a -m "commit message"
```

## branch
create a new branch
```bash
git branch testing
```
remove a branch
```bash
git branch -d <branch_name>
```
## switch (checkout)
create & switch branch
```bash
git switch -C new-feature
```
switch branch
```bash
git switch feature 
```
### not recommended
create & switch branch
```bash
git checkout -b <branch_name>
```
switch branch
```bash
git checkout <branch>
```
## clone
```bash
git clone <repo_url> <folder_address>
```
## remote
```bash
git remote add <name> <url>
git remote rm <name>
git push -u <name> <branch>
```
## diff
show unstaged differences
```bash
git diff
git diff --staged
e.g. -copyright (c) 2012 ABC Company (in red color, removed text)
     +copyright (c) 2012 XYZ Company (in green color, added text)
```
## add
```bash
git add filename 
git add --all 
git add *.txt
git add docs
git add docs/*.txt
git add <list of files>
```
## restore (reset & checkout)
remove from the staging area (unstage)
```bash
git restore --staged secrets.sample.json
```
restore working tree files
```bash
git restore secrets.sample.json
```
### not recommended
reset current HEAD to the specified state
```bash
git checkout -- filename
```
unstage file
```bash
git reset HEAD -- path/to/file
```
unstage directory
```bash
git reset HEAD -- .
```
## rm
unstage and tell git to mark file/directory as deleted
```bash
git rm --cached -r .
```
## merge (empty)
