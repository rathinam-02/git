# Git course and commands
# git --version
# git config --global user.name 'rathinam-02'
# git config --global user.email 'rathinamaanikamm@gmail.com'
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
# PS E:\AWS-Devops-GT\Devops\Git\git-testing> git mv readme.md readme-commands.md
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