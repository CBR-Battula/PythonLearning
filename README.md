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
