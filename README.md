practices of Git all related to bundle2

Exercise 2:


$ git add service.html

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git commit -m "add changes"
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md
        service

nothing added to commit but untracked files present (use "git add" to track)      

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git push origin main
To https://github.com/Manzikim/bundle1.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/Manzikim/bundle1.git'      
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.        

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git pull ft/service-redesign
fatal: 'ft/service-redesign' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git remotre -v
git: 'remotre' is not a git command. See 'git --help'.

The most similar command is
        restore

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git remote -v
origin  https://github.com/Manzikim/bundle1.git (fetch)
origin  https://github.com/Manzikim/bundle1.git (push)

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/service-redesign)
$ git pull
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 698 bytes | 5.00 KiB/s, done.
From https://github.com/Manzikim/bundle1
   befbd9d..8e6f98f  ft/service-redesign -> origin/ft/service-redesign
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:       

    git branch --set-upstream-to=origin/<branch> ft/service-redesign


NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/service-redesign)
$ git push origin
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/service-redesign)
$ git push origin ft/service-redesign
To https://github.com/Manzikim/bundle1.git
 ! [rejected]        ft/service-redesign -> ft/service-redesign (non-fast-forward)error: failed to push some refs to 'https://github.com/Manzikim/bundle1.git'      
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.        

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/service-redesign)
$ git push origin --delete<ft/service-redesign>
bash: syntax error near unexpected token `newline'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/service-redesign)
$ git checkout main
Switched to branch 'main'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git push origin --delete<ft/service-redesign>
bash: syntax error near unexpected token `newline'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git push origin --delete <ft/service-redesign>
bash: syntax error near unexpected token `newline'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$
 *  History restored 


NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git checkout ain
error: pathspec 'ain' did not match any file(s) known to git

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git checkout ain
error: pathspec 'ain' did not match any file(s) known to git

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git checkout main
Already on 'main'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git pull origin main
From https://github.com/Manzikim/bundle1
 * branch            main       -> FETCH_HEAD
error: The following untracked working tree files would be overwritten by merge:
        README.md
Please move or remove them before you merge.
Aborting
Updating befbd9d..00565dd

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git checkout -b ft/service-redesign
fatal: a branch named 'ft/service-redesign' already exists

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git checkout -b ft/service-redesign
fatal: a branch named 'ft/service-redesign' already exists

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git checkout -b ft/service-redesign
fatal: a branch named 'ft/service-redesign' already exists

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git pull origin main
From https://github.com/Manzikim/bundle1
 * branch            main       -> FETCH_HEAD
error: The following untracked working tree files would be overwritten by merge:
        README.md
Please move or remove them before you merge.
Aborting
Updating befbd9d..00565dd

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git checkout -b ft/service-redesign
fatal: a branch named 'ft/service-redesign' already exists


NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git checkout -b ft/servic-redesign
Switched to a new branch 'ft/servic-redesign'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/servic-redesign)
$ vim service.html

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/servic-redesign)
$ git add service.html

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/servic-redesign)
$ git commit -m "Add new changes to service.html"
[ft/servic-redesign 400e521] Add new changes to service.html
 1 file changed, 1 insertion(+), 1 deletion(-)

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/servic-redesign)
$ git push origin ft/servic-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 295 bytes | 49.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'ft/servic-redesign' on GitHub by visiting:
remote:      https://github.com/Manzikim/bundle1/pull/new/ft/servic-redesign
remote:
To https://github.com/Manzikim/bundle1.git
 * [new branch]      ft/servic-redesign -> ft/servic-redesign

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/servic-redesign)
$ git pull origin ft/servic-redesign
From https://github.com/Manzikim/bundle1
 * branch            ft/servic-redesign -> FETCH_HEAD
Already up to date.

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/servic-redesign)
$ git checkout main
Switched to branch 'main'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ cat service.html
unserting

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git add service.html

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git commit -m "Add diff"
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md
        service

nothing added to commit but untracked files present (use "git add" to track)

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ - Checkout your `main` branch and pull the latest changes
bash: main: command not found
bash: -: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ - Create a new branch named `ft/service-redesign`
bash: ft/service-redesign: No such file or directory
bash: -: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ - Add new changes to the `service.html` page
bash: service.html: command not found
bash: -: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ - commit and push them
bash: -: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ - create a new PR for your changes
bash: -: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ - go back to your `main` branch and add again new changes to your `service.html` page, you can add different changes but make sure to affect the same part(line of code) as you did in the other PR
bash: syntax error near unexpected token `('

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ - Commit and push those changes
bash: -: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ - Now go back to the github PR you had created for the `ft/service-redesign`branch, you 
will then see that you have conflicts with the `main` branch
bash: ft/service-redesign: No such file or directory
bash: main: command not found
bash: -: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ - In your project checkout the `ft/service-redesign`branch
bash: ft/service-redesign: No such file or directory
bash: -: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ - Compare the `ft/service-redesign`with the `main` branch using git diff and observe the changes
bash: ft/service-redesign: No such file or directory
bash: main: command not found
bash: -: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git push origin main
To https://github.com/Manzikim/bundle1.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/Manzikim/bundle1.git'
hint: Updates were rejected because the tip of your current branch is behind

hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ vim service.html

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git add service.html

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git commit -m "Add diff"
[main 80dc27b] Add diff
 1 file changed, 1 insertion(+), 1 deletion(-)

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git push origin main
To https://github.com/Manzikim/bundle1.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/Manzikim/bundle1.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git push origin main
To https://github.com/Manzikim/bundle1.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Manzikim/bundle1.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git push origin ft/servic-redesign
Everything up-to-date

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git push origin main
To https://github.com/Manzikim/bundle1.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Manzikim/bundle1.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git checkout ft/servic-redesign
Switched to branch 'ft/servic-redesign'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/servic-redesign)
$ git diff main

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/servic-redesign)
$ git add service.html

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/servic-redesign)
$ git commit -m "Resolving conflicts"
On branch ft/servic-redesign
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md
        service

