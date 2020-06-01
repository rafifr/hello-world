Last login: Sat May  9 13:59:38 on console

The default interactive shell is now zsh.
To update your account to use zsh, please run `chsh -s /bin/zsh`.
For more details, please visit https://support.apple.com/kb/HT208050.
(base) Rafis-New-MacBook-Pro:~ rafifried$ git --version
git version 2.21.1 (Apple Git-122.3)
(base) Rafis-New-MacBook-Pro:~ rafifried$ git config --global "Rafi Fried"
error: key does not contain a section: Rafi Fried
(base) Rafis-New-MacBook-Pro:~ rafifried$ cat ~/.gitconfig
cat: /Users/rafifried/.gitconfig: No such file or directory
(base) Rafis-New-MacBook-Pro:~ rafifried$ cat ~/.config/git/config
cat: /Users/rafifried/.config/git/config: No such file or directory
(base) Rafis-New-MacBook-Pro:~ rafifried$ ls ~
Applications	Documents	Dropbox		Mirror		Music		Pictures	Public
Desktop		Downloads	Library		Movies		OneDrive	Programming
(base) Rafis-New-MacBook-Pro:~ rafifried$ cat ~/.config
cat: /Users/rafifried/.config: Is a directory
(base) Rafis-New-MacBook-Pro:~ rafifried$ git config --list
credential.helper=osxkeychain
(base) Rafis-New-MacBook-Pro:~ rafifried$ git config --list
credential.helper=osxkeychain
(base) Rafis-New-MacBook-Pro:~ rafifried$ git config --list --show-origin
file:/Applications/Xcode.app/Contents/Developer/usr/share/git-core/gitconfig    credential.helper=osxkeychain
(base) Rafis-New-MacBook-Pro:~ rafifried$ git --version
git version 2.21.1 (Apple Git-122.3)
(base) Rafis-New-MacBook-Pro:~ rafifried$ git remote -v
fatal: not a git repository (or any of the parent directories): .git
(base) Rafis-New-MacBook-Pro:~ rafifried$ git config --global user.name "Rafi Fried"
(base) Rafis-New-MacBook-Pro:~ rafifried$ git config --global user.email rafifried1@gmail.com
(base) Rafis-New-MacBook-Pro:~ rafifried$ git config --list --show-origin
file:/Applications/Xcode.app/Contents/Developer/usr/share/git-core/gitconfig    credential.helper=osxkeychain
file:/Users/rafifried/.gitconfig        user.name=Rafi Fried
file:/Users/rafifried/.gitconfig        user.email=rafifried1@gmail.com
(base) Rafis-New-MacBook-Pro:~ rafifried$ git config --global core.editor "atom --wait"
(base) Rafis-New-MacBook-Pro:~ rafifried$ git config --list --show-origin
file:/Applications/Xcode.app/Contents/Developer/usr/share/git-core/gitconfig    credential.helper=osxkeychain
file:/Users/rafifried/.gitconfig        user.name=Rafi Fried
file:/Users/rafifried/.gitconfig        user.email=rafifried1@gmail.com
file:/Users/rafifried/.gitconfig        core.editor=atom --wait
(base) Rafis-New-MacBook-Pro:~ rafifried$ git config --list
credential.helper=osxkeychain
user.name=Rafi Fried
user.email=rafifried1@gmail.com
core.editor=atom --wait
(base) Rafis-New-MacBook-Pro:~ rafifried$ git config --global color.ui auto
(base) Rafis-New-MacBook-Pro:~ rafifried$ git config --list
credential.helper=osxkeychain
user.name=Rafi Fried
user.email=rafifried1@gmail.com
core.editor=atom --wait
color.ui=auto
(base) Rafis-New-MacBook-Pro:~ rafifried$ git config user.name
Rafi Fried
(base) Rafis-New-MacBook-Pro:~ rafifried$ git help config
(base) Rafis-New-MacBook-Pro:~ rafifried$ git add -h
usage: git add [<options>] [--] <pathspec>...

    -n, --dry-run         dry run
    -v, --verbose         be verbose

    -i, --interactive     interactive picking
    -p, --patch           select hunks interactively
    -e, --edit            edit current diff and apply
    -f, --force           allow adding otherwise ignored files
    -u, --update          update tracked files
    --renormalize         renormalize EOL of tracked files (implies -u)
    -N, --intent-to-add   record only the fact that the path will be added later
    -A, --all             add changes from all tracked and untracked files
    --ignore-removal      ignore paths removed in the working tree (same as --no-all)
    --refresh             don't add, only refresh the index
    --ignore-errors       just skip files which cannot be added because of errors
    --ignore-missing      check if - even missing - files are ignored in dry run
    --chmod (+|-)x        override the executable bit of the listed files

