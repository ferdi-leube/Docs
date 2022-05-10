leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack
$ ls
CV/  Ironferdi/  Ironlab/      file.txt   ironNatan/  test3/
DA/  Ironhack    Lab1Felicia/  file1.txt  test/

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack
$ cd Ironferdi

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/Ironferdi (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/Ironferdi (main)
$ ls
about.txt

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/Ironferdi (main)
$ git pull origin main
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 4 (delta 0), reused 3 (delta 0), pack-reused 0
Unpacking objects: 100% (4/4), 951 bytes | 59.00 KiB/s, done.
From https://github.com/ferdi-leube/Ironferdi
 * branch            main       -> FETCH_HEAD
   dde4508..3a27adc  main       -> origin/main
Updating dde4508..3a27adc
Fast-forward
 felicia.txt | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 felicia.txt

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/Ironferdi (main)
$ ls
about.txt  felicia.txt

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/Ironferdi (main)
$ echo "I am 18 years old" >> about.txt

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/Ironferdi (main)
$ git add .
warning: LF will be replaced by CRLF in about.txt.
The file will have its original line endings in your working directory

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/Ironferdi (main)
$ git commit -m "change for conflict
>
>
>
>
>
> "
[main 55fe243] change for conflict
 1 file changed, 1 insertion(+)

...skipping...
commit 55fe2438a6124050a9a301945a9f62c00641c2d2 (HEAD -> main, origin/main)
Author: Ferdinand Leube <leubeb@gmail.com>nferdi.git (fetch)
Date:   Tue May 10 09:05:44 2022 +0200/Ironferdi.git (push)

    change for conflictINGW64 ~/Ironhack/Ironferdi (main)
$ git push -u origin main
commit 3a27adc197f683cb770d75cc592a2b4483e8d72a
Merge: dde4508 4cbe622 (5/5), done.
Author: ferdi-leube <102727928+ferdi-leube@users.noreply.github.com>
Date:   Mon May 9 15:44:58 2022 +0200.
Writing objects: 100% (3/3), 348 bytes | 348.00 KiB/s, done.
    Merge pull request #1 from Leecia-2864/classmate
    ttps://github.com/ferdi-leube/Ironferdi.git
    my new branch43  main -> main
branch 'main' set up to track 'origin/main'.
commit 4cbe62274f9d67b0cea079af7d5ec2c2d354bb98
Author: [Felicia] <[feliciaonwudinjo@gmail.com]>di (main)
Date:   Mon May 9 14:39:39 2022 +0100
commit 55fe2438a6124050a9a301945a9f62c00641c2d2 (HEAD -> main, origin/main)
    my new branch Leube <leubeb@gmail.com>
Date:   Tue May 10 09:05:44 2022 +0200
commit dde4508d7e3ffb35c625945c1fe50048ba4b9b98 (HEAD -> main, origin/main)
Author: Ferdinand Leube <leubeb@gmail.com>
Date:   Mon May 9 14:19:56 2022 +02000

    Lab1 file with fun fact
~
~ommit 3a27adc197f683cb770d75cc592a2b4483e8d72a
~erge: dde4508 4cbe622
~uthor: ferdi-leube <102727928+ferdi-leube@users.noreply.github.com>
~ate:   Mon May 9 15:44:58 2022 +0200
~
~   Merge pull request #1 from Leecia-2864/classmate
~
~   my new branch
~
~ommit 4cbe62274f9d67b0cea079af7d5ec2c2d354bb98
~uthor: [Felicia] <[feliciaonwudinjo@gmail.com]>
~ate:   Mon May 9 14:39:39 2022 +0100
~
~   my new branch
~
~ommit dde4508d7e3ffb35c625945c1fe50048ba4b9b98
~uthor: Ferdinand Leube <leubeb@gmail.com>
~o next tag  (press RETURN)
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
...skipping...
commit 55fe2438a6124050a9a301945a9f62c00641c2d2 (HEAD -> main, origin/main)
Author: Ferdinand Leube <leubeb@gmail.com>
Date:   Tue May 10 09:05:44 2022 +0200

    change for conflict

commit 3a27adc197f683cb770d75cc592a2b4483e8d72a
Merge: dde4508 4cbe622
Author: ferdi-leube <102727928+ferdi-leube@users.noreply.github.com>
Date:   Mon May 9 15:44:58 2022 +0200

    Merge pull request #1 from Leecia-2864/classmate

    my new branch

commit 4cbe62274f9d67b0cea079af7d5ec2c2d354bb98
Author: [Felicia] <[feliciaonwudinjo@gmail.com]>
Date:   Mon May 9 14:39:39 2022 +0100

    my new branch

commit dde4508d7e3ffb35c625945c1fe50048ba4b9b98
Author: Ferdinand Leube <leubeb@gmail.com>
Date:   Mon May 9 14:19:56 2022 +0200

    Lab1 file with fun fact
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~
~

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/Ironferdi (main)
$ git reset --hard dde4508d7e3ffb35c625945c1fe50048ba4b9b98
HEAD is now at dde4508 Lab1 file with fun fact

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/Ironferdi (main)
$ git checkout -b lab-resolving-git-conflicts
Switched to a new branch 'lab-resolving-git-conflicts'

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/Ironferdi (lab-resolving-git-conflicts)
$ ls
about.txt

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/Ironferdi (lab-resolving-git-conflicts)
$ git add .

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/Ironferdi (lab-resolving-git-conflicts)
$ git commit -m "try to merge for conflict"
[lab-resolving-git-conflicts d8b882d] try to merge for conflict
 1 file changed, 16 insertions(+), 1 deletion(-)
 rewrite about.txt (100%)

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/Ironferdi (lab-resolving-git-conflicts)
$ git remote -v
origin  https://github.com/ferdi-leube/Ironferdi.git (fetch)
origin  https://github.com/ferdi-leube/Ironferdi.git (push)

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/Ironferdi (lab-resolving-git-conflicts)
$ git pull origin master
fatal: couldn't find remote ref master

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/Ironferdi (lab-resolving-git-conflicts)
$ git pull origin lab-resolving-git-conflicts
fatal: couldn't find remote ref lab-resolving-git-conflicts

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/Ironferdi (lab-resolving-git-conflicts)
$ git pull origin main
From https://github.com/ferdi-leube/Ironferdi
 * branch            main       -> FETCH_HEAD
Auto-merging about.txt
CONFLICT (content): Merge conflict in about.txt
Automatic merge failed; fix conflicts and then commit the result.

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/Ironferdi (lab-resolving-git-conflicts|MERGING)
$ git status
On branch lab-resolving-git-conflicts
You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Changes to be committed:
        new file:   felicia.txt

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   about.txt


leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/Ironferdi (lab-resolving-git-conflicts|MERGING)
$ git status
On branch lab-resolving-git-conflicts
You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Changes to be committed:
        new file:   felicia.txt

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   about.txt


leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/Ironferdi (lab-resolving-git-conflicts|MERGING)
$ git add .

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/Ironferdi (lab-resolving-git-conflicts|MERGING)
$ git commit -m "fixed files"
[lab-resolving-git-conflicts 350375a] fixed files

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/Ironferdi (lab-resolving-git-conflicts)
$ git remote -v
origin  https://github.com/ferdi-leube/Ironferdi.git (fetch)
origin  https://github.com/ferdi-leube/Ironferdi.git (push)

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/Ironferdi (lab-resolving-git-conflicts)
$ git push -u origin lab-resolving-git-conflicts
Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 8 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (6/6), 883 bytes | 441.00 KiB/s, done.
Total 6 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'lab-resolving-git-conflicts' on GitHub by visiting:
remote:      https://github.com/ferdi-leube/Ironferdi/pull/new/lab-resolving-git-conflicts
remote:
To https://github.com/ferdi-leube/Ironferdi.git
 * [new branch]      lab-resolving-git-conflicts -> lab-resolving-git-conflicts
branch 'lab-resolving-git-conflicts' set up to track 'origin/lab-resolving-git-conflicts'.
