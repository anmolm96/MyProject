Git commands:

git log —-oneline // One commit per line
git log -p //Shows the diff+log
git add —-all //Adds all
git blame <file> -—date short //All changes in a file
git rm <file> //Removes file
git rm —-cached <file> //Stops tracking
git reset —-soft HEAD^ // last commit into Staging
git commit —-amend -m “new message” //Modifies last commit
git reset —-hard HEAD^ //Removes last commit
git revert HEAD //Cancel last commit
git remote add origin _______ //Adds online rep
git checkout —- ‘file’ //Removes from staging
git push -u <name> <branch> //pushes changes
git clone <url> //Clones online repo
git branch <name> //New branch called name
git checkout <branch> //Switch to other branch
git merge <branch> //Merges branch with the master
git branch -d <name> //Deletes branch
git checkout -b <name> //Shortcut to add+switch a branch
:wq //Merge and quit in Vi
git remote show origin //Shows remote branches and local branches
git push origin :<name> //Deletes remote branch
git push <heroku> <other branch>:master //Will merge/deploy other branch on heroku
git tag //Lists out all tags
git checkout <tag> //Check out code at commit
git tag -a <tag_name> -m “Message” //Adds new tag
git push —-tags
Local: git fetch + git rebase
Remote: git checkout <other> + git rebase master + git checkout master + git merge <other>
git rebase —-continue

//Add to new .gitconfig file
defaults write com.apple.finder AppleShowAllFiles YES
defaults write com.apple.finder AppleShowAllFiles NO
[alias]
  co = checkout
  ci = commit
  st = status
  br = branch
  hist = log --pretty=format:\"%h %ad | %s%d [%an]\" --graph --date=short