(base) Rafis-New-MacBook-Pro:~ rafifried$ ls
Applications	Documents	Dropbox		Mirror		Music		Pictures	Public
Desktop		Downloads	Library		Movies		OneDrive	Programming
(base) Rafis-New-MacBook-Pro:~ rafifried$ cd Desktop/
(base) Rafis-New-MacBook-Pro:Desktop rafifried$ ls
 stocks.docx				Screen Shot 2020-03-26 at 07.05.14.png
3X.xlsx					Screen Shot 2020-05-22 at 13.34.02.png
Contacts for start-up.docx		Screen Shot 2020-05-28 at 21.30.26.png
Git					git_practice
(base) Rafis-New-MacBook-Pro:Desktop rafifried$ cd git_practice/
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ touch hello_word
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ ls
hello_word
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ ls
child_folder	hello_word
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ cd child_folder/
(base) Rafis-New-MacBook-Pro:child_folder rafifried$ cd ..
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ cd child_folder/ && touch hello_child
(base) Rafis-New-MacBook-Pro:child_folder rafifried$ ls
hello_child
(base) Rafis-New-MacBook-Pro:child_folder rafifried$ open hello_child 
(base) Rafis-New-MacBook-Pro:child_folder rafifried$ cd ..
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ ls
child_folder	hello_word
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ pwd
/Users/rafifried/Desktop/git_practice
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git init
Initialized empty Git repository in /Users/rafifried/Desktop/git_practice/.git/
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ ls
child_folder	hello_word
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ ls -a
.		..		.DS_Store	.git		child_folder	hello_word
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	.DS_Store
	child_folder/
	hello_word

nothing added to commit but untracked files present (use "git add" to track)
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git branch
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	.DS_Store
	child_folder/
	hello_word

nothing added to commit but untracked files present (use "git add" to track)
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git diff
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git add hello_word 
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   hello_word

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	.DS_Store
	child_folder/

