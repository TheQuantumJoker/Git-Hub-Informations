# Git & GitHub Information and Testing Repo

## TO DO LIST
### From praqma-training
This are exercises taken from [here](https://github.com/praqma-training/git-katas.git).
#### Basics
- [x] configure-git
- [x] basic-commits
- [x] basic-cleaning
- [x] basic-branching
- [x] basic-staging
- [x] basic-revert
- [x] basic-stashing
#### Advanced
- [ ] ignore
- [ ] amend
- [ ] ff-merge
- [ ] merge-mergesort
- [ ] merge-conflict
- [ ] rebase-branch
- [ ] reset
- [ ] detached-head
### From GitHub Skills
There are standard exercises from [Github Tutorial](https://skills.github.com/).
#### First day on GitHub
- [x] Introduction to GitHub
- [x] Communicate using Markdown
- [x] GitHub Pages
#### First week on GitHub
- [ ] Review pull requests
- [ ] Resolve merge conflicts
- [ ] Release-based workflow
- [ ] Connect the dots
- [ ] Code with Codespaces
- [ ] Code with Copilot
#### Automate workflows with GitHub Actions
- [ ] Hello GitHub Actions
- [ ] Test with Actions
- [ ] Publish packages
- [ ] Deploy to Azure
- [ ] Write JavaScript actions
- [ ] Reusable workflows
#### Code security and analysis
- [ ] Secure your repository supply chain
- [ ] Secure code game
- [ ] Introduction to code QL
### What's next?
After all this you can set new goals which now doesn't really makes much sense to define.


## Git(Hub) commands list

### Local command
- *git status* show active branch, commits, if there's something to commit.
- *git add filename* to add the file(s) named filename for the next commit.
- *git commit -m "My commit message"* To commit what is added.
- *git log --oneline -n 5* To see the last -n commit, in --oneline. With --graph shows the relations, with --all show all the branches (without it shows only the current one).
- *git clean* Delete all temporary files, with the exception of the ones in the staging area. With the option -n it doesn't delete anything but tells you what would be deleted.
- *git branch* see available branches, the green one is the one you are logged in.
- *git branch newbranch* create a branch named newbranch (from the current one?).
- *git switch branchName* switch to the branch named branchName.
- *git diff branch1 branch2* show the differences between branch1 and branch2.
- *git diff* tells you differences between current branch version and it's last commit. With the option --staged tells you the differences between last commit and staging area.
- *git restore myfile* change myfile in the folder as its previous commit. If you add --staged changes myfile in the staging area as its previous commit.
- *git revert commitHash* Delete all the upgrade made with the commit that had hash commitHash.
- *git show commitHash* Show all the modification made by the commit with hash commitHash.
- *git stash* Recover last commited version, and hide in a "stash area" all the modified file. The stashed areas can be listed with *git stash list*, and all the files shown with *git stash show*.
- *git reset* is the unsafe version of stash: it recovers the last commit permanently deleting files, so basically never to use.