# subModuleTest

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods
$

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods
$ mkdir subMod1

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods
$ mkdir subMod2

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods
$ mkdir mainGit

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods
$ ls
mainGit/  subMod1/  subMod2/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods
$ cd mainGit/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit
$ ls

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit
$ git clone https://github.com/chandreshtank/subModuleTest.git
Cloning into 'subModuleTest'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit
$ ls
subModuleTest/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit
$ cd subModuleTest/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ ls
README.md

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ touch a.txt

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ echo Hi > a.txt

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        a.txt

nothing added to commit but untracked files present (use "git add" to track)

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git add .

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git commit -m "a.txt added"
[master 15387ad] a.txt added
 1 file changed, 1 insertion(+)
 create mode 100644 a.txt

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git push -u origin master
Username for 'https://github.com': chandreshtank@gmail.com
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 281 bytes | 40.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/chandreshtank/subModuleTest.git
   617b550..15387ad  master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git submodule add https://github.com/chandreshtank/subMod1.git
Cloning into 'D:/projects/subMods/mainGit/subModuleTest/subMod1'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ ls
a.txt  README.md  subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ cd subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ ls
README.md

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ vi README.md

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ ls
README.md

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ cd ..

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ ls
a.txt  README.md  subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   .gitmodules
        new file:   subMod1


Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git diff

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ cd subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ ls
README.md

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ git diff

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ cd ..

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ ls
a.txt  README.md  subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git diff --submodule

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git diff --submodule --cached
diff --git a/.gitmodules b/.gitmodules
new file mode 100644
index 0000000..48d74dc
--- /dev/null
+++ b/.gitmodules
@@ -0,0 +1,3 @@
+[submodule "subMod1"]
+       path = subMod1
+       url = https://github.com/chandreshtank/subMod1.git
Submodule subMod1 0000000...78a7455 (new submodule)

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   .gitmodules
        new file:   subMod1


Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git commit -m "submodule Added"
[master 7604c84] submodule Added
 2 files changed, 4 insertions(+)
 create mode 100644 .gitmodules
 create mode 160000 subMod1

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git push -u origin master
Username for 'https://github.com': chandreshtank@gmail.com
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 427 bytes | 53.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/chandreshtank/subModuleTest.git
   15387ad..7604c84  master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ ls
a.txt  README.md  subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ echo "hello hello " >> subMod1/README.md

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git diff
diff --git a/subMod1 b/subMod1
--- a/subMod1
+++ b/subMod1
@@ -1 +1 @@
-Subproject commit 78a7455a27aa7b101c18afd2a31375bd7ad22c43
+Subproject commit 78a7455a27aa7b101c18afd2a31375bd7ad22c43-dirty

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)
  (commit or discard the untracked or modified content in submodules)

        modified:   subMod1 (modified content)

no changes added to commit (use "git add" and/or "git commit -a")

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git diff
diff --git a/subMod1 b/subMod1
--- a/subMod1
+++ b/subMod1
@@ -1 +1 @@
-Subproject commit 78a7455a27aa7b101c18afd2a31375bd7ad22c43
+Subproject commit 78a7455a27aa7b101c18afd2a31375bd7ad22c43-dirty

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git checkout subMod1/README.md
error: pathspec 'subMod1/README.md' did not match any file(s) known to git.

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git submodule update

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ ls
a.txt  README.md  subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ cd subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ ls
README.md

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ ls
README.md

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ git diff
diff --git a/README.md b/README.md
index e441ac1..e13bec6 100644
--- a/README.md
+++ b/README.md
@@ -1,2 +1,3 @@
 # subMod1
 sample sub module
+hello hello

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ ls
README.md

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ cd ..

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ ls
a.txt  README.md  subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git diff
diff --git a/subMod1 b/subMod1
--- a/subMod1
+++ b/subMod1
@@ -1 +1 @@
-Subproject commit 78a7455a27aa7b101c18afd2a31375bd7ad22c43
+Subproject commit 78a7455a27aa7b101c18afd2a31375bd7ad22c43-dirty

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ ls
a.txt  README.md  subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ cd subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ ls
README.md

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ cd ..

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ ls
a.txt  README.md  subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ ls
a.txt  README.md  subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ cd ..

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit
$ ls
subModuleTest/

