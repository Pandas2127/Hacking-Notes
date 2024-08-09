# LINUX FOR USER🤓
### Over View Of Kali Linux
##### Specifically i will going to show you with kali linux with gnome but you can have any kinda but Debian is recommended.
##### Previously known as Backtrack.
## Kali Linux Menu
#### 1.Information Gathering
##### Is Tools for information gathering in system network host.
#### 2.Vulnerability Analysis
##### Is Tools for finding vulnerabilities.
#### 3.Web Application Analysis
##### Is Tools for finding vulnerabilities and exploits on websites.
#### 4,Data Base Assessment
##### Is Tools for finding vulnerabilities and exploits on Data bases.
#### 5,Password Attacks
##### Tools for exploiting Passwords for login,websites,application, windows.
#### 6,Wireless Attacks
##### Tools for exploiting Wireless Systems like wifi, bluetooth.
#### 7.Reverse Engineering
##### Tools for exploiting Softwares , Mobile Applications and any binary files.
#### 8) Exploitation Tools
##### Tools for exploiting Softwares, Mobile ,Computers ,websites and any things.
#### 9) Sniffing & Spoofing
##### Tools for Listening or hijacking networks.
#### 10) POST exploitation
##### Tools for Maintaining our access. Used after exploiting a system.
#### 11) Forensics
##### Tools for Doing researches and investigate a Cyber Attacks.
#### 12) Reporting tools
##### Tools for Report preparation. After some forensic you will get data and you will write report and these tools will help you.
#### 13) Social Engineering tools
##### Tools Used for Social Engineering attacks.
#### 14) System Services
##### Buttons used to start some services.
#### 15) Usually used applications
##### Software for some basic purposes.
### Folder Managers
1. Dolphin
2. Thunar
3. Nautilus
### Linux Commands
##### Linux Systems uses shell. The shell help us to Communicate with the kernel and helps to execute codes.
##### Shell also called *Terminal*.
#### What is the default shell type for kali linux?
##### Kali Linux, use the **Z Shell** as their default shell.
#### Command Name
##### The terminal have 5 parts.
![[Pasted image 20240804003039.png]]
![[Pasted image 20240804003116.png]]
- [ ] Username = Kali
○ Hostname = Hunter
○ Current Directory = PATH
○ Priviledge = $-(user) , #-(root)
○ Command place = _
● Home directory is ~
● Local directory with .
● All directory *
- [ ] Directory Means Folder.
### Linux Command Basics
![[Pasted image 20240804003445.png]]
##### On linux there are over 100 commands. But we will see the main and the useful only.
##### Also those commands have their own options and arguments.
### What Is Command?
 ##### Is Small programs that do one task well.
 #### ls / List Directory
 ![[Pasted image 20240804003825.png]]
 ##### SYNOPSIS ls [OPTION]... [FILE]...DESCRIPTION List information about the FILE (the current directory by default).
 #### Content
 - [ ] ls -l
- [ ] ls -a
- [ ] ls filename
- [ ] ls -R => recursive
You can combine them, ls -Rla Linux hidden files startwith dot.
#### cd / Change Directory
###### SYNOPSIS cd [directory] DESCRIPTIONIt is used to change current working directory.
#### cont…
● cd / => root
● cd => home
● cd .. => 1x Back
● cd ../.. => 2x Back
● cd foldername
#### Pwd / print working directory
##### SYNOPSIS pwd [-options] DESCRIPTION It prints the path of the working directory, starting from the root. Example after typing pwd:
/home/omar/Desktop/OSLab
#### echo
##### echo command in linux is used todisplay line of text/string that are passed as an argument.
##### > this is save echo text.
##### >> this is *add or append* file terminal code.
### cat
##### Used to show the content of a file.
### touch
##### Creates any kind of Files with the name you gave it. With empty inside.
#### Mkdir / make directory
##### Creates Folder with the name u gave it.
#### rm / remove
##### rm [FILE1] [FILE2] [FILE3] DESCRIPTION \\Remove.
#### cont…
● rm -r => recursive(4 folders)
● rm -i => for prompt(ask)
● rm -f => force delete
###### You can use them in combination too like, rm -rf ‘filename’.
#### grep - global search for regular expression
###### ● grep [options] pattern [files]
###### ● The grep filter searches a file for aparticular pattern of characters, and displays all lines that contain that pattern.The pattern that is searched in the file is referred to as the regular expression (grep stands for global search for regular expression and print out).
#### cont…
● grep -i “search” file
○ - case insensitive
● grep -c “search” file
○ - count numbers
● grep -l “search” *
○ - displays filename
● grep -R “search” foldername
○ - search text in folders
● grep -v ‘term’ filename
○ To display without this term
● grep -n “term” file
○ To display the term find number
#### Wc - word count
![[Pasted image 20240804011250.png]]
![[Pasted image 20240804011306.png]]
##### wc [OPTION]... [FILE]... DESCRIPTION It is used to find out number of lines, word count, byte and characters count in the files specified in the file arguments. Line(-l) word(-w) byte(-c).
#### Multiple Command Executions
● You can run/ execute multiple commands in 1 line.
● using 3 methods:
○ And ( && )
○ Or ( || )
○ Pipeing( | )
#### AND ( && )
![[Pasted image 20240804011541.png]]
![[Pasted image 20240804011553.png]]
##### On AND operation All commands you entered will be executed. If both are working without error.
#### OR ( || )
![[Pasted image 20240804011801.png]]
![[Pasted image 20240804011815.png]]
##### On OR operation the command will be executed. If it have error or not.
#### Piping ( | )
![[Pasted image 20240804011921.png]]
![[Pasted image 20240804011944.png]]
##### On pipe, will help you run commands by using the output of the 1st command as the input for the next one.
# EXERCISE TIME
1) Create A text file with name paragraph.txt
“ Hello my name is <Yourname>, i got this course of linux and
said hello, and am tring to learn linux. I love linux, so i said HELLO
world “
2)  How many times did the word hello written ?
3) how many byte is the size of this text
4) how many words are there?
