
Inssert
 work/
 workspaceeclipse/
 workspacejavascript/

yamini@yamini-PC MINGW64 ~
$ ~cd./My Documents
bash: ~cd./My: No such file or directory

yamini@yamini-PC MINGW64 ~
$  git config --global user.name "Hemu967"

yamini@yamini-PC MINGW64 ~
$ git config -- user.email "himanshutyagi967@gmail.com"
fatal: not in a git directory

yamini@yamini-PC MINGW64 ~
$ git config --global user.email "himanshutyagi967@gmail.com"

yamini@yamini-PC MINGW64 ~
$ cd Desktop

yamini@yamini-PC MINGW64 ~/Desktop
$ clear

yamini@yamini-PC MINGW64 ~/Desktop
$ git clone https://github.com/Hemu967/testGitHub.git
Cloning into 'testGitHub'...
remote: Counting objects: 3, done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.

yamini@yamini-PC MINGW64 ~/Desktop
$ cd testGitHub

yamini@yamini-PC MINGW64 ~/Desktop/testGitHub (master)
$ vim README.md

yamini@yamini-PC MINGW64 ~/Desktop/testGitHub (master)
$ git status
On branch master
Your branch is up-to-date with 'origin/master'.
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

yamini@yamini-PC MINGW64 ~/Desktop/testGitHub (master)
$ git add README.md

yamini@yamini-PC MINGW64 ~/Desktop/testGitHub (master)
$ git commit -help
usage: git commit [<options>] [--] <pathspec>...

    -q, --quiet           suppress summary after successful commit
    -v, --verbose         show diff in commit message template

Commit message options
    -F, --file <file>     read message from file
    --author <author>     override author for commit
    --date <date>         override date for commit
    -m, --message <message>
                          commit message
    -c, --reedit-message <commit>
                          reuse and edit message from specified commit
    -C, --reuse-message <commit>
                          reuse message from specified commit
    --fixup <commit>      use autosquash formatted message to fixup specified co                                                                                                                mmit
    --squash <commit>     use autosquash formatted message to squash specified c                                                                                                                ommit
    --reset-author        the commit is authored by me now (used with -C/-c/--am                                                                                                                end)
    -s, --signoff         add Signed-off-by:
    -t, --template <file>
                          use specified template file
    -e, --edit            force edit of commit
    --cleanup <default>   how to strip spaces and #comments from message
    --status              include status in commit message template
    -S, --gpg-sign[=<key-id>]
                          GPG sign commit

Commit contents options
    -a, --all             commit all changed files
    -i, --include         add specified files to index for commit
    --interactive         interactively add files
    -p, --patch           interactively add changes
    -o, --only            commit only specified files
    -n, --no-verify       bypass pre-commit and commit-msg hooks
    --dry-run             show what would be committed
    --short               show status concisely
    --branch              show branch information
    --porcelain           machine-readable output
    --long                show status in long format (default)
    -z, --null            terminate entries with NUL
    --amend               amend previous commit
    --no-post-rewrite     bypass post-rewrite hook
    -u, --untracked-files[=<mode>]
                          show untracked files, optional modes: all, normal, no.                                                                                                                 (Default: all)


yamini@yamini-PC MINGW64 ~/Desktop/testGitHub (master)
$ git commit -m "update readme file for good"
[master 370a107] update readme file for good
 1 file changed, 29 insertions(+), 2 deletions(-)

yamini@yamini-PC MINGW64 ~/Desktop/testGitHub (master)
$ git log
commit 370a1072cd099ceaf4fe3197dca24e50b557daee
Author: Hemu967 <himanshutyagi967@gmail.com>
Date:   Fri Apr 7 21:09:51 2017 +0530

    update readme file for good

commit bdcb43c3308574af7cbbba16838cf43c1b3026a7
Author: Hemu967 <himanshutyagi967@gmail.com>
Date:   Fri Apr 7 20:49:17 2017 +0530

    Initial commit

yamini@yamini-PC MINGW64 ~/Desktop/testGitHub (master)
$ git status
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)
nothing to commit, working tree clean