(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git add -A
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   .DS_Store
	new file:   child_folder/hello_child
	new file:   hello_word

(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   .DS_Store
	new file:   child_folder/hello_child
	new file:   hello_word

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   hello_word

(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git checkout hello_word 
Updated 1 path from the index
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   .DS_Store
	new file:   child_folder/hello_child
	new file:   hello_word

(base) Rafis-New-MacBook-Pro:git_practice rafifried$ atom .
-bash: atom: command not found
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   .DS_Store
	new file:   child_folder/hello_child
	new file:   hello_word

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   hello_word

(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git checkout hello_word 
Updated 1 path from the index
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   .DS_Store
	new file:   child_folder/hello_child
	new file:   hello_word

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   hello_word

(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git diff
diff --git a/hello_word b/hello_word
index 7b95538..c5c86df 100644
--- a/hello_word
+++ b/hello_word
@@ -1,4 +1,6 @@
 This is my 1st revision of this file.
 It is my git practice.
 
-My 1st time changing this file after creating it
\ No newline at end of file
+My 1st time changing this file after creating it
+
+My 2nd change
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   .DS_Store
	new file:   child_folder/hello_child
	new file:   hello_word

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   hello_word

(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   .DS_Store
	new file:   child_folder/hello_child
	new file:   hello_word

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   child_folder/hello_child
	modified:   hello_word

(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git diff
diff --git a/child_folder/hello_child b/child_folder/hello_child
index 34d6ae0..093fdcc 100644
--- a/child_folder/hello_child
+++ b/child_folder/hello_child
@@ -1,2 +1,4 @@
 This is the child file.
-In the hello_child folder.
\ No newline at end of file
+In the hello_child folder.
+
+My 1st change to this child file
diff --git a/hello_word b/hello_word
index 7b95538..c5c86df 100644
--- a/hello_word
+++ b/hello_word
@@ -1,4 +1,6 @@
 This is my 1st revision of this file.
 It is my git practice.
 
-My 1st time changing this file after creating it
\ No newline at end of file
+My 1st time changing this file after creating it
+
+My 2nd change
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   .DS_Store
	new file:   child_folder/hello_child
	new file:   hello_word

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   child_folder/hello_child
	modified:   hello_word

(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git add hello_word 
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   .DS_Store
	new file:   child_folder/hello_child
	new file:   hello_word

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   child_folder/hello_child

(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git checkout child_folder/
Updated 1 path from the index
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   .DS_Store
	new file:   child_folder/hello_child
	new file:   hello_word
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git commit -m "This is my 1st commit"
[master (root-commit) 2649c69] This is my 1st commit
 3 files changed, 8 insertions(+)
 create mode 100644 .DS_Store
 create mode 100644 child_folder/hello_child
 create mode 100644 hello_word
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git status
On branch master
nothing to commit, working tree clean
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   child_folder/hello_child

no changes added to commit (use "git add" and/or "git commit -a")
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git diff
diff --git a/child_folder/hello_child b/child_folder/hello_child
index 34d6ae0..25f11a8 100644
--- a/child_folder/hello_child
+++ b/child_folder/hello_child
@@ -1,2 +1,4 @@
 This is the child file.
-In the hello_child folder.
\ No newline at end of file
+In the hello_child folder.
+
+Second changes cycle
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git checkout child_folder/
Updated 1 path from the index
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   child_folder/hello_child

no changes added to commit (use "git add" and/or "git commit -a")
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git diff
diff --git a/child_folder/hello_child b/child_folder/hello_child
index 34d6ae0..deb0d60 100644
--- a/child_folder/hello_child
+++ b/child_folder/hello_child
@@ -1,2 +1,4 @@
 This is the child file.
-In the hello_child folder.
\ No newline at end of file
+In the hello_child folder.
+
+My 2nd round of change
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git add child_folder/
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git diff
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	modified:   child_folder/hello_child

(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git commit -m "This is my 2nd commit"
[master 3c9c87b] This is my 2nd commit
 1 file changed, 3 insertions(+), 1 deletion(-)
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git status
On branch master
nothing to commit, working tree clean
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git log
commit 3c9c87b6fecb3413eb923ea1a2ccf1766cde206f (HEAD -> master)
Author: Rafi Fried <rafifried1@gmail.com>
Date:   Sun May 31 13:47:43 2020 -0700

    This is my 2nd commit

commit 2649c698ade248419301c2a0c8f22ebb2f0262b8
Author: Rafi Fried <rafifried1@gmail.com>
Date:   Sun May 31 13:42:36 2020 -0700

    This is my 1st commit
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git checkout 2649c698ade248419301c2a0c8f22ebb2f0262b8
Note: checking out '2649c698ade248419301c2a0c8f22ebb2f0262b8'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by performing another checkout.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -b with the checkout command again. Example:

  git checkout -b <new-branch-name>

HEAD is now at 2649c69 This is my 1st commit
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git log
commit 2649c698ade248419301c2a0c8f22ebb2f0262b8 (HEAD)
Author: Rafi Fried <rafifried1@gmail.com>
Date:   Sun May 31 13:42:36 2020 -0700

    This is my 1st commit
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git checkout 3c9c87b6fecb3413eb923ea1a2ccf1766cde206f
Previous HEAD position was 2649c69 This is my 1st commit
HEAD is now at 3c9c87b This is my 2nd commit
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ git log
commit 3c9c87b6fecb3413eb923ea1a2ccf1766cde206f (HEAD, master)
Author: Rafi Fried <rafifried1@gmail.com>
Date:   Sun May 31 13:47:43 2020 -0700

    This is my 2nd commit

commit 2649c698ade248419301c2a0c8f22ebb2f0262b8
Author: Rafi Fried <rafifried1@gmail.com>
Date:   Sun May 31 13:42:36 2020 -0700

    This is my 1st commit
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ pwd
/Users/rafifried/Desktop/git_practice
(base) Rafis-New-MacBook-Pro:git_practice rafifried$ cd ..
(base) Rafis-New-MacBook-Pro:Desktop rafifried$ pwd
/Users/rafifried/Desktop
(base) Rafis-New-MacBook-Pro:Desktop rafifried$ las
-bash: las: command not found
(base) Rafis-New-MacBook-Pro:Desktop rafifried$ ls
 stocks.docx				Screen Shot 2020-05-22 at 13.34.02.png
3X.xlsx					Screen Shot 2020-05-28 at 21.30.26.png
Contacts for start-up.docx		git_practice
Git					my 2nd git trial
Screen Shot 2020-03-26 at 07.05.14.png
(base) Rafis-New-MacBook-Pro:Desktop rafifried$ ls
 stocks.docx				Screen Shot 2020-05-22 at 13.34.02.png
3X.xlsx					Screen Shot 2020-05-28 at 21.30.26.png
Contacts for start-up.docx		git_practice
Git					my_git_trial_2
Screen Shot 2020-03-26 at 07.05.14.png
(base) Rafis-New-MacBook-Pro:Desktop rafifried$ cd my_git_trial_2/
(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ ls
(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ ls -a
.	..
(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git init
Initialized empty Git repository in /Users/rafifried/Desktop/my_git_trial_2/.git/
(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ ls -a
.	..	.git
(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git status
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)
(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	file1

nothing added to commit but untracked files present (use "git add" to track)
(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	dir1/
	file1

nothing added to commit but untracked files present (use "git add" to track)
(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git add file1 
(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   file1

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	dir1/

(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git add dir1/
(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   dir1/file2
	new file:   file1

(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   dir1/file2
	new file:   file1

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   dir1/file2

(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git add dir1/
(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git log
fatal: your current branch 'master' does not have any commits yet
(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ gir checkout dir1/
-bash: gir: command not found
(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git checkout dir1/
Updated 0 paths from the index
(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ gir status
-bash: gir: command not found
(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   dir1/file2
	new file:   file1

(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git checkout dir1/file2 
Updated 0 paths from the index
(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   dir1/file2
	new file:   file1

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   dir1/file2

(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git checkout dir1/file2 
Updated 1 path from the index
(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   dir1/file2
	new file:   file1

(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   dir1/file2
	new file:   file1

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   dir1/file2

(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git add dir1/file2 
(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   dir1/file2
	new file:   file1

(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git log
fatal: your current branch 'master' does not have any commits yet
(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git commit -m "my 1st commit"
[master (root-commit) a8e19f5] my 1st commit
 2 files changed, 4 insertions(+)
 create mode 100644 dir1/file2
 create mode 100644 file1
(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git log
commit a8e19f55c23f90fbb256419b52015f3614f5eb16 (HEAD -> master)
Author: Rafi Fried <rafifried1@gmail.com>
Date:   Sun May 31 17:43:07 2020 -0700

    my 1st commit
(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ pwd
/Users/rafifried/Desktop/my_git_trial_2
(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ git remote
(base) Rafis-New-MacBook-Pro:my_git_trial_2 rafifried$ cd ..
(base) Rafis-New-MacBook-Pro:Desktop rafifried$ pwd
/Users/rafifried/Desktop
(base) Rafis-New-MacBook-Pro:Desktop rafifried$ git clone https://github.com/rafifr/hello-world
Cloning into 'hello-world'...
remote: Enumerating objects: 7, done.
remote: Total 7 (delta 0), reused 0 (delta 0), pack-reused 7
Unpacking objects: 100% (7/7), done.
(base) Rafis-New-MacBook-Pro:Desktop rafifried$ ls
 stocks.docx				Screen Shot 2020-05-28 at 21.30.26.png
3X.xlsx					Screen Shot 2020-05-31 at 18.44.58.png
Contacts for start-up.docx		git_practice
Screen Shot 2020-03-26 at 07.05.14.png	hello-world
Screen Shot 2020-05-22 at 13.34.02.png	my_git_trial_2
(base) Rafis-New-MacBook-Pro:Desktop rafifried$ cd hello-world/
(base) Rafis-New-MacBook-Pro:hello-world rafifried$ ls
README.md
(base) Rafis-New-MacBook-Pro:hello-world rafifried$ cat README.md 
# hello-world
My 1st repository
Adding a 1st comment
(base) Rafis-New-MacBook-Pro:hello-world rafifried$ git remote
origin
(base) Rafis-New-MacBook-Pro:hello-world rafifried$ git remote -v
origin	https://github.com/rafifr/hello-world (fetch)
origin	https://github.com/rafifr/hello-world (push)
(base) Rafis-New-MacBook-Pro:hello-world rafifried$ 
