$ git init
Initialized empty Git repository in C:/Users/Sheeba/Downloads/DevOpsProject/sample-project/.git/

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (master)
$ git branch

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        css/
        fonts/
        img/
        index.html

nothing added to commit but untracked files present (use "git add" to track)

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (master)
$ git config --global user.name "Vjash28"

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (master)
$ git config --global user.email "Vijay.aswath@tcs.com"

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (master)
$ git add .
warning: LF will be replaced by CRLF in css/site.css.
The file will have its original line endings in your working directory
warning: LF will be replaced by CRLF in index.html.
The file will have its original line endings in your working directory

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   css/site.css
        new file:   fonts/segoeuil.ttf
        new file:   img/cloneWhite.svg
        new file:   img/deployWhite.svg
        new file:   img/lightbulbWhite.svg
        new file:   img/stackWhite.svg
        new file:   img/successCloudNew.svg
        new file:   img/tweetThis.svg
        new file:   index.html


Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (master)
$ git commit
Aborting commit due to empty commit message.

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (master)
$ git commit -m "initial code"
[master (root-commit) be4ac37] initial code
 9 files changed, 198 insertions(+)
 create mode 100644 css/site.css
 create mode 100644 fonts/segoeuil.ttf
 create mode 100644 img/cloneWhite.svg
 create mode 100644 img/deployWhite.svg
 create mode 100644 img/lightbulbWhite.svg
 create mode 100644 img/stackWhite.svg
 create mode 100644 img/successCloudNew.svg
 create mode 100644 img/tweetThis.svg
 create mode 100644 index.html

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (master)
$ git checkout new-branch
error: pathspec 'new-branch' did not match any file(s) known to git

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (master)
$ git branch checkout new-branch
fatal: Not a valid object name: 'new-branch'.

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (master)
$ git checkout newChange
error: pathspec 'newChange' did not match any file(s) known to git

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (master)
$ ls
css/  fonts/  img/  index.html

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (master)
$ git branch
* master

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (master)
$ git checkout -b new-branch
Switched to a new branch 'new-branch'

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (new-branch)
$ ls
css/  fonts/  img/  index.html

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (new-branch)
$ ls
css/  fonts/  img/  index.html  notes.txt

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (new-branch)
$ git checkout master
Switched to branch 'master'

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (master)
$ ls
css/  fonts/  img/  index.html  notes.txt

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (master)
$ ls
css/  fonts/  img/  index.html

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (master)
$ git checkout new-branch
Switched to branch 'new-branch'

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (new-branch)
$ ls
css/  fonts/  img/  index.html

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (new-branch)
$ git add notes
fatal: pathspec 'notes' did not match any files

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (new-branch)
$ git add .

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (new-branch)
$ git status
On branch new-branch
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   notes.txt


Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (new-branch)
$ git commit -m "added a note file"
[new-branch 0675dc4] added a note file
 1 file changed, 1 insertion(+)
 create mode 100644 notes.txt

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (new-branch)
$ git status
On branch new-branch
nothing to commit, working tree clean

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (new-branch)
$ git switch master
Switched to branch 'master'

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (master)
$ ls
css/  fonts/  img/  index.html

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (master)
$ git merge new-branch
Updating be4ac37..0675dc4
Fast-forward
 notes.txt | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 notes.txt

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (master)
$ ls
css/  fonts/  img/  index.html  notes.txt

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (master)
$ git log
commit 0675dc427595dc26701c26e10309e095e58bf42d (HEAD -> master, new-branch)
Author: Vjash28 <Vijay.aswath@tcs.com>
Date:   Fri Oct 29 14:16:10 2021 +0530

    added a note file

commit be4ac3788297fbc430103face840d907afb78f29
Author: Vjash28 <Vijay.aswath@tcs.com>
Date:   Fri Oct 29 14:08:40 2021 +0530

    initial code

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (master)
$ git switch new-branch
Switched to branch 'new-branch'

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (new-branch)
$ git log
commit 0675dc427595dc26701c26e10309e095e58bf42d (HEAD -> new-branch, master)
Author: Vjash28 <Vijay.aswath@tcs.com>
Date:   Fri Oct 29 14:16:10 2021 +0530

    added a note file

commit be4ac3788297fbc430103face840d907afb78f29
Author: Vjash28 <Vijay.aswath@tcs.com>
Date:   Fri Oct 29 14:08:40 2021 +0530

    initial code

Sheeba@LAPTOP-R2P7SO0R MINGW64 ~/Downloads/DevOpsProject/sample-project (new-branch)
$
