I will be back!@DESKTOP-7S4OCHI MINGW32 /d/test/git (master)
$ git config --global user.name "ludgoole"

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/test/git (master)
$ git config --global user.email "ludgoole@163.com"

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/test/git (master)
$ cd D:

I will be back!@DESKTOP-7S4OCHI MINGW32 /d
$ cd www
bash: cd: www: No such file or directory

I will be back!@DESKTOP-7S4OCHI MINGW32 /d
$ mkdir^C

I will be back!@DESKTOP-7S4OCHI MINGW32 /d
$ mkdir www

I will be back!@DESKTOP-7S4OCHI MINGW32 /d
$ cd www

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www
$ mkdir testgit

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www
$ pwd
/d/www

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www
$ cd testgit

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit
$ pwd
/d/www/testgit

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit
$ git init
Initialized empty Git repository in D:/www/testgit/.git/

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git add readme.txt

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git commit -m "first"
[master (root-commit) e6b95fc] first
 1 file changed, 1 insertion(+)
 create mode 100644 readme.txt

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git status
On branch master
nothing to commit, working tree clean

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   readme.txt

no changes added to commit (use "git add" and/or "git commit -a")

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git diff readme.txt
diff --git a/readme.txt b/readme.txt
index b23c1c5..b72ce18 100644
--- a/readme.txt
+++ b/readme.txt
@@ -1 +1,2 @@
-111111
\ No newline at end of file
+111111
+222222
\ No newline at end of file

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git add readme.txt

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   readme.txt


I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git commit -m "two add 222222"
[master a5432b1] two add 222222
 1 file changed, 2 insertions(+), 1 deletion(-)

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git add readme.txt

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git log
commit a5432b124be9a7650a2c86f219863dc50d431dba (HEAD -> master)
Author: ludgoole <ludgoole@163.com>
Date:   Thu Feb 1 11:51:34 2018 +0800

    two add 222222

commit e6b95fc01dc4f9ad48a7d55b0b48786bcc10d0d7
Author: ludgoole <ludgoole@163.com>
Date:   Thu Feb 1 11:47:32 2018 +0800

    first

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git commit -m "three add 333333"
[master d15f702] three add 333333
 1 file changed, 2 insertions(+), 1 deletion(-)

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git log
commit d15f702d185578a24e966db177c45da76c7f7460 (HEAD -> master)
Author: ludgoole <ludgoole@163.com>
Date:   Thu Feb 1 11:53:40 2018 +0800

    three add 333333

commit a5432b124be9a7650a2c86f219863dc50d431dba
Author: ludgoole <ludgoole@163.com>
Date:   Thu Feb 1 11:51:34 2018 +0800

    two add 222222

commit e6b95fc01dc4f9ad48a7d55b0b48786bcc10d0d7
Author: ludgoole <ludgoole@163.com>
Date:   Thu Feb 1 11:47:32 2018 +0800

    first

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git log -pretty=oneline
fatal: unrecognized argument: -pretty=oneline

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git log --pritty=oneline
fatal: unrecognized argument: --pritty=oneline

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git log --pretty=oneline
d15f702d185578a24e966db177c45da76c7f7460 (HEAD -> master) three add 333333
a5432b124be9a7650a2c86f219863dc50d431dba two add 222222
e6b95fc01dc4f9ad48a7d55b0b48786bcc10d0d7 first

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git reset --hard HEAD^
HEAD is now at a5432b1 two add 222222

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git reset --hard head^
fatal: ambiguous argument 'hehead^': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git reset --hard HEAD^
HEAD is now at e6b95fc first

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ cat readme.txt
111111
I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git log
commit e6b95fc01dc4f9ad48a7d55b0b48786bcc10d0d7 (HEAD -> master)
Author: ludgoole <ludgoole@163.com>
Date:   Thu Feb 1 11:47:32 2018 +0800

    first

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git reflog
e6b95fc (HEAD -> master) HEAD@{0}: reset: moving to HEAD^
a5432b1 HEAD@{1}: reset: moving to HEAD^
d15f702 HEAD@{2}: commit: three add 333333
a5432b1 HEAD@{3}: commit: two add 222222
e6b95fc (HEAD -> master) HEAD@{4}: commit (initial): first

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git reset --hard d15f702
HEAD is now at d15f702 three add 333333

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ cat readme.txt
111111
222222
333333

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ cd ~/.ssh
bash: cd: /c/Users/I will be back!/.ssh: No such file or directory

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ ssh-keygen -t rsa -C "ludgoole@163.com"
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/I will be back!/.ssh/id_rsa):
Created directory '/c/Users/I will be back!/.ssh'.
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/I will be back!/.ssh/id_rsa.
Your public key has been saved in /c/Users/I will be back!/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:6qmBVqygw4WjmAAuI0ycp3NdZqx/MoQwX8d82uwlxUk ludgoole@163.com
The key's randomart image is:
+---[RSA 2048]----+
|             E   |
|. .   . o   o .  |
|.+ +   * + . +   |
|= +.= B . = .    |
|*B oo= .S. + .   |
|O+=+  o.  . o    |
|*.+ . .+ . .     |
| o   o .+        |
|    ..o          |
+----[SHA256]-----+

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git remote add origin http://github.com/ludgoole/testgit.git

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git push -u origin master
warning: redirecting to https://github.com/ludgoole/testgit.git/
Counting objects: 9, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (9/9), 631 bytes | 157.00 KiB/s, done.
Total 9 (delta 0), reused 0 (delta 0)
To http://github.com/ludgoole/testgit.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.

I will be back!@DESKTOP-7S4OCHI MINGW32 /d/www/testgit (master)
$ git colne https://github.com/ludgoole/testgit.git/
