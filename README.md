# git-test

This git test worked

I will store everything that has been output here real quick


Last login: Tue Mar 18 13:08:31 on ttys002
❯ cd git-test
❯ touch testfile1.txt
❯ open -e testfile1.txt
❯ code testfile1.txt
❯ open -e testfile1.txt
❯ code testfile1.txt
❯ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	testfile.txt
	testfile1.txt

nothing added to commit but untracked files present (use "git add" to track)
❯ git add testfile1.txt
❯ git add testfile1.txt testfile.txt
❯ git commit -m "these are test files
dquote>                                   
dquote> "
[main (root-commit) 9607450] these are test files
 2 files changed, 8 insertions(+)
 create mode 100644 testfile.txt
 create mode 100644 testfile1.txt
❯ git push origin main
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
❯ git status
On branch main
nothing to commit, working tree clean
❯ git-test
zsh: command not found: git-test
❯ git remote add origin git@github.com:Carlarlgfy/git-test.git
❯ git remote -v
origin	git@github.com:Carlarlgfy/git-test.git (fetch)
origin	git@github.com:Carlarlgfy/git-test.git (push)
❯ git push -u origin main
Enter passphrase for key '/Users/carlmarquis-olson/.ssh/id_ed25519': 
To github.com:Carlarlgfy/git-test.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'github.com:Carlarlgfy/git-test.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
❯ git pull origin main --rebase
Enter passphrase for key '/Users/carlmarquis-olson/.ssh/id_ed25519': 
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 864 bytes | 432.00 KiB/s, done.
From github.com:Carlarlgfy/git-test
 * branch            main       -> FETCH_HEAD
 * [new branch]      main       -> origin/main
Successfully rebased and updated refs/heads/main.
❯ git push origin main
Enter passphrase for key '/Users/carlmarquis-olson/.ssh/id_ed25519': 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 479 bytes | 479.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: error: GH007: Your push would publish a private email address.
remote: You can make your email public or disable this protection by visiting:
remote: https://github.com/settings/emails
To github.com:Carlarlgfy/git-test.git
 ! [remote rejected] main -> main (push declined due to email privacy restrictions)
error: failed to push some refs to 'github.com:Carlarlgfy/git-test.git'
❯ git config --global user.email marquispique@gmail.com
❯ git config --global user.email marquispique@gmail.com
❯ git commit --amend --reset-author
[main 7d5d2bd] these are test files
 2 files changed, 8 insertions(+)
 create mode 100644 testfile.txt
 create mode 100644 testfile1.txt
❯ git push origin main --force
Enter passphrase for key '/Users/carlmarquis-olson/.ssh/id_ed25519': 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 474 bytes | 474.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: error: GH007: Your push would publish a private email address.
remote: You can make your email public or disable this protection by visiting:
remote: https://github.com/settings/emails
To github.com:Carlarlgfy/git-test.git
 ! [remote rejected] main -> main (push declined due to email privacy restrictions)
error: failed to push some refs to 'github.com:Carlarlgfy/git-test.git'
❯ git config --global user.email marquispique@gmail.com
❯ git commit --amend --reset-author
[main 4b59b87] these are test files
 2 files changed, 8 insertions(+)
 create mode 100644 testfile.txt
 create mode 100644 testfile1.txt
❯ git push origin main
Enter passphrase for key '/Users/carlmarquis-olson/.ssh/id_ed25519': 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 474 bytes | 474.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: error: GH007: Your push would publish a private email address.
remote: You can make your email public or disable this protection by visiting:
remote: https://github.com/settings/emails
To github.com:Carlarlgfy/git-test.git
 ! [remote rejected] main -> main (push declined due to email privacy restrictions)
error: failed to push some refs to 'github.com:Carlarlgfy/git-test.git'
❯ git config --global user.email
marquispique@gmail.com
❯ git config --global user.email "12345678+YourUsername@users.noreply.github.com"
❯ git commit --amend --reset-author
[main 67401e6] these are test files
 2 files changed, 8 insertions(+)
 create mode 100644 testfile.txt
 create mode 100644 testfile1.txt
❯ git push origin main --force
Enter passphrase for key '/Users/carlmarquis-olson/.ssh/id_ed25519': 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 496 bytes | 496.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To github.com:Carlarlgfy/git-test.git
   87c581e..67401e6  main -> main
