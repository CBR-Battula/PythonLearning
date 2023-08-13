# PythonLearning
This is Python learning practice series.
##intitial setup of git from local machine to github remote
C:\Users\brahm>cd Documents
C:\Users\brahm\Documents>mkdir Github_Repo
C:\Users\brahm\Documents>cd Github_Repo
C:\Users\brahm\Documents\Github_Repo>git clone https://github.com/CBR-Battula/PythonLearning.git
Cloning into 'PythonLearning'...
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 6 (delta 0), reused 3 (delta 0), pack-reused 0
Receiving objects: 100% (6/6), done.

C:\Users\brahm\Documents\Github_Repo>git
usage: git [-v | --version] [-h | --help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           [--config-env=<name>=<envvar>] <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone     Clone a repository into a new directory
   init      Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add       Add file contents to the index
   mv        Move or rename a file, a directory, or a symlink
   restore   Restore working tree files
   rm        Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
   bisect    Use binary search to find the commit that introduced a bug
   diff      Show changes between commits, commit and working tree, etc
   grep      Print lines matching a pattern
   log       Show commit logs
   show      Show various types of objects
   status    Show the working tree status

grow, mark and tweak your common history
   branch    List, create, or delete branches
   commit    Record changes to the repository
   merge     Join two or more development histories together
   rebase    Reapply commits on top of another base tip
   reset     Reset current HEAD to the specified state
   switch    Switch branches
   tag       Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch     Download objects and refs from another repository
   pull      Fetch from and integrate with another repository or a local branch
   push      Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
See 'git help git' for an overview of the system.

C:\Users\brahm\Documents\Github_Repo>git init
Initialized empty Git repository in C:/Users/brahm/Documents/Github_Repo/.git/

C:\Users\brahm\Documents\Github_Repo>git --version
git version 2.41.0.windows.3

C:\Users\brahm\Documents\Github_Repo>git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        PythonLearning/

nothing added to commit but untracked files present (use "git add" to track)
## create file PythonLearning/HelloWorld.py and some text into it

C:\Users\brahm\Documents\Github_Repo>git add PythonLearning/HelloWorld.py

C:\Users\brahm\Documents\Github_Repo>git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        PythonLearning/

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\brahm\Documents\Github_Repo\PythonLearning>git add HelloWorld.py

C:\Users\brahm\Documents\Github_Repo\PythonLearning>git commit -m "HelloWorld"
[main e94550a] HelloWorld
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 HelloWorld.py
### Run the below command if not link ur remote rep with local repo
C:\Users\brahm\Documents\Github_Repo\PythonLearning>git remote add origin https://github.com/CBR-Battula/PythonLearning.git
error: remote origin already exists.

C:\Users\brahm\Documents\Github_Repo\PythonLearning>git push origin master
error: src refspec master does not match any
error: failed to push some refs to 'https://github.com/CBR-Battula/PythonLearning.git'

C:\Users\brahm\Documents\Github_Repo\PythonLearning>git push origin
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 283 bytes | 283.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/CBR-Battula/PythonLearning.git
   eb40167..e94550a  main -> main

C:\Users\brahm\Documents\Github_Repo\PythonLearning>git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

C:\Users\brahm\Documents\Github_Repo\PythonLearning>

## Go and check in the report github repository for the file.

# you can run the commands in vs code via integrated terminal
right click on the file in vs code and choose "open in integrated terminal"
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> ls


    Directory: C:\Users\brahm\Documents\Github_Repo\PythonLearning


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        11-08-2023     11:41              0 HelloWorld.py
-a----        11-08-2023     11:58           5154 README.md


PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   HelloWorld.py

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git add HelloWorld.py
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git commit -m "simple addition program"
[main b34e47e] simple addition program
 1 file changed, 5 insertions(+)
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git push origin
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 378 bytes | 378.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/CBR-Battula/PythonLearning.git
   8ddcdfe..b34e47e  main -> main
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning>

## create a new branch
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch
* main
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch -c New_PythonLearning
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch
  New_PythonLearning
* main
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git checkout New_PythonLearning
Switched to branch 'New_PythonLearning'
Your branch is up to date with 'origin/main'.
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch
* New_PythonLearning
  main

PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch
  New_PythonLearning
* main
PS C:\Users\brahm\Documents\Github_Repo> git clone https://github.com/CBR-Battula/PythonLearning.git
Cloning into 'PythonLearning'...
remote: Enumerating objects: 21, done.
remote: Counting objects: 100% (21/21), done.
remote: Compressing objects: 100% (15/15), done.
remote: Total 21 (delta 2), reused 18 (delta 2), pack-reused 0
Receiving objects: 100% (21/21), 5.42 KiB | 1.81 MiB/s, done.
Resolving deltas: 100% (2/2), done.
PS C:\Users\brahm\Documents\Github_Repo> 


#### go to Respository "PythonLearning"
 C:\Users\brahm\Documents\Github_Repo> cd .\PythonLearning\
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning>
## list the branches , * indicates the current active branch and we switch the branch by checkout
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch
* main
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch -c NewPythonLeaning
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch
  NewPythonLeaning
* main
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git checkout NewPythonLearning
error: pathspec 'NewPythonLearning' did not match any file(s) known to git
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git checkout NewPythonLeaning
Switched to branch 'NewPythonLeaning'
Your branch is up to date with 'origin/main'.
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch
* NewPythonLeaning
  main


PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git add .                
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git commit -m "new branch creation"
[NewPythonLeaning ed190b3] new branch creation
 1 file changed, 1 insertion(+)
 create mode 100644 PythonLearning/HelloPython.py
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git push origin HEAD
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 425 bytes | 212.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'NewPythonLeaning' on GitHub by visiting:
remote:      https://github.com/CBR-Battula/PythonLearning/pull/new/NewPythonLeaning
remote:
To https://github.com/CBR-Battula/PythonLearning.git
 * [new branch]      HEAD -> NewPythonLeaning

PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git pull
Already up to date.
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch
* NewPythonLeaning
  main
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git add .
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git commit -m "trying again and again"
[NewPythonLeaning ad5c494] trying again and again
 1 file changed, 1 insertion(+), 1 deletion(-)
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git push origin HEAD
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 12 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (8/8), 820 bytes | 273.00 KiB/s, done.
Total 8 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'NewPythonLeaning' on GitHub by visiting:
remote:      https://github.com/CBR-Battula/PythonLearning/pull/new/NewPythonLeaning
remote:
To https://github.com/CBR-Battula/PythonLearning.git
 * [new branch]      HEAD -> NewPythonLeaning
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git status
On branch NewPythonLeaning
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch
* NewPythonLeaning
  main
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (1/1), 631 bytes | 126.00 KiB/s, done.
From https://github.com/CBR-Battula/PythonLearning
   0f0fcf9..65a2a7f  main       -> origin/main
Updating ad5c494..65a2a7f
Fast-forward
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch
* NewPythonLeaning
  main
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git checkout main
Switched to branch 'main'
Your branch is behind 'origin/main' by 3 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git pull
Updating 0f0fcf9..65a2a7f
Fast-forward
 PythonLearning/HelloPython.py | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 PythonLearning/HelloPython.py
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch
  NewPythonLeaning
* main
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch -a
  NewPythonLeaning
* main
  remotes/origin/HEAD -> origin/main
  remotes/origin/NewPythonLeaning
  remotes/origin/New_PythonLearning
  remotes/origin/main
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git remote prune origin
Pruning origin
URL: https://github.com/CBR-Battula/PythonLearning.git
 * [pruned] origin/NewPythonLeaning
 * [pruned] origin/New_PythonLearning
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch
  NewPythonLeaning
* main
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch –D NewPythonLeaning
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch
  NewPythonLeaning
* main
  –D
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> gut pull -p
gut : The term 'gut' is not recognized as the name of a cmdlet, function, script file, or operable program. Check the spelling of the name, or if a path was included, verify that the path is 
correct and try again.
At line:1 char:1
+ gut pull -p
+ ~~~
    + CategoryInfo          : ObjectNotFound: (gut:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException

PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git pull -p
Already up to date.
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch
  NewPythonLeaning
* main
  –D
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch -r
  origin/HEAD -> origin/main
  origin/main
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch -a
  NewPythonLeaning
* main
  –D
  remotes/origin/HEAD -> origin/main
  remotes/origin/main
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch -d NewPythonLeaning 
Deleted branch NewPythonLeaning (was 65a2a7f).
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch
* main
  –D
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch -d –D
Deleted branch –D (was 65a2a7f).
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch
* main
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> cd ..
PS C:\Users\brahm\Documents\Github_Repo> git pull
There is no tracking information for the current branch.













PS C:\Users\brahm\Documents\Github_Repo> git clone https://github.com/CBR-Battula/PythonLearning.git
Cloning into 'PythonLearning'...
remote: Enumerating objects: 27, done.
remote: Counting objects: 100% (27/27), done.
remote: Compressing objects: 100% (18/18), done.
remote: Total 27 (delta 1), reused 23 (delta 1), pack-reused 0
Receiving objects: 100% (27/27), 5.90 KiB | 1.97 MiB/s, done.
Resolving deltas: 100% (1/1), done.
PS C:\Users\brahm\Documents\Github_Repo> cd .\PythonLearning\
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git rm -r PythonLearning
rm 'PythonLearning/HelloPython.py'
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git commit
[main ecc2a65] ere
 1 file changed, 1 deletion(-)
 delete mode 100644 PythonLearning/HelloPython.py
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git push origin
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 267 bytes | 267.00 KiB/s, done.
Total 2 (delta 0), reused 1 (delta 0), pack-reused 0
To https://github.com/CBR-Battula/PythonLearning.git
   65a2a7f..ecc2a65  main -> main
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch
* main
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch -c NewPythonLearning
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch
  NewPythonLearning
* main
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git checkout NewPythonLearning
Switched to branch 'NewPythonLearning'
Your branch is up to date with 'origin/main'.
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch
* NewPythonLearning
  main
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git status
On branch NewPythonLearning
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        NewHelloWorld.py

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git add NewHelloWorld.py
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git commit -m "newfile in new branch"
[NewPythonLearning 38fee50] newfile in new branch
 1 file changed, 1 insertion(+)
 create mode 100644 NewHelloWorld.py
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git push origin HEAD
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 362 bytes | 181.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'NewPythonLearning' on GitHub by visiting:
remote:      https://github.com/CBR-Battula/PythonLearning/pull/new/NewPythonLearning
remote:
To https://github.com/CBR-Battula/PythonLearning.git
 * [new branch]      HEAD -> NewPythonLearning
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch
* NewPythonLearning
  main
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch -a
* NewPythonLearning
  main
  remotes/origin/HEAD -> origin/main
  remotes/origin/NewPythonLearning
  remotes/origin/main
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> cd ..
PS C:\Users\brahm\Documents\Github_Repo> git pull
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=<remote>/<branch> main

PS C:\Users\brahm\Documents\Github_Repo> cd PythonLearning
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (1/1), 636 bytes | 127.00 KiB/s, done.
From https://github.com/CBR-Battula/PythonLearning
   ecc2a65..7c78f4f  main       -> origin/main
Updating 38fee50..7c78f4f
Fast-forward
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch -a
* NewPythonLearning
  main
  remotes/origin/HEAD -> origin/main
  remotes/origin/NewPythonLearning
  remotes/origin/main
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch -d NewPythonLearning
error: Cannot delete branch 'NewPythonLearning' checked out at 'C:/Users/brahm/Documents/Github_Repo/PythonLearning'
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git checkout main
Switched to branch 'main'
Your branch is behind 'origin/main' by 2 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch -d NewPythonLearning
warning: deleting branch 'NewPythonLearning' that has been merged to
         'refs/remotes/origin/main', but not yet merged to HEAD.
Deleted branch NewPythonLearning (was 7c78f4f).
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git branch
* main
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning> git pull
Updating ecc2a65..7c78f4f
Fast-forward
 NewHelloWorld.py | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 NewHelloWorld.py
PS C:\Users\brahm\Documents\Github_Repo\PythonLearning>