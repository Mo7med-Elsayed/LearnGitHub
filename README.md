# LearnGitHub

Basic Git Commands:
1. git init                                   = creates a git repo
2. git add *                                  = add files to the stageing area (index)
3. git commit *                               = creates a version in the git repo
4. git status                                 = show files status
5. git log --oneline                          = show the commit history
6. git reflog                                 = show all commit history
7. git show <file>                            = show the content of the file
8. git diff <commitSha> <commitSha>           = display the difference between 2 commits
9. git tag -a v<VersionNum> -m "Tag Massage"  = exactly like the commit but tagged with version number

Undoing Things:
1. git restore --staged <file>                = restore the files from the stageing area
2. git restore <file>                         = discard changes in the modified files
3. git commit --amend                         = edit the last commit massage
4. git reset HEAD~1                           = will move the HEAD pointer to the prevous commit (Moving Backward) (index)
5. git reset --hard HEAD~1                    = will move the HEAD pointer to the prevous commit (Moving Backward) (WD)

Branching & Merge:
1. git branch <branchName>                    = to create a branch
2. git branch                                 = to show all branches
3. git switch <branchName>                    = to transeverse between branches
4. git merge <branchName>                     = to merge the branch to master while (HEAD => maser)

Working With Remote:
1. git clone <remote-repo> <local-repo>       = for cloning the repo
2. git remote -v                              = to show all remotes exist
3. git pull <remoteName>                      = to fetch and merge all changes
4. git push -u <remoteName> <localBranchName> = to push all changes to the remote repo branch
=> -u (--set-upstream) => for establish tracking relationship between the local branch and the remote branch (write it one time for each branch)
5. git branch -vv                             = to check on the tracking status between remote and local branches