❯ git push origin main
Enter passphrase for key '/Users/carlmarquis-olson/.ssh/id_ed25519': 
Enter passphrase for key '/Users/carlmarquis-olson/.ssh/id_ed25519': 
Everything up-to-date
❯ git config --global user.name "Carlarlgfy"
❯ git config --global user.email "marquispique@gmail.com"
❯ git config --global --list
user.name=Carlarlgfy
user.email=marquispique@gmail.com
init.defaultbranch=main
pull.rebase=false
core.excludesfile=/Users/carlmarquis-olson/.gitignore_global
core.autocrlf=input
❯ git commit --amend --reset-author
[main 853bf41] these are test files
 2 files changed, 8 insertions(+)
 create mode 100644 testfile.txt
 create mode 100644 testfile1.txt
❯ git push origin main --force
Enter passphrase for key '/Users/carlmarquis-olson/.ssh/id_ed25519': 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 474 bytes | 474.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: error: GH007: Your push would publish a private email address.
remote: You can make your email public or disable this protection by visiting:
remote: https://github.com/settings/emails
To github.com:Carlarlgfy/git-test.git
 ! [remote rejected] main -> main (push declined due to email privacy restrictions)
error: failed to push some refs to 'github.com:Carlarlgfy/git-test.git'
❯ git push origin main
Enter passphrase for key '/Users/carlmarquis-olson/.ssh/id_ed25519': 
To github.com:Carlarlgfy/git-test.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'github.com:Carlarlgfy/git-test.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. If you want to integrate the remote changes,
hint: use 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
❯ git pull origin main --rebase
Enter passphrase for key '/Users/carlmarquis-olson/.ssh/id_ed25519': 
From github.com:Carlarlgfy/git-test
 * branch            main       -> FETCH_HEAD
warning: skipped previously applied commit 853bf41
hint: use --reapply-cherry-picks to include skipped commits
hint: Disable this message with "git config set advice.skippedCherryPicks false"
Successfully rebased and updated refs/heads/main.
❯ git push origin main
Enter passphrase for key '/Users/carlmarquis-olson/.ssh/id_ed25519': 
Everything up-to-date
❯ touch testfile2.txt
❯ open -e testfile2.txt
❯ open -e testfile1.txt
❯ git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   testfile1.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	testfile2.txt

no changes added to commit (use "git add" and/or "git commit -a")
❯ git add testfile1.txt testfile2.txt
❯ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	modified:   testfile1.txt
	new file:   testfile2.txt

❯ git commit
Aborting commit due to empty commit message.
❯ git push origin main
Enter passphrase for key '/Users/carlmarquis-olson/.ssh/id_ed25519': 
Everything up-to-date
❯ giot status
zsh: command not found: giot
❯ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	modified:   testfile1.txt
	new file:   testfile2.txt

❯ git commit -m "This is a second commit
dquote> "
[main 93e9553] This is a second commit
 2 files changed, 4 insertions(+), 1 deletion(-)
 create mode 100644 testfile2.txt
❯ git push origin main
Enter passphrase for key '/Users/carlmarquis-olson/.ssh/id_ed25519': 
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 553 bytes | 553.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To github.com:Carlarlgfy/git-test.git
   67401e6..93e9553  main -> main
❯ touch hello_world.txt
❯ git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	hello_world.txt

nothing added to commit but untracked files present (use "git add" to track)
❯ open -e hello_world.txt
❯ open -e hello_world.txt
❯ git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	hello_world.txt

nothing added to commit but untracked files present (use "git add" to track)
❯ git add hello_world.txt
❯ git commit -m "add hello_world.txt"
[main 6418418] add hello_world.txt
 1 file changed, 2 insertions(+)
 create mode 100644 hello_world.txt
❯ git status
On branch main
nothing to commit, working tree clean
❯ git log
commit 64184180a87934881f6302524af0f73edf3d3fde (HEAD -> main)
Author: Carlarlgfy <marquispique@gmail.com>
Date:   Tue Mar 18 14:15:50 2025 -0400

    add hello_world.txt

commit 93e9553cc6366d11c95eb3b16ba29955fe44be9d (origin/main)
Author: Carlarlgfy <marquispique@gmail.com>
Date:   Tue Mar 18 14:08:08 2025 -0400

    This is a second commit

commit 67401e6d4d9df67a2f75c6970a515d297c4ce6e3
Author: Carlarlgfy <12345678+YourUsername@users.noreply.github.com>
Date:   Tue Mar 18 13:54:51 2025 -0400

    these are test files

commit 87c581e476cc134235f5a80e99be6e01c3f6922b
Author: Carlarlgfy <90008064+Carlarlgfy@users.noreply.github.com>
Date:   Tue Mar 18 13:21:35 2025 -0400

    Initial commit
❯ open -e README.md
 ~/git-test  main                                                  ✔  14:18:02 