yamini@yamini-PC MINGW64 ~/Desktop/testGitHub (master)
$ git remote add origin https://github.com/hemu967/testGitHub.git
fatal: remote origin already exists.

yamini@yamini-PC MINGW64 ~/Desktop/testGitHub (master)
$ git push -u origin master
Counting objects: 3, done.
Writing objects: 100% (3/3), 267 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/Hemu967/testGitHub.git
   bdcb43c..370a107  master -> master
Branch master set up to track remote branch master from origin.

yamini@yamini-PC MINGW64 ~/Desktop/testGitHub (master)
$ touch testfiles.txt

yamini@yamini-PC MINGW64 ~/Desktop/testGitHub (master)
$ ls
README.md  testfiles.txt

yamini@yamini-PC MINGW64 ~/Desktop/testGitHub (master)
$ vim testfiles

yamini@yamini-PC MINGW64 ~/Desktop/testGitHub (master)
$ git status
On branch master
Your branch is up-to-date with 'origin/master'.
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        testfiles
        testfiles.txt

nothing added to commit but untracked files present (use "git add" to track)

yamini@yamini-PC MINGW64 ~/Desktop/testGitHub (master)
$ git add .
warning: LF will be replaced by CRLF in testfiles.
The file will have its original line endings in your working directory.

yamini@yamini-PC MINGW64 ~/Desktop/testGitHub (master)
$ git commit -m "testfiles is added as a test:
> git commit -m "testfiles is added as a test"
>
> git commit -m "testfiles is added as a test:
git commit -m "testfiles is added as a test"
error: pathspec 'is' did not match any file(s) known to git.
error: pathspec 'added' did not match any file(s) known to git.
error: pathspec 'as' did not match any file(s) known to git.
error: pathspec 'a' did not match any file(s) known to git.
error: pathspec 'test

git commit -m testfiles' did not match any file(s) known to git.
error: pathspec 'is' did not match any file(s) known to git.
error: pathspec 'added' did not match any file(s) known to git.
error: pathspec 'as' did not match any file(s) known to git.
error: pathspec 'a' did not match any file(s) known to git.
error: pathspec 'test:' did not match any file(s) known to git.
[master 5a44383] testfiles is added as a test
 2 files changed, 1 insertion(+)
 create mode 100644 testfiles
 create mode 100644 testfiles.txt

yamini@yamini-PC MINGW64 ~/Desktop/testGitHub (master)
$ git commit -m "testfiles is added as test"
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)
nothing to commit, working tree clean

yamini@yamini-PC MINGW64 ~/Desktop/testGitHub (master)
$ git log
commit 5a44383a0cb5c865bbca634a54c253adb77c08cf
Author: Hemu967 <himanshutyagi967@gmail.com>
Date:   Fri Apr 7 23:37:00 2017 +0530

    testfiles is added as a test

commit 370a1072cd099ceaf4fe3197dca24e50b557daee
Author: Hemu967 <himanshutyagi967@gmail.com>
Date:   Fri Apr 7 21:09:51 2017 +0530

    update readme file for good

commit bdcb43c3308574af7cbbba16838cf43c1b3026a7
Author: Hemu967 <himanshutyagi967@gmail.com>
Date:   Fri Apr 7 20:49:17 2017 +0530

    Initial commit

yamini@yamini-PC MINGW64 ~/Desktop/testGitHub (master)
$ git status
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)
nothing to commit, working tree clean

yamini@yamini-PC MINGW64 ~/Desktop/testGitHub (master)
$ git push
Counting objects: 4, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 358 bytes | 0 bytes/s, done.
Total 4 (delta 0), reused 0 (delta 0)
To https://github.com/Hemu967/testGitHub.git
   370a107..5a44383  master -> master

yamini@yamini-PC MINGW64 ~/Desktop/testGitHub (master)
$ git pull origin master
From https://github.com/Hemu967/testGitHub
 * branch            master     -> FETCH_HEAD
Already up-to-date.

yamini@yamini-PC MINGW64 ~/Desktop/testGitHub (master)
$




























