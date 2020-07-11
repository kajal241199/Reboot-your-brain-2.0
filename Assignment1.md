#SOLUTIONS OF:
#PROBLEM 1:



#PROBLEM 2: create a directory without name from command line
            create a directory with name "-okgoogle"
Solution:
> a)mkdir ' '
> b)mkdir -- -okgoogle or mkdir ./-okgoogle


#PROBLEM 3: create a directory structure :
You are only allowed to use a single command and only one time
Solution: mkdir -p a/{b/{g/k/reboot.txt,h/k/reboot.txt},c/{i/j/reboot.txt,j/l/reboot.txt},d/{f/l/reboot.txt,e/m/reboot.txt}}

#PROBLEM 4:

#PROBLEM 5:
  create  3 files named   abc.txt  ok  fine  g.txt  /tmp directory 
  create  4  directories   aa aaa aaaa  under  /tmp directory 
  give ls command to  list the content of  /tmp directory 
  make sure it will only list the content (file|directory)  having 2 char in their name.
Solution:
1.go to tmp directory
2.creating files 
  touch abc.txt  ok\ fine  g.txt
3.creating directories
  mkdir aa aaa aaaa aaaaa
4.ls -f ??    #list the files with 2 chars
  ls -d ??    #list the directories with 2 chars
