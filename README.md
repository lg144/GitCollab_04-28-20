# GitCollab_04-28-20
Git collaboration workshop

- `git clone <URL>`: downloads the repository from the web to our computer
  - Make sure you don't nest this command in another repository
  - Just like `git init` do this only once per repository

##Branches
- `git branch <branchname>`: create a new branch
- `git switch <branchname>`: move to a branch
  - `git checkout <branchname>`: old way of moving to branch

- `git switch -c <branchname>`: Create and move in one command
  - `git checkout -b <branchname>`

- `git stash`: temp saves current state as a commit so you can `checkout` or `switch`
  - `git stash apply` to apply the last stash from the stack

## Pull Requests (online merge)
  - `git push origin <branchname>`: pushes branch to remote
    - this is where you will create the pull request online
    - you merge the PR (and also the branch) by accepting and merging the PR
  - don't forget to clean up your Branches- `git fetch --prune`: cleans up the references in your `git log --oneline --all --graph --decorate`
  - `git branch -d <branchname>`: this will safely delete the branch
    - it till tell you to move to another branch first (make sure you're not on the branch you're trying to delete)
