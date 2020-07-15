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
  
#PROBLEM 6: run command without any output 

  open terminal and type any command 
  once you press enter your output of given command must not  print
  you are not allowed to redirect output anywhere 
  
 Solution:
 $ bash -n
 
#PROBLEM 7:  create a shell script 

create a shell script named /root/delvex.sh 
make sure it will run /bin/sh shell 
a user will be running this script my using a command name opensource
when a user  run like  "opensource  time" it must give current time only
when it runs like "opensource user"  it will give list of interactive shell users only
when run like "opensource 100"  it must print "Hello Delvex" 100 times in interval of 1 sec
if runs like  "opensource windows"  then it must shutdown OS
if run opensource command without any parameter  then it must show out --
             i)   name of kernel 
             ii)   version of kernel 
             iii)  current date in the format of  /DD/MM/YY
             iv)  name of OS 
             v)   last reboot time 
             
Solution:
#!/bin/sh 

if  [ $1 == "time"  ]
then
                echo "$(date +%T)"
elif  [ $1 == "user"  ]
then
                echo "$(cat /etc/passwd)"
elif  [ $1 == "100"  ]
then
for i in 1 2 3 4 5
do
        echo "Hello Delvex"
        sleep 1
done
elif  [ $1 == "windows"  ]
then
                echo "$(shutdown -P now)"
elif  [ $1 ==   ]
then
                echo "$(uname -s)\n"
                echo "$(uname -v)\n"
                echo "$(date +'%d/%m/%Y')\n"
                echo "$(uname -o)\n"
                echo "$(who -b)\n"
else
       echo "command not found"
fi



