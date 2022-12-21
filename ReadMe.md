andre@TALUS MINGW64 /e/Documents/Scripts/QA
$ mkdir RepoRepo

andre@TALUS MINGW64 /e/Documents/Scripts/QA
$ cd RepoRepo/

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo
$ >> ReadMe.md

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo
$ ls
ReadMe.md

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo
$ git init
Initialized empty Git repository in E:/Documents/Scripts/QA/RepoRepo/.git/

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (master)
$ git add ReadMe.md

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   ReadMe.md


andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (master)
$ git commit -m "First commit"
[master (root-commit) 62074ca] First commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 ReadMe.md

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (master)
$ git branch -m main

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (main)
$ git remote add origin https://github.com/Andrew-McCall/RepoRepo

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 213 bytes | 213.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Andrew-McCall/RepoRepo
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (main)
$ cd ..

andre@TALUS MINGW64 /e/Documents/Scripts/QA
$ rm -rfv RepoRepo
removed 'RepoRepo/.git/COMMIT_EDITMSG'
removed 'RepoRepo/.git/config'
removed 'RepoRepo/.git/description'
removed 'RepoRepo/.git/HEAD'
removed 'RepoRepo/.git/hooks/applypatch-msg.sample'
removed 'RepoRepo/.git/hooks/commit-msg.sample'
removed 'RepoRepo/.git/hooks/fsmonitor-watchman.sample'
removed 'RepoRepo/.git/hooks/post-update.sample'
removed 'RepoRepo/.git/hooks/pre-applypatch.sample'
removed 'RepoRepo/.git/hooks/pre-commit.sample'
removed 'RepoRepo/.git/hooks/pre-merge-commit.sample'
removed 'RepoRepo/.git/hooks/pre-push.sample'
removed 'RepoRepo/.git/hooks/pre-rebase.sample'
removed 'RepoRepo/.git/hooks/pre-receive.sample'
removed 'RepoRepo/.git/hooks/prepare-commit-msg.sample'
removed 'RepoRepo/.git/hooks/push-to-checkout.sample'
removed 'RepoRepo/.git/hooks/update.sample'
removed directory 'RepoRepo/.git/hooks'
removed 'RepoRepo/.git/index'
removed 'RepoRepo/.git/info/exclude'
removed directory 'RepoRepo/.git/info'
removed 'RepoRepo/.git/logs/HEAD'
removed 'RepoRepo/.git/logs/refs/heads/main'
removed directory 'RepoRepo/.git/logs/refs/heads'
removed 'RepoRepo/.git/logs/refs/remotes/origin/main'
removed directory 'RepoRepo/.git/logs/refs/remotes/origin'
removed directory 'RepoRepo/.git/logs/refs/remotes'
removed directory 'RepoRepo/.git/logs/refs'
removed directory 'RepoRepo/.git/logs'
removed 'RepoRepo/.git/objects/52/fe1ba4ac2b979c0a8fbeb9f87c1b1c9f177520'
removed directory 'RepoRepo/.git/objects/52'
removed 'RepoRepo/.git/objects/62/074ca6bb470569571e1849ad7fde2d9e1eac8c'
removed directory 'RepoRepo/.git/objects/62'
removed 'RepoRepo/.git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391'
removed directory 'RepoRepo/.git/objects/e6'
removed directory 'RepoRepo/.git/objects/info'
removed directory 'RepoRepo/.git/objects/pack'
removed directory 'RepoRepo/.git/objects'
removed 'RepoRepo/.git/refs/heads/main'
removed directory 'RepoRepo/.git/refs/heads'
removed 'RepoRepo/.git/refs/remotes/origin/main'
removed directory 'RepoRepo/.git/refs/remotes/origin'
removed directory 'RepoRepo/.git/refs/remotes'
removed directory 'RepoRepo/.git/refs/tags'
removed directory 'RepoRepo/.git/refs'
removed directory 'RepoRepo/.git'
removed 'RepoRepo/ReadMe.md'
removed directory 'RepoRepo'

andre@TALUS MINGW64 /e/Documents/Scripts/QA
$ git clone https://github.com/Andrew-McCall/RepoRepo
Cloning into 'RepoRepo'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 3 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.

andre@TALUS MINGW64 /e/Documents/Scripts/QA
$ cd RepoRepo

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (main)
$ ls
ReadMe.md

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (main)
$ git branch ChangeOne

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (main)
$ git checkout ChangeOne
Switched to branch 'ChangeOne'

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (ChangeOne)
$ nano ReadMe.md

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (ChangeOne)
$ git add ReadMe.md
warning: in the working copy of 'ReadMe.md', LF will be replaced by CRLF the next time Git touches it

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (ChangeOne)
$ git commit -m "ReadMe"
[ChangeOne 5be7bd4] ReadMe
 1 file changed, 1 insertion(+)
g
andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (ChangeOne)
$ git push -u origin ChangeOne
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Writing objects: 100% (3/3), 247 bytes | 247.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'ChangeOne' on GitHub by visiting:
remote:      https://github.com/Andrew-McCall/RepoRepo/pull/new/ChangeOne
remote:
To https://github.com/Andrew-McCall/RepoRepo
 * [new branch]      ChangeOne -> ChangeOne
branch 'ChangeOne' set up to track 'origin/ChangeOne'.

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (ChangeOne)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (main)
$ git branch ChangeTwo

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (main)
$ git checkout ChangeTwo
Switched to branch 'ChangeTwo'

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (ChangeTwo)
$ notepad ReadMe.md

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (ChangeTwo)
$ git add ReadMe.md

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (ChangeTwo)
$ git commit -m "Change Two"
[ChangeTwo 9184bfc] Change Two
 1 file changed, 1 insertion(+)
g
andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (ChangeTwo)
$ git push -u origin ChangeTwo
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Writing objects: 100% (3/3), 252 bytes | 252.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'ChangeTwo' on GitHub by visiting:
remote:      https://github.com/Andrew-McCall/RepoRepo/pull/new/ChangeTwo
remote:
To https://github.com/Andrew-McCall/RepoRepo
 * [new branch]      ChangeTwo -> ChangeTwo
branch 'ChangeTwo' set up to track 'origin/ChangeTwo'.

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (ChangeTwo)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (main)
$ git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (1/1), 623 bytes | 11.00 KiB/s, done.
From https://github.com/Andrew-McCall/RepoRepo
   62074ca..c1cfcc8  main       -> origin/main
Updating 62074ca..c1cfcc8
Fast-forward
 ReadMe.md | 1 +
 1 file changed, 1 insertion(+)

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (main)
$ git merge ChangeTwo
Auto-merging ReadMe.md
CONFLICT (content): Merge conflict in ReadMe.md
Automatic merge failed; fix conflicts and then commit the result.

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (main|MERGING)
$ notepad ReadMe.md

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (main|MERGING)
$ git add ReadMe.md

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (main|MERGING)
$ git commit -m "Fixed conflict"
[main 4562c39] Fixed conflict

andre@TALUS MINGW64 /e/Documents/Scripts/QA/RepoRepo (main)
$ git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Writing objects: 100% (3/3), 289 bytes | 289.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Andrew-McCall/RepoRepo
   c1cfcc8..4562c39  main -> main