nothing added to commit but untracked files present (use "git add" to track)

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/servic-redesign)
$ git push ft/servic-redesign
fatal: 'ft/servic-redesign' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/servic-redesign)
$ git push origin ft/servic-redesign
Everything up-to-date

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/servic-redesign)
$ git checkout ain
error: pathspec 'ain' did not match any file(s) known to git

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/servic-redesign)
$ git checkout main
Switched to branch 'main'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git merge ft/servic-redesign
Merge made by the 'ort' strategy.

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git commit -m "merging"
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md
        service

nothing added to commit but untracked files present (use "git add" to track)

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git push origin main
To https://github.com/Manzikim/bundle1.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Manzikim/bundle1.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git add service
warning: in the working copy of 'service', LF will be replaced by CRLF the next time Git touches it

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git add README.md
warning: in the working copy of 'README.md', LF will be replaced by CRLF the next time Git touches it

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git commit -m "Resolving conflicts"
[main 27ac603] Resolving conflicts
 2 files changed, 43 insertions(+)
 create mode 100644 README.md
 create mode 100644 service

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git push origin main
To https://github.com/Manzikim/bundle1.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Manzikim/bundle1.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git checkout ft/servic-redesign
Switched to branch 'ft/servic-redesign'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/servic-redesign)
$ ls
ban_dem  service.html

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/servic-redesign)
$ git commit -m "Resolving conflicts"
On branch ft/servic-redesign
nothing to commit, working tree clean

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/servic-redesign)
$ git push origin ft/servic-redesign
Everything up-to-date

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/servic-redesign)
$ git checkout main
Switched to branch 'main'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git commit -m "Resolving conflicts"
On branch main
nothing to commit, working tree clean

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git push origin main
To https://github.com/Manzikim/bundle1.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Manzikim/bundle1.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  bundle 3
  
  Exercise 1
  
  
  
  NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/team-page)
