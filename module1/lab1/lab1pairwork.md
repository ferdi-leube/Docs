leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack
$ git clone https://github.com/ferdi-leube/ironNatan.git
Cloning into 'ironNatan'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 3 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack
$ ls
CV/  Ironferdi/  Ironlab/      file.txt   ironNatan/  test3/
DA/  Ironhack    Lab1Felicia/  file1.txt  test/

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack
$ cd ironNatan

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/ironNatan (main)
$ git checkout -b classmate
Switched to a new branch 'classmate'

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/ironNatan (classmate)
$ touch ferdi2.txt

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/ironNatan (classmate)
$ echo "I participate in the bootcamp in order to recieve a good foundation for my economics and computer science studies" >> ferdi2.txt

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/ironNatan (classmate)
$ git add ferdi2.txt
warning: LF will be replaced by CRLF in ferdi2.txt.
The file will have its original line endings in your working directory

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/ironNatan (classmate)
$ git commit -m "Lab1 pair work"
[classmate 8c2da32] Lab1 pair work
 1 file changed, 1 insertion(+)
 create mode 100644 ferdi2.txt

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/ironNatan (classmate)
$ git remote -v
origin  https://github.com/ferdi-leube/ironNatan.git (fetch)
origin  https://github.com/ferdi-leube/ironNatan.git (push)

leube@LAPTOP-3UCS3K18 MINGW64 ~/Ironhack/ironNatan (classmate)
$ git push -u origin classmate
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 369 bytes | 369.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/ferdi-leube/ironNatan.git
   3f839b1..8c2da32  classmate -> classmate
branch 'classmate' set up to track 'origin/classmate'.