< At this point, Just to check, we went to the github.com and in github.com , i have created and commited a new file called subfile.txt in 
subMod1 git repository, now if anyone clones subMod1.git repo, they will get README.md and subfile.txt file as they both are now in subMod1 git repo. 
Now here, we are cloning the submoduleTest git repository and we will see when we will updte subModuleTest git repo's submodule which is "subMod1"
Whether we will get the new version of SubMod1 with both the file, Readme.md and subfile.txt or the previous version of subMod1 which has only 
README.md file and that was the version which we have added to the submodule

Going forward you will see that it will take the preivious version of SubMod1 even thought the new version is available of submod1 while cloning subModuelTest 
git repo.

then we will see how we can update the SubModuleTest's submodule's so that others also get the updated submodules.

>

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit
$ mkdir temmmm

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit
$ ls
subModuleTest/  temmmm/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit
$ cd tm
bash: cd: tm: No such file or directory

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit
$ cd temmmm/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/temmmm
$ ls

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/temmmm
$ git clone https://github.com/chandreshtank/subModuleTest.git
Cloning into 'subModuleTest'...
remote: Enumerating objects: 9, done.
remote: Counting objects: 100% (9/9), done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 9 (delta 0), reused 6 (delta 0), pack-reused 0
Unpacking objects: 100% (9/9), done.

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/temmmm
$ ls
subModuleTest/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/temmmm
$ cd subModuleTest/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/temmmm/subModuleTest (master)
$ ls
a.txt  README.md  subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/temmmm/subModuleTest (master)
$ cd subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/temmmm/subModuleTest/subMod1 (master)
$ ls

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/temmmm/subModuleTest/subMod1 (master)
$ cd ..

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/temmmm/subModuleTest (master)
$ ls
a.txt  README.md  subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/temmmm/subModuleTest (master)
$ ls
a.txt  README.md  subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/temmmm/subModuleTest (master)
$ git submodule init
Submodule 'subMod1' (https://github.com/chandreshtank/subMod1.git) registered for path 'subMod1'

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/temmmm/subModuleTest (master)
$ git submodule update
Cloning into 'D:/projects/subMods/mainGit/temmmm/subModuleTest/subMod1'...
Submodule path 'subMod1': checked out '78a7455a27aa7b101c18afd2a31375bd7ad22c43'

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/temmmm/subModuleTest (master)
$ ls
a.txt  README.md  subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/temmmm/subModuleTest (master)
$ cd subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/temmmm/subModuleTest/subMod1 ((78a7455...))
$ ls
README.md

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/temmmm/subModuleTest/subMod1 ((78a7455...))
$ cd ..

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/temmmm/subModuleTest (master)
$ ls
a.txt  README.md  subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/temmmm/subModuleTest (master)
$

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/temmmm/subModuleTest (master)
$ so here, even after we have added another file (subfile.txt) directly in github.com, and after that we have cloned ou
r directory with submodule, the cloned directory will only have the previous version of submodule which doesn't have su
bfile.txt file. It only have README.md file. That is because the submodule "subMod1" is not updated for submoduleTest g
it repository. for submoduleTest git repository, the submodule "subMod1" is still running as the previous commit of sub
Mod1.
bash: syntax error near unexpected token `('

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/temmmm/subModuleTest (master)
$ Now lets update the submodule 1
bash: Now: command not found

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/temmmm/subModuleTest (master)
$ cd ..

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/temmmm
$ ls
subModuleTest/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/temmmm
$ cd ..

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit
$ ls
subModuleTest/  temmmm/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit
$ cd subModuleTest/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ ls
a.txt  README.md  subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ cd subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ ls
README.md

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ cd ..

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ ls
a.txt  README.md  subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git diff
diff --git a/subMod1 b/subMod1
--- a/subMod1
+++ b/subMod1
@@ -1 +1 @@
-Subproject commit 78a7455a27aa7b101c18afd2a31375bd7ad22c43
+Subproject commit 78a7455a27aa7b101c18afd2a31375bd7ad22c43-dirty

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)
  (commit or discard the untracked or modified content in submodules)

        modified:   subMod1 (modified content)

no changes added to commit (use "git add" and/or "git commit -a")

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ Let's take update of git submodule in this subModuleTest git repository and then commit it so that git submodule gets
 updated.
> '
bash: $'Lets take update of git submodule in this subModuleTest git repository and then commit it so that git submodule gets updated.\n': command not found

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ ls
a.txt  README.md  subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ cd subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ ls
README.md

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ git fetch
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.
From https://github.com/chandreshtank/subMod1
   78a7455..9b68a63  master     -> origin/master

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ ls
README.md

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ git diff
diff --git a/README.md b/README.md
index e441ac1..e13bec6 100644
--- a/README.md
+++ b/README.md
@@ -1,2 +1,3 @@
 # subMod1
 sample sub module
+hello hello

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ git merge origin/master
Updating 78a7455..9b68a63
Fast-forward
 subfile.txt | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 subfile.txt

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ ls
README.md  subfile.txt

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ git diff
diff --git a/README.md b/README.md
index e441ac1..e13bec6 100644
--- a/README.md
+++ b/README.md
@@ -1,2 +1,3 @@
 # subMod1
 sample sub module
+hello hello

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ Now let's update this submodule to git repository so that next time if anyone takes the git submoduleTest git, they s
hould get the new version of submodule'
bash: Now: command not found

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ git submodule update --remote

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ git submodule update --remote subMod1
error: pathspec 'subMod1' did not match any file(s) known to git.

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ If this doesnt work then you can always just commit in your subModuelTest git repository and then next time if anyone
 is cloning it our updating it, they will get new version of submodule
bash: If: command not found

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ git commit -m "updating sub module"
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
        modified:   README.md

no changes added to commit

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ git log
commit 9b68a63b26d2deb13aeb822d953fc795d1bd5019 (HEAD -> master, origin/master, origin/HEAD)
Author: chandreshtank <34219877+chandreshtank@users.noreply.github.com>
Date:   Wed Jan 23 17:20:36 2019 +0530

    Create subfile.txt

commit 78a7455a27aa7b101c18afd2a31375bd7ad22c43
Author: chandreshtank <34219877+chandreshtank@users.noreply.github.com>
Date:   Wed Jan 23 17:06:36 2019 +0530

    Initial commit

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ git diff
diff --git a/README.md b/README.md
index e441ac1..e13bec6 100644
--- a/README.md
+++ b/README.md
@@ -1,2 +1,3 @@
 # subMod1
 sample sub module
+hello hello

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ ls
README.md  subfile.txt

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest/subMod1 (master)
$ cd ..

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ ls
a.txt  README.md  subMod1/

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)
  (commit or discard the untracked or modified content in submodules)

        modified:   subMod1 (new commits, modified content)

no changes added to commit (use "git add" and/or "git commit -a")

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git add subMod1

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   subMod1

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)
  (commit or discard the untracked or modified content in submodules)

        modified:   subMod1 (modified content)


Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git commit -m "updated submodule"
[master 43466c7] updated submodule
 1 file changed, 1 insertion(+), 1 deletion(-)

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ git push -u origin master
Username for 'https://github.com': chandreshtank@gmail.com
Counting objects: 2, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 254 bytes | 63.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/chandreshtank/subModuleTest.git
   7604c84..43466c7  master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
$ Now the submodule is updated so next time if anyone clones the subModuleTest directory, they wil get the new version
of submodule
bash: Now: command not found

Chandresh.Tank@Chandresh-PC MINGW64 /d/projects/subMods/mainGit/subModuleTest (master)