$ git checkout main
Switched to branch 'main'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/team-page)
$ git log
commit 3974b1968d36fe2acfae66f433760c290caff0c2 (HEAD -> ft/team-page)
Author: Manzikim <manzidakimo@gmail.com>
Date:   Sat May 20 01:30:37 2023 -0700

    changes added

commit 87aaf01670b09493f82f947bc1a497c0869dc6e0
Author: Manzikim <manzidakimo@gmail.com>
Date:   Sat May 20 01:22:55 2023 -0700

    changes added

commit 27ac603a379a3b4866557644c530b9e7a77ea43d (main, ft/contact-page)
Author: Manzikim <manzidakimo@gmail.com>
Date:   Sat May 20 01:06:23 2023 -0700

    Resolving conflicts

commit a28a99a0a905eef5b75a0fcf67471ab07a1d8d7e
Merge: 80dc27b 400e521
Author: Manzikim <manzidakimo@gmail.com>
Date:   Sat May 20 01:04:16 2023 -0700

    Merge branch 'ft/servic-redesign'

commit 80dc27b1d43fa42fd76c82c6f07da103c4d5259e
Author: Manzikim <manzidakimo@gmail.com>
Date:   Sat May 20 00:56:40 2023 -0700


NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/team-page)
$

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ git cherry-pick commit 3974b1968d36fe2acfae66f433760c290caff0c2 (HEAD -> ft/team-page)
bash: syntax error near unexpected token `('

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ Author: Manzikim <manzidakimo@gmail.com>
bash: syntax error near unexpected token `newline'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ Date:   Sat May 20 01:30:37 2023 -0700
bash: Date:: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$     changes added
bash: changes: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ commit 87aaf01670b09493f82f947bc1a497c0869dc6e0
bash: commit: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ Author: Manzikim <manzidakimo@gmail.com>
bash: syntax error near unexpected token `newline'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ Date:   Sat May 20 01:22:55 2023 -0700
bash: Date:: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$     changes added
bash: changes: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ commit 27ac603a379a3b4866557644c530b9e7a77ea43d (main, ft/contact-page)
bash: syntax error near unexpected token `('

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ Author: Manzikim <manzidakimo@gmail.com>
bash: syntax error near unexpected token `newline'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ Date:   Sat May 20 01:06:23 2023 -0700
bash: Date:: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$     Resolving conflicts
bash: Resolving: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ commit a28a99a0a905eef5b75a0fcf67471ab07a1d8d7e
bash: commit: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ Merge: 80dc27b 400e521
bash: Merge:: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ Author: Manzikim <manzidakimo@gmail.com>
bash: syntax error near unexpected token `newline'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ Date:   Sat May 20 01:04:16 2023 -0700
bash: Date:: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$     Merge branch 'ft/servic-redesign'
bash: Merge: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ commit 80dc27b1d43fa42fd76c82c6f07da103c4d5259e
bash: commit: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ Author: Manzikim <manzidakimo@gmail.com>
bash: syntax error near unexpected token `newline'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ Date:   Sat May 20 00:56:40 2023 -0700
bash: Date:: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ git cherry-pick <commit 3974b1968d36fe2acfae66f433760c290caff0c2 (HEAD -> ft/team-page)>
bash: syntax error near unexpected token `('

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ Author: Manzikim <manzidakimo@gmail.com>
bash: syntax error near unexpected token `newline'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ Date:   Sat May 20 01:30:37 2023 -0700
bash: Date:: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$     changes added
bash: changes: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ commit 87aaf01670b09493f82f947bc1a497c0869dc6e0
bash: commit: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ Author: Manzikim <manzidakimo@gmail.com>
bash: syntax error near unexpected token `newline'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ Date:   Sat May 20 01:22:55 2023 -0700
bash: Date:: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$     changes added
bash: changes: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ commit 27ac603a379a3b4866557644c530b9e7a77ea43d (main, ft/contact-page)
bash: syntax error near unexpected token `('

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ Author: Manzikim <manzidakimo@gmail.com>
bash: syntax error near unexpected token `newline'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ Date:   Sat May 20 01:06:23 2023 -0700
bash: Date:: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$     Resolving conflicts
bash: Resolving: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ commit a28a99a0a905eef5b75a0fcf67471ab07a1d8d7e
bash: commit: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ Merge: 80dc27b 400e521
bash: Merge:: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ Author: Manzikim <manzidakimo@gmail.com>
bash: syntax error near unexpected token `newline'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ Date:   Sat May 20 01:04:16 2023 -0700
bash: Date:: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$     Merge branch 'ft/servic-redesign'
bash: Merge: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ commit 80dc27b1d43fa42fd76c82c6f07da103c4d5259e
bash: commit: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ Author: Manzikim <manzidakimo@gmail.com>
bash: syntax error near unexpected token `newline'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ Date:   Sat May 20 00:56:40 2023 -0700
bash: Date:: command not found

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ git log
commit 27ac603a379a3b4866557644c530b9e7a77ea43d (HEAD -> ft/contact-page, main)       
Author: Manzikim <manzidakimo@gmail.com>
Date:   Sat May 20 01:06:23 2023 -0700

    Resolving conflicts

commit a28a99a0a905eef5b75a0fcf67471ab07a1d8d7e
Merge: 80dc27b 400e521
Author: Manzikim <manzidakimo@gmail.com>
Merge: 80dc27b 400e521
commit 27ac603a379a3b4866557644c530b9e7a77ea43d (HEAD -> ft/contact-page, main)       
Author: Manzikim <manzidakimo@gmail.com>
Date:   Sat May 20 01:06:23 2023 -0700

    Resolving conflicts

commit a28a99a0a905eef5b75a0fcf67471ab07a1d8d7e
Merge: 80dc27b 400e521
Author: Manzikim <manzidakimo@gmail.com>
Date:   Sat May 20 01:04:16 2023 -0700

    Merge branch 'ft/servic-redesign'

commit 80dc27b1d43fa42fd76c82c6f07da103c4d5259e
Author: Manzikim <manzidakimo@gmail.com>
Date:   Sat May 20 00:56:40 2023 -0700

    Add diff

commit 400e5219f5c78fad600d53a05460ec8b2e96bcaa (origin/ft/servic-redesign, ft/servic-redesign)
Author: Manzikim <manzidakimo@gmail.com>
Date:   Sat May 20 00:48:57 2023 -0700

    Add new changes to service.html

commit befbd9d5321866629a1c34fe987a172943a9ba53 (origin/ft/bundle-2, ft/service-redesign, ft/bundle-2)
Author: Manzikim <manzidakimo@gmail.com>

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ git cherry-pick 27ac603a379a3b4866557644c530b9e7a77ea43d (HEAD -> ft/contact-page, main)
bash: syntax error near unexpected token `('

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page)
$ git cherry-pick 27ac603a379a3b4866557644c530b9e7a77
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:

    git commit --allow-empty

Otherwise, please use 'git cherry-pick --skip'
On branch ft/contact-page
You are currently cherry-picking commit 27ac603.
  (all conflicts fixed: run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

nothing to commit, working tree clean

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page|CHERRY-PICKING)        
$ git cherry-pick 27ac603a379a3b4866557644c530b9e7a77ea43d
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:

    git commit --allow-empty

Otherwise, please use 'git cherry-pick --skip'
On branch ft/contact-page
You are currently cherry-picking commit 27ac603.
  (all conflicts fixed: run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

nothing to commit, working tree clean

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page|CHERRY-PICKING)        
$ git cherry-pick <27ac603a379a3b4866557644c530b9e7a77ea43d>
bash: syntax error near unexpected token `newline'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page|CHERRY-PICKING)        
$ git cherry-pick 27ac603a379a3b4866557644c530b9e7a77ea43d
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:

    git commit --allow-empty

Otherwise, please use 'git cherry-pick --skip'
On branch ft/contact-page
You are currently cherry-picking commit 27ac603.
  (all conflicts fixed: run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

nothing to commit, working tree clean

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page|CHERRY-PICKING)        
$ git add .

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page|CHERRY-PICKING)        
$ git commit -m "changes"
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:

    git commit --allow-empty

Otherwise, please use 'git cherry-pick --skip'
On branch ft/contact-page
You are currently cherry-picking commit 27ac603.
  (all conflicts fixed: run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

nothing to commit, working tree clean

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/contact-page|CHERRY-PICKING)        
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'
warning: cancelling a cherry picking in progress

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/faq-page)
$ touch faq.html

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/faq-page)
$ git add faq.html

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/faq-page)
$ git comit -m "changes"
git: 'comit' is not a git command. See 'git --help'.

