# Git course and commands
# git --version
# git config --global user.name 'rathinam-02'
# git config --global user.email 'rathinamaanikamm@gmail.com'
 create a new repository on the command line
# echo "# testing" >> README.md
# git init
# git add README.md
# git commit -m "first commit"
# git branch -M main
# git remote add origin https://github.com/rathinam-02/testing.git
# git push -u origin main
 push an existing repository from the command line
# git remote add origin https://github.com/rathinam-02/testing.git
# git branch -M main
# git push -u origin main
# git config --global init.defaultBranch main
# git init
# git status
# git add .
# git commit -m 'message'
#  git log
commit 2acab69a35f5426b227c8971d8e1b92f79a5a756 (HEAD -> main)
Author: rathinam-02 <rathinamaanikamm@gmail.com>
Date:   Tue Jul 28 19:08:03 2026 +0530

    readme file

commit bdf9daedfe783abefe68d77c0800261bc7c77324
Author: rathinam-02 <rathinamaanikamm@gmail.com>
Date:   Tue Jul 28 19:05:52 2026 +0530

    Initial commit

 #   PS E:\AWS-Devops-GT\Devops\Git\git-testing> git log --oneline
4c6f918 (HEAD -> Main-Branch) readme-conflict-merge
6a63900 (orgin/git-main, git-main, git-command) done merge
63fba78 Merge branch 'git-command' into git-main merge complete
b3829bd merge instruction
17bf68d merge
6926a04 (orgin/git-command) edited
6d8b0df Merge pull request #5 from rathinam-02/git-command
22f847d new-commit-new-branch
28acfc0 new-branch commit
ddd2612 (branch-test) revert done
5ce2b83 repo create cmd added
a85f4ce all changed saved
# PS E:\AWS-Devops-GT\Devops\Git\git-testing> git reflog
2acab69 (HEAD -> main) HEAD@{0}: commit: readme file
bdf9dae HEAD@{1}: commit (initial): Initial commit
# PS E:\AWS-Devops-GT\Devops\Git\git-testing> git add remote orgin 'https://github.com/rathinam-02/git'
## PS E:\AWS-Devops-GT\Devops\Git\git-testing> git mv readme.md readme-commands.md
# PS E:\AWS-Devops-GT\Devops\Git\git-testing> git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        renamed:    readme.md -> readme-commands.md

# PS E:\AWS-Devops-GT\Devops\Git\git-testing> git commint -m 'renamed file readme-commands.md'
git: 'commint' is not a git command. See 'git --help'.

The most similar command is
        commit
# PS E:\AWS-Devops-GT\Devops\Git\git-testing> git commit -m 'renamed file readme-commands.md' 
[main 7187769] renamed file readme-commands.md
 1 file changed, 0 insertions(+), 0 deletions(-)
 rename readme.md => readme-commands.md (100%)
# PS E:\AWS-Devops-GT\Devops\Git\git-testing> git pull orgin main   
remote: Enumerating objects: 66, done.
remote: Counting objects: 100% (66/66), done.
remote: Compressing objects: 100% (41/41), done.
remote: Total 66 (delta 29), reused 53 (delta 20), pack-reused 0 (from 0)
Unpacking objects: 100% (66/66), 8.55 KiB | 2.00 KiB/s, done.
From https://github.com/rathinam-02/git
 * branch            main       -> FETCH_HEAD
 * [new branch]      main       -> orgin/main
fatal: refusing to merge unrelated histories
# PS E:\AWS-Devops-GT\Devops\Git\git-testing> git fetch 
remote: Enumerating objects: 26, done.
remote: Counting objects: 100% (26/26), done.
remote: Compressing objects: 100% (15/15), done.
remote: Total 20 (delta 9), reused 15 (delta 4), pack-reused 0 (from 0)
Unpacking objects: 100% (20/20), 1.85 KiB | 2.00 KiB/s, done.
From https://github.com/rathinam-02/git
 * [new branch]      bug         -> orgin/bug
 * [new branch]      feature     -> orgin/feature
 * [new branch]      feature2    -> orgin/feature2
 * [new branch]      new-feature -> orgin/new-feature
# PS E:\AWS-Devops-GT\Devops\Git\git-testing> git pull orgin main
From https://github.com/rathinam-02/git
 * branch            main       -> FETCH_HEAD
fatal: refusing to merge unrelated histories

# PS E:\AWS-Devops-GT\Devops\Git\git-testing> git branch
  Main-Branch
  branch-test
  git-main
* main
# PS E:\AWS-Devops-GT\Devops\Git\git-testing> git switch git-main
Switched to branch 'git-main'
Your branch is up to date with 'orgin/git-main'.
# PS E:\AWS-Devops-GT\Devops\Git\git-testing> git switch -c git-command
Switched to a new branch 'git-command'

TO merge we need to switch to the branch in which we need to merge 
#PS E:\AWS-Devops-GT\Devops\Git\git-testing> git branch
* Main-Branch
  branch-test
  git-command
  git-main
  main

# PS E:\AWS-Devops-GT\Devops\Git\git-testing> git switch git-main
Switched to branch 'git-main'

Now 
# git merge git-command
and when it shows the conflict open the file in VI and edit the code in the file and save it and 
then git add .
and git commit -m 'message' 
to resolve the merge conflict

# git pull  (merge- fast-forward-)
# PS E:\AWS-Devops-GT\Devops\Git\git-testing> git branch
  Main-Branch
  branch-test
  git-command
* git-main
  main
# PS E:\AWS-Devops-GT\Devops\Git\git-testing> git pull orgin git-main
remote: Enumerating objects: 17, done.
remote: Counting objects: 100% (17/17), done.
remote: Compressing objects: 100% (12/12), done.
remote: Total 12 (delta 7), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (12/12), 4.07 KiB | 4.00 KiB/s, done.
From https://github.com/rathinam-02/git
 * branch            git-main   -> FETCH_HEAD
   6a63900..0d68aa0  git-main   -> orgin/git-main
Updating 6a63900..0d68aa0
Fast-forward
 index.html         |  4 ++--
 readmd.md          | 11 ++++++++---
 readme-commands.md |  6 ++++--
 readme.md          | 11 +++++++++--
 4 files changed, 23 insertions(+), 9 deletions(-)



# PS E:\AWS-Devops-GT\Devops\Git\git-testing> git stash
Saved working directory and index state WIP on git-command: 6926a04 edited

# PS E:\AWS-Devops-GT\Devops\Git\git-testing> git stash list
stash@{0}: WIP on git-command: 6926a04 edited
# PS E:\AWS-Devops-GT\Devops\Git\git-testing> git stash pop
On branch git-command
Your branch is up to date with 'orgin/git-command'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   readme-commands.md

no changes added to commit (use "git add" and/or "git commit -a")
Dropped refs/stash@{0} (f31aa071add6997b9f6f8bd1a53428ee18297eaf)