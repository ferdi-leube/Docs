leube@LAPTOP-3UCS3K18 MINGW64 ~
$ mkdir git-merge-testing

leube@LAPTOP-3UCS3K18 MINGW64 ~
$ cd git-merge-testing

leube@LAPTOP-3UCS3K18 MINGW64 ~/git-merge-testing
$ git init .
Initialized empty Git repository in C:/Users/leube/git-merge-testing/.git/

leube@LAPTOP-3UCS3K18 MINGW64 ~/git-merge-testing (master)
$ echo "this is some content to work with" > merging.txt

leube@LAPTOP-3UCS3K18 MINGW64 ~/git-merge-testing (master)
$ git add merging.txt
warning: LF will be replaced by CRLF in merging.txt.
The file will have its original line endings in your working directory

leube@LAPTOP-3UCS3K18 MINGW64 ~/git-merge-testing (master)
$ git commit -m "initial content"
[master (root-commit) 70f8665] initial content
 1 file changed, 1 insertion(+)
 create mode 100644 merging.txt

leube@LAPTOP-3UCS3K18 MINGW64 ~/git-merge-testing (master)
$ git checkout -b new_branch_to_merge_later
Switched to a new branch 'new_branch_to_merge_later'

leube@LAPTOP-3UCS3K18 MINGW64 ~/git-merge-testing (new_branch_to_merge_later)
$ echo "totally different content to merge later" > merging.txt

leube@LAPTOP-3UCS3K18 MINGW64 ~/git-merge-testing (new_branch_to_merge_later)
$ git commit -m "edited the content of merging.txt to cause a conflict"
On branch new_branch_to_merge_later
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   merging.txt

no changes added to commit (use "git add" and/or "git commit -a")

leube@LAPTOP-3UCS3K18 MINGW64 ~/git-merge-testing (new_branch_to_merge_later)
$ git commit -am "edited the content of merging.txt to cause a conflict"
warning: LF will be replaced by CRLF in merging.txt.
The file will have its original line endings in your working directory
[new_branch_to_merge_later 2cb5a34] edited the content of merging.txt to cause a conflict
 1 file changed, 1 insertion(+), 1 deletion(-)

leube@LAPTOP-3UCS3K18 MINGW64 ~/git-merge-testing (new_branch_to_merge_later)
$ git checkout -b master
fatal: a branch named 'master' already exists

leube@LAPTOP-3UCS3K18 MINGW64 ~/git-merge-testing (new_branch_to_merge_later)
$ git checkout master
Switched to branch 'master'

leube@LAPTOP-3UCS3K18 MINGW64 ~/git-merge-testing (master)
$ echo "content to append" >>  merging.txt

leube@LAPTOP-3UCS3K18 MINGW64 ~/git-merge-testing (master)
$ git commit -am "append content to merging.txt"
warning: LF will be replaced by CRLF in merging.txt.
The file will have its original line endings in your working directory
[master 489453c] append content to merging.txt
 1 file changed, 1 insertion(+)

leube@LAPTOP-3UCS3K18 MINGW64 ~/git-merge-testing (master)
$ git merge new_branch_to_merge_later
Auto-merging merging.txt
CONFLICT (content): Merge conflict in merging.txt
Automatic merge failed; fix conflicts and then commit the result.

leube@LAPTOP-3UCS3K18 MINGW64 ~/git-merge-testing (master|MERGING)
$ git status
On branch master
You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   merging.txt

no changes added to commit (use "git add" and/or "git commit -a")

leube@LAPTOP-3UCS3K18 MINGW64 ~/git-merge-testing (master|MERGING)
$ cat merging.txt
<<<<<<< HEAD
this is some content to work with
content to append
=======
totally different content to merge later
>>>>>>> new_branch_to_merge_later

leube@LAPTOP-3UCS3K18 MINGW64 ~/git-merge-testing (master|MERGING)
$ cat merging.txt
<<<<<<< HEAD

content to append
=======
totally different content to merge later
>>>>>>> new_branch_to_merge_later

leube@LAPTOP-3UCS3K18 MINGW64 ~/git-merge-testing (master|MERGING)
$ cat merging.txt
content to append
totally different content to merge later


leube@LAPTOP-3UCS3K18 MINGW64 ~/git-merge-testing (master|MERGING)
$ git add merging.txt

leube@LAPTOP-3UCS3K18 MINGW64 ~/git-merge-testing (master|MERGING)
$ git commit -m "final file"
[master 9c89d94] final file

leube@LAPTOP-3UCS3K18 MINGW64 ~/git-merge-testing (master)
$