The most similar command is
        commit

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/faq-page)
$ git commit -m "changes"
[ft/faq-page 40cac14] changes
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 faq.html

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/faq-page)
$ git push origin ft/faq-page
Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 4 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (8/8), 1.33 KiB | 340.00 KiB/s, done.
Total 8 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), done.
remote: 
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/Manzikim/bundle1/pull/new/ft/faq-page
remote:
To https://github.com/Manzikim/bundle1.git
 * [new branch]      ft/faq-page -> ft/faq-page

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/faq-page)
$ git log
commit 40cac14ab02b613353ec3ed018da6750d0b86b1d (HEAD -> ft/faq-page, origin/ft/faq-page)
Author: Manzikim <manzidakimo@gmail.com>
Date:   Sat May 20 01:48:14 2023 -0700

    changes

commit 27ac603a379a3b4866557644c530b9e7a77ea43d (main, ft/contact-page)
Author: Manzikim <manzidakimo@gmail.com>
Date:   Sat May 20 01:06:23 2023 -0700

    Resolving conflicts

commit a28a99a0a905eef5b75a0fcf67471ab07a1d8d7e
Merge: 80dc27b 400e521
Author: Manzikim <manzidakimo@gmail.com>
Date:   Sat May 20 01:04:16 2023 -0700

    Merge branch 'ft/servic-redesign'

