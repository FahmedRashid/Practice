
Utilities & Tips --------------------------------------------//
git status

Stage & commit: --------------------------------------------//
git add .                       # stage all changes
git commit -m "commit message"

Create a branch and switch to it: --------------------------------------------//
git checkout -b branch-name   # Old style
git switch -c branch-name     # New style

Switch to an existing branch: --------------------------------------------//
git checkout branch-name
git switch branch-name

List branches:
git branch          # local branches
git branch -r       # remote branches
git branch -a       # all branches

Delete a branch:
git branch -d branch-name       # safe delete (won't delete unmerged)
git branch -D branch-name       # force delete

Pushing & Pulling --> Push a branch to remote: --------------------------------------------//
git push -u origin branch-name   # first push, sets upstream
git push                        # subsequent pushes

Pull changes from remote: --------------------------------------------//
git pull                        # pull current branch from remote
git pull origin branch-name      # pull a specific branch

Working with Multiple Remotes (personal/office)
git remote add personal https://github.com/FahmedRashid/Practice.git
git remote add office https://github.com/FahmedFN/office-repo.git

Push to a specific remote:
git push personal branch-name
git push office branch-name

Fetch/pull from a specific remote:
git fetch office
git pull office master

List remotes: 
git remote -v



Undo last commit (keep changes staged):
git reset --soft HEAD~1

View commit history:
git log --oneline --graph --all
