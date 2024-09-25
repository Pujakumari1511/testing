s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % subl README.md
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % ls -ltar
total 8
drwx------@ 14 s2400794  staff  448 Sep 25 21:37 ..
drwxr-xr-x   9 s2400794  staff  288 Sep 25 21:41 .git
drwxr-xr-x@  4 s2400794  staff  128 Sep 25 21:45 .
-rw-r--r--   1 s2400794  staff  703 Sep 25 21:45 README.md
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % cat README.md 
Create a new GH repo for testing
create local repo for testing
In readme file write down all steps you do for this task.
Connect both repo
Make changes on the local repo and then push it to the remote repo
Make changes to the remote repository.
Make changes on the local repository and then push it to the remote repository.
Solve merge conflict.
Update the readme file with instructions how to avoide merge conflicts and how to solve it.

git checkout -b my_branch_name // Create and switch to a new branch
git checkout existing branch // switch branches
git push origin my_branch_name // push branch to remote repo
git pull origin my_branch_name // pull changes from a specific branch on a remote repo%    s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	README.md

nothing added to commit but untracked files present (use "git add" to track)
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git add README.md 
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git status       
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
	new file:   README.md

s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git commit -m "adding readme file"
[main (root-commit) d5bd8d6] adding readme file
 1 file changed, 14 insertions(+)
 create mode 100644 README.md
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git status
On branch main
nothing to commit, working tree clean
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git remote add origin https://github.com/Pujakumari1511/testing.git
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git status
On branch main
nothing to commit, working tree clean
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 520 bytes | 520.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Pujakumari1511/testing.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % subl README.md 
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git push
Everything up-to-date
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git add .
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	modified:   README.md

s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git commit -m "Update readme file"
[main 51ef581] Update readme file
 1 file changed, 15 insertions(+), 13 deletions(-)
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 388 bytes | 388.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Pujakumari1511/testing.git
   d5bd8d6..51ef581  main -> main
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git log
commit 51ef581979557f53fb020fb5a6ee0f58a09a4d86 (HEAD -> main, origin/main)
Author: Pujakumari1511 <puja.kumari6494@gmail.com>
Date:   Wed Sep 25 22:05:16 2024 +0300

    Update readme file

commit d5bd8d6176b408f700ea4cc442a00ab44428a366
Author: Pujakumari1511 <puja.kumari6494@gmail.com>
Date:   Wed Sep 25 21:54:27 2024 +0300

    adding readme file
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % subl README.md 
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % subl puja.md
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git status                        
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	puja.md

nothing added to commit but untracked files present (use "git add" to track)
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git add .
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git commit -m "add puja.md file"
[main a5db337] add puja.md file
 1 file changed, 1 insertion(+)
 create mode 100644 puja.md
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git push
To https://github.com/Pujakumari1511/testing.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Pujakumari1511/testing.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % subl README.md 
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git add .
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git commit -m "upd"
[main 3257c29] upd
 1 file changed, 1 insertion(+), 1 deletion(-)
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git commit --amend 
[main 0d68fd6] Add new line to readme
 Date: Wed Sep 25 22:17:30 2024 +0300
 1 file changed, 1 insertion(+), 1 deletion(-)
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git push
To https://github.com/Pujakumari1511/testing.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Pujakumari1511/testing.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git pull
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 929 bytes | 132.00 KiB/s, done.
From https://github.com/Pujakumari1511/testing
   51ef581..49d08a8  main       -> origin/main
hint: You have divergent branches and need to specify how to reconcile them.
hint: You can do so by running one of the following commands sometime before
hint: your next pull:
hint:
hint:   git config pull.rebase false  # merge
hint:   git config pull.rebase true   # rebase
hint:   git config pull.ff only       # fast-forward only
hint:
hint: You can replace "git config" with "git config --global" to set a default
hint: preference for all repositories. You can also pass --rebase, --no-rebase,
hint: or --ff-only on the command line to override the configured default per
hint: invocation.
fatal: Need to specify how to reconcile divergent branches.
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git pull --rebase
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
error: could not apply 0d68fd6... Add new line to readme
hint: Resolve all conflicts manually, mark them as resolved with
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".
hint: To abort and get back to the state before "git rebase", run "git rebase --abort".
hint: Disable this message with "git config advice.mergeConflict false"
Could not apply 0d68fd6... Add new line to readme
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % subl README.md 
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git status           
interactive rebase in progress; onto 49d08a8
Last commands done (2 commands done):
   pick a5db337 add puja.md file
   pick 0d68fd6 Add new line to readme
No commands remaining.
You are currently rebasing branch 'main' on '49d08a8'.
  (fix conflicts and then run "git rebase --continue")
  (use "git rebase --skip" to skip this patch)
  (use "git rebase --abort" to check out the original branch)

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to mark resolution)
	both modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git add README.md 
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git status
interactive rebase in progress; onto 49d08a8
Last commands done (2 commands done):
   pick a5db337 add puja.md file
   pick 0d68fd6 Add new line to readme
No commands remaining.
You are currently rebasing branch 'main' on '49d08a8'.
  (all conflicts fixed: run "git rebase --continue")

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	modified:   README.md

s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git rebase --continue
[detached HEAD 956c929] Add new line to readme
 1 file changed, 1 insertion(+)
Successfully rebased and updated refs/heads/main.
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git status
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % git push
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 8 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (6/6), 600 bytes | 600.00 KiB/s, done.
Total 6 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Pujakumari1511/testing.git
   49d08a8..956c929  main -> main
s2400794@BC-JNY03D7FFR-Kannettava-tietokone testing % 