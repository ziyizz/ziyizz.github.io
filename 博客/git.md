1.git config --local user.name '你的大名'

2.git config --local user.email '你的邮箱地址'

3.创建仓库
mkdir learn-git
git init

4.git add readme.md
git commit -m 'add readme.md'

5.向 readme.md 中添加一些文字内容，如：
life is shit ！！！
然后，提交修改，提交修改和提交文件是一样的步骤：
第一步，执行 git add 命令：
git add readme.md
同样也不会有任何提示，第二步，执行 git commit 命令：
git commit -m 'add first line of text'
在命令行工具上，会有如下提示：
[master (root-commit) fa77113] add first line of text
 1 file changed, 1 insertion(+)
 create mode 100644 readme.md
输出命令解释如下：
1 file changed：1个文件被改动（我们刚刚修改的readme.md文件）；
1 insertions：插入了1行内容（我们刚刚向readme.md文件中添加了一行代码）;

6.
小熊816@LAPTOP-NIRK96P1 MINGW64 ~/Desktop/runoob-text.git (master)
$ git init
Reinitialized existing Git repository in C:/Users/小熊816/Desktop/runoob-text.git/.git/

小熊816@LAPTOP-NIRK96P1 MINGW64 ~/Desktop/runoob-text.git (master)
$ git remote add origin https://gitee.com/zhangziyi-zzy/runoob-text.git

小熊816@LAPTOP-NIRK96P1 MINGW64 ~/Desktop/runoob-text.git (master)
$ git add "flappy bird"
warning: LF will be replaced by CRLF in flappy bird/index.css.
The file will have its original line endings in your working directory
warning: LF will be replaced by CRLF in flappy bird/index.js.
The file will have its original line endings in your working directory
warning: LF will be replaced by CRLF in flappy bird/utils.js.
The file will have its original line endings in your working directory

小熊816@LAPTOP-NIRK96P1 MINGW64 ~/Desktop/runoob-text.git (master)
$ git commit -m "zzz"
[master 1177629] zzz
 12 files changed, 552 insertions(+)
 create mode 100644 flappy bird/images/bird.png
 create mode 100644 flappy bird/images/birds.png
 create mode 100644 flappy bird/images/pipe1.png
 create mode 100644 flappy bird/images/pipe2.png
 create mode 100644 flappy bird/images/sky.png
 create mode 100644 "flappy bird/images/\345\233\276\347\244\272-1.jpg"
 create mode 100644 "flappy bird/images/\345\233\276\347\244\272-2.jpg"
 create mode 100644 "flappy bird/images/\346\265\201\347\250\213\345\233\276.png"
 create mode 100644 flappy bird/index.css
 create mode 100644 flappy bird/index.html
 create mode 100644 flappy bird/index.js
 create mode 100644 flappy bird/utils.js

小熊816@LAPTOP-NIRK96P1 MINGW64 ~/Desktop/runoob-text.git (master)
$ git push origin master
info: detecting host provider for 'https://gitee.com/'...
warning: ----------------- SECURITY WARNING ----------------
warning: | TLS certificate verification has been disabled! |
warning: ---------------------------------------------------
warning: HTTPS connections may not be secure. See https://aka.ms/gcmcore-tlsverify for more information.
warning: ----------------- SECURITY WARNING ----------------
warning: | TLS certificate verification has been disabled! |
warning: ---------------------------------------------------
warning: HTTPS connections may not be secure. See https://aka.ms/gcmcore-tlsverify for more information.
info: detecting host provider for 'https://gitee.com/'...
warning: ----------------- SECURITY WARNING ----------------
warning: | TLS certificate verification has been disabled! |
warning: ---------------------------------------------------
warning: HTTPS connections may not be secure. See https://aka.ms/gcmcore-tlsverify for more information.
remote: [session-9541ab8d] zhangziyi-zzy: Incorrect username or password (access token)
fatal: Authentication failed for 'https://gitee.com/zhangziyi-zzy/runoob-text.git/'

小熊816@LAPTOP-NIRK96P1 MINGW64 ~/Desktop/runoob-text.git (master)
$ git push origin master
info: detecting host provider for 'https://gitee.com/'...
warning: ----------------- SECURITY WARNING ----------------
warning: | TLS certificate verification has been disabled! |
warning: ---------------------------------------------------
warning: HTTPS connections may not be secure. See https://aka.ms/gcmcore-tlsverify for more information.
warning: ----------------- SECURITY WARNING ----------------
warning: | TLS certificate verification has been disabled! |
warning: ---------------------------------------------------
warning: HTTPS connections may not be secure. See https://aka.ms/gcmcore-tlsverify for more information.
info: detecting host provider for 'https://gitee.com/'...
warning: ----------------- SECURITY WARNING ----------------
warning: | TLS certificate verification has been disabled! |
warning: ---------------------------------------------------
warning: HTTPS connections may not be secure. See https://aka.ms/gcmcore-tlsverify for more information.
To https://gitee.com/zhangziyi-zzy/runoob-text.git
 ! [rejected]        master -> master (fetch first)
error: failed to push some refs to 'https://gitee.com/zhangziyi-zzy/runoob-text.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

小熊816@LAPTOP-NIRK96P1 MINGW64 ~/Desktop/runoob-text.git (master)
$ git push --help

小熊816@LAPTOP-NIRK96P1 MINGW64 ~/Desktop/runoob-text.git (master)
$ git remote -v
origin  https://gitee.com/zhangziyi-zzy/runoob-text.git (fetch)
origin  https://gitee.com/zhangziyi-zzy/runoob-text.git (push)

小熊816@LAPTOP-NIRK96P1 MINGW64 ~/Desktop/runoob-text.git (master)
$ git push\
> git push
git: 'pushgit' is not a git command. See 'git --help'.

小熊816@LAPTOP-NIRK96P1 MINGW64 ~/Desktop/runoob-text.git (master)
$ git push
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin master


小熊816@LAPTOP-NIRK96P1 MINGW64 ~/Desktop/runoob-text.git (master)
$ git remote rm orgin
error: No such remote: 'orgin'

小熊816@LAPTOP-NIRK96P1 MINGW64 ~/Desktop/runoob-text.git (master)
$ git remote rm origin

小熊816@LAPTOP-NIRK96P1 MINGW64 ~/Desktop/runoob-text.git (master)
$ git remote add github git@github.com:ziyizz/ziyizz.github.io.git

小熊816@LAPTOP-NIRK96P1 MINGW64 ~/Desktop/runoob-text.git (master)
$ git remote add gitee git@gitee.com:zhangziyi-zzy/runoob-text.git

小熊816@LAPTOP-NIRK96P1 MINGW64 ~/Desktop/runoob-text.git (master)
$ git remote -v
gitee   git@gitee.com:zhangziyi-zzy/runoob-text.git (fetch)
gitee   git@gitee.com:zhangziyi-zzy/runoob-text.git (push)
github  git@github.com:ziyizz/ziyizz.github.io.git (fetch)
github  git@github.com:ziyizz/ziyizz.github.io.git (push)

小熊816@LAPTOP-NIRK96P1 MINGW64 ~/Desktop/runoob-text.git (master)
$ git push github master
Enumerating objects: 24, done.
Counting objects: 100% (24/24), done.
Delta compression using up to 8 threads
Compressing objects: 100% (21/21), done.
Writing objects: 100% (24/24), 238.17 KiB | 1.50 MiB/s, done.
Total 24 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'master' on GitHub by visiting:
remote:      https://github.com/ziyizz/ziyizz.github.io/pull/new/master
remote:
To github.com:ziyizz/ziyizz.github.io.git
 * [new branch]      master -> master

小熊816@LAPTOP-NIRK96P1 MINGW64 ~/Desktop/runoob-text.git (master)
$ git push gitee master
git@gitee.com: Permission denied (publickey).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

小熊816@LAPTOP-NIRK96P1 MINGW64 ~/Desktop/runoob-text.git (master)
$
