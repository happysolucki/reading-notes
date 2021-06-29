# Git Stuff

### What is Git?

Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.

Basically it's a version control system. Git allows you to document your changes to files while keeping them in a repository. The way in which git works encourages collaboration. You can clone someone else's repo to your device locally. After maybe refactoring some of the code, adding a new feature, or updating the README you can track these changes, commit them, then push them to orginal creators repo through a pull request or to your own forked version of the repo.

### Essential Git Actions

- `git init` : starts a local git repository
- `git status` : shows current status of git repo; included info on current branch, tracked/untracked files, etc.
- `git add filename` `git add .` : tracks & stages a file; latter command tracks & stages all files in git repo
- `git commit -m "Some change"` : records your changes and prepares them to be pushed to a remote repository; the phrase in quotations is your commit message
- `git commit -a` : records all of your changes; basically does `git add .` for all tracked files in case those changes weren't staged already
- `git push origin main` : pushes/uploads commits to the set remote repository. "main" can often times be "master" instead