commit 80dc27b1d43fa42fd76c82c6f07da103c4d5259e
Author: Manzikim <manzidakimo@gmail.com>
Date:   Sat May 20 00:56:40 2023 -0700

    Add diff

commit 400e5219f5c78fad600d53a05460ec8b2e96bcaa (origin/ft/servic-redesign, ft/servic-redesign)
Author: Manzikim <manzidakimo@gmail.com>

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/faq-page)
$ git revert 40cac14ab02b613353ec3ed018da6750d0b86b1d1
fatal: bad revision '40cac14ab02b613353ec3ed018da6750d0b86b1d1'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/faq-page)
$ git revert <40cac14ab02b613353ec3ed018da6750d0b86b1d1>
bash: syntax error near unexpected token `newline'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/faq-page)
$ git revert 40cac14ab02b613353ec3ed018da6750d0b86b1d1
fatal: bad revision '40cac14ab02b613353ec3ed018da6750d0b86b1d1'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/faq-page)
$ git revert '40cac14ab02b613353ec3ed018da6750d0b86b1d1'
fatal: bad revision '40cac14ab02b613353ec3ed018da6750d0b86b1d1'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/faq-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/team-page)
$ git push origin ft/team-page
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 499 bytes | 99.00 KiB/s, done.
Total 5 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/Manzikim/bundle1/pull/new/ft/team-page
remote:
To https://github.com/Manzikim/bundle1.git
 * [new branch]      ft/team-page -> ft/team-page

NIC@DESKTOP-J0Q1ROH MINGW64 ~/Documents/trial (ft/team-page)
$
