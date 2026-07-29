# Git course and commands
# git --version
# git config --global user.name 'rathinam-02'
# git config --global user.email 'rathinamaanikamm@gmail.com'
# create a new repository on the command line
echo "# testing" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/rathinam-02/testing.git
git push -u origin main
# push an existing repository from the command line
git remote add origin https://github.com/rathinam-02/testing.git
git branch -M main
git push -u origin main
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
# create a new repository on the command line
# echo "# testing" >> README.md
# git init
# git add README.md
# git commit -m "first commit"
# git branch -M main
# git remote add origin https://github.com/rathinam-02/testing.git
# git push -u origin main
# push an existing repository from the command line
# git remote add origin https://github.com/rathinam-02/testing.git
# git branch -M main
# git push -u origin main
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