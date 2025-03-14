This is simple fiel



### Below are the all the commands that we tried in VS code.


PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT> git --version
git version 2.48.1.windows.1
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT> git clone https://github.com/ravi-savalagi/git_complete_basics.git
Cloning into 'git_complete_basics'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (3/3), done.
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT> cd .\git_complete_basics\
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\git_complete_basics> ls


    Directory: C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\git_complete_basics


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a---l         3/14/2025  10:33 AM             21 README.md


PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\git_complete_basics> git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\git_complete_basics> git add .
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\git_complete_basics> git add .
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\git_complete_basics> git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md
        new file:   index.html

PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\git_complete_basics> git commit -m "add new para"
[main 992bbd9] add new para
 Committer: Savalagi <ravikumar.savalagi@accenture.com>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 2 files changed, 4 insertions(+), 1 deletion(-)
 create mode 100644 index.html
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\git_complete_basics> git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\git_complete_basics> git push origin main
info: please complete authentication in your browser...
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 374 bytes | 187.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/ravi-savalagi/git_complete_basics.git
   47ac29d..992bbd9  main -> main
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\git_complete_basics> cd ..
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT> mkdir LocalRepo


    Directory: C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----         3/14/2025  11:47 AM                LocalRepo


PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT> cd .\git_complete_basics\
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\git_complete_basics> cd ..             
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT> cd LocalRepo
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> ls -a
Get-ChildItem : Parameter cannot be processed because the parameter name 'a' is ambiguous. Possible matches include: 
-Attributes -Directory -File -Hidden -ReadOnly -System.
At line:1 char:4
+ ls -a
+    ~~
    + CategoryInfo          : InvalidArgument: (:) [Get-ChildItem], ParameterBindingException
    + FullyQualifiedErrorId : AmbiguousParameter,Microsoft.PowerShell.Commands.GetChildItemCommand

PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git init
Initialized empty Git repository in C:/Users/ravikumar.savalagi/OneDrive - Accenture/Desktop/GIT/LocalRepo/.git/
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> ls -a   
Get-ChildItem : Parameter cannot be processed because the parameter name 'a' is ambiguous. Possible matches include:      
-Attributes -Directory -File -Hidden -ReadOnly -System.
At line:1 char:4
+ ls -a
+    ~~
    + CategoryInfo          : InvalidArgument: (:) [Get-ChildItem], ParameterBindingException
    + FullyQualifiedErrorId : AmbiguousParameter,Microsoft.PowerShell.Commands.GetChildItemCommand

PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git add .
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   sample.html
        new file:   style.css

PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git commit -m "add initial files"
[main (root-commit) 3c90519] add initial files
 Committer: Savalagi <ravikumar.savalagi@accenture.com>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 2 files changed, 4 insertions(+)
 create mode 100644 sample.html
 create mode 100644 style.css
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git status
On branch main
nothing to commit, working tree clean
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git remote add origin https://github.com/ravi-savalagi/git_complete_basics_localrepo.git
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git remote -v
origin  https://github.com/ravi-savalagi/git_complete_basics_localrepo.git (fetch)
origin  https://github.com/ravi-savalagi/git_complete_basics_localrepo.git (push)
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git branch
* main
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git branch -M main
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git branch
* main
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git push -u origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 307 bytes | 307.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/ravi-savalagi/git_complete_basics_localrepo.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git add .
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git commit "Adding READM.md file"
error: pathspec 'Adding READM.md file' did not match any file(s) known to git
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git -m commit "Adding READM.md file"
unknown option: -m
usage: git [-v | --version] [-h | --help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--no-lazy-fetch]
           [--no-optional-locks] [--no-advice] [--bare] [--git-dir=<path>]
           [--work-tree=<path>] [--namespace=<name>] [--config-env=<name>=<envvar>]
           <command> [<args>]
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git commit -m  "Adding READM.md file"
[main 14d401e] Adding READM.md file
 Committer: Savalagi <ravikumar.savalagi@accenture.com>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
 create mode 100644 README.md
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 344 bytes | 344.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/ravi-savalagi/git_complete_basics_localrepo.git
   3c90519..14d401e  main -> main
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git branch
* main
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git checkout -b feature1
Switched to a new branch 'feature1'
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git branch
* feature1
  main
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git branch       
  feature1
* main
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git checkout feature1
Switched to branch 'feature1'
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git branch
* feature1
  main
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git checkout feature2
error: pathspec 'feature2' did not match any file(s) known to git
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git branch
* feature1
  main
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git checkout -b feature2
Switched to a new branch 'feature2'
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git branch
  feature1
* feature2
  main
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git branch -d feature2
error: cannot delete branch 'feature2' used by worktree at 'C:/Users/ravikumar.savalagi/OneDrive - Accenture/Desktop/GIT/LocalRepo'
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git checkout main       
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git branch
  feature1
  feature2
* main
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git branch -d feature2
Deleted branch feature2 (was 14d401e).
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git branch       
  feature1
* main
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git checkout feature1   
Switched to branch 'feature1'
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git branch
* feature1
  main
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git add .
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git status
On branch feature1
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   sample.html

PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git commit -m "Add new feature"
[feature1 581279b] Add new feature
 Committer: Savalagi <ravikumar.savalagi@accenture.com>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 2 insertions(+), 1 deletion(-)
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git status
On branch feature1
nothing to commit, working tree clean
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git checkout feature1
Switched to branch 'feature1'
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git branch
* feature1
  main
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git push origin feature1
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 367 bytes | 367.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'feature1' on GitHub by visiting:
remote:      https://github.com/ravi-savalagi/git_complete_basics_localrepo/pull/new/feature1
remote:
To https://github.com/ravi-savalagi/git_complete_basics_localrepo.git
 * [new branch]      feature1 -> feature1
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git branch
* feature1
  main
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git diff main
diff --git a/sample.html b/sample.html
index 1286de6..fff9ad5 100644
--- a/sample.html
+++ b/sample.html
@@ -1 +1,2 @@
-<p>Hello Developers</p>
\ No newline at end of file
+<p>Hello Developers</p>
+<p> This is new feature</p>
\ No newline at end of file
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git checkout main       
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git branch       
  feature1
* main
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git pull origin main
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (1/1), 898 bytes | 299.00 KiB/s, done.
From https://github.com/ravi-savalagi/git_complete_basics_localrepo
 * branch            main       -> FETCH_HEAD
   14d401e..e45f3c6  main       -> origin/main
Updating 14d401e..e45f3c6
Fast-forward
 sample.html | 3 ++-
 1 file changed, 2 insertions(+), 1 deletion(-)
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> 
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> 
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git add . 
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git commit -m "Add button"
[main 557070b] Add button
 Committer: Savalagi <ravikumar.savalagi@accenture.com>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+), 1 deletion(-)
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git checkout feature1
Switched to branch 'feature1'
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git branch
* feature1
  main
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git add .
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git commit -m "Add dropdown"
[feature1 0a5d862] Add dropdown
 Committer: Savalagi <ravikumar.savalagi@accenture.com>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+), 1 deletion(-)
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git diff main
diff --git a/sample.html b/sample.html
index eacf79f..da9b271 100644
--- a/sample.html
+++ b/sample.html
@@ -1,2 +1,2 @@
 <p>Hello Developers</p>
-<p> This is new feature (button) </p>
\ No newline at end of file
+<p> This is new feature (dropdown) </p>
\ No newline at end of file
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git merge main
Auto-merging sample.html
CONFLICT (content): Merge conflict in sample.html
Automatic merge failed; fix conflicts and then commit the result.
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git status
On branch feature1
You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   sample.html

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git add .
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git commit -m "Add both features"
[feature1 edcecbf] Add both features
 Committer: Savalagi <ravikumar.savalagi@accenture.com>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git status
On branch feature1
nothing to commit, working tree clean
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git diff main
diff --git a/sample.html b/sample.html
index eacf79f..05588e4 100644
--- a/sample.html
+++ b/sample.html
@@ -1,2 +1,3 @@
 <p>Hello Developers</p>
-<p> This is new feature (button) </p>
\ No newline at end of file
+<p> This is new feature (dropdown) </p>
+<p> This is new feature (button) </p>
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git branch
  feature1
* main
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git merge feature1
Updating 557070b..edcecbf
Fast-forward
 sample.html | 3 ++-
 1 file changed, 2 insertions(+), 1 deletion(-)
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> git push
Enumerating objects: 11, done.
Counting objects: 100% (11/11), done.
Delta compression using up to 12 threads
Compressing objects: 100% (9/9), done.
Writing objects: 100% (9/9), 1.02 KiB | 174.00 KiB/s, done.
Total 9 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/ravi-savalagi/git_complete_basics_localrepo.git
   e45f3c6..edcecbf  main -> main
PS C:\Users\ravikumar.savalagi\OneDrive - Accenture\Desktop\GIT\LocalRepo> 
