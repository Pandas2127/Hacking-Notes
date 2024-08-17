# Finishing for Linux
## Topics
● Script Installation
● Errors on package managers
● Help on linux
● Linux Services
● Symbolic linking
● alias
● tmux
● Wget
● find
#### Script installation
###### Some hacking tools are developed by some peoples and those peoples make it open-source, that means we can get those scripts/programs from github.
###### So we can download and use it. For this purpose git have a feature called ‘clone’.
###### Syntax =>git clone <link_of_the_script_from_github>
#### Script modules
###### Scripts are made with scripting languages(programming) like *python,bash,go,ruby,...*
###### So when we use these programming languages to do tasks their is something called modules/libraries these are needed to run the script as the dependencies.
##### Example:
###### 1,Python: to install python modules we use -> pip install Python: to install python modules we use -> pip install *(modulename)*
i. For requirements file -> pip install -r requirements.txt
###### 2,Go: to install go modules -> go install *(modulename)*
###### 3,Ruby: to install ruby modules -> gem install *(modulename)*
#### Python installation
###### If pip is not found there will be an error.
###### It will install. (pip install term)
###### If the package is already installed:(pip install -r requirements.txt)
#### Go package installation
###### Go scripts are scripts made with go-lang(go programming language).
###### There are 2 installation methods:-
A. Old version
B. New version
##### Old version
###### A,go get github.com:capotej/groupcache-db-experiment.git
##### New version
###### A,Downloading the package go install github.com/lc/gau/v2/cmd/gau@latest
###### B,Moving the file to /usr/bin( the default download place is (/home/rexder/go/bin) sudo mv filename /usr/bin
#### Errors you may encounter
###### Don’t close apt while installation.
###### Repository errors, if this happened you can fix it using *sudo apt edit-source*
###### For those kinds of errors what you have to do is google/youtube { detail we will see this while we learn Footprinting }
#### If you need help on linux about commands
##### man (manual)
###### This will give you the whole manual and instruction of a tool or command. (man yourcommand) Keys: arrow keys for navigation | q for quit.
#### Cont…
##### Help
###### Some Commands have help option.
- [ ] yourcommand -h
- [ ] yourcommand -help
- [ ] yourcommand - -help
##### Breaking time
##### 1. Download and run the python script from this github
a. https://github.com/aboul3la/Sublist3r
##### 2. Download and test this go project
a. https://github.com/lc/gau
##### 3. What is the tr command on linux?
##### 4. What is the option for the ping command that can “use (size) as number of data bytes to be sent”.
### Linux Processes & Services
###### As we interact with Linux, we create numbered instances of running programs called “processes”.
###### To get the processes: ps [options]
###### More commands
- [ ] ps -> for process running on my shell
- [ ] ps -A -> view all running process
- [ ] ps -u username -> view users process
###### PID - Process ID
### Cont…
###### To stop process: Kill [options] [PID]
###### More on kill
- [ ] kill -19 PID -> to stop the process
- [ ] kill -18 PID -> to resume the process we stopped
- [ ] kill -9 PID -> to Stop a process immediately
- [ ] … there are 31 options.
#### Foreground / background
###### Thus far, we have run commands at the prompt and waited for them to complete. We call this running in the “foreground.”
###### Use the “&” operator, to run programs in the “background” or press ^Z
###### To get the background process back to foreground. [fg]
###### To stop a process going inside your shell just press ^C
### Null device
###### /dev/null - Redirects output to nowhere.
###### If you want to ignore output, you can send it to the null device, /dev/null.
###### The null device is a special file that throws away whatever is fed to it.
###### You may hear people refer to it as the bit bucket.
###### If you do not want to see errors on your screen and you do not want to save them to a file, you can redirect them to /dev/null
###### On shell output there are 2 things.
- [ ] STDERR= 2
- [ ] STDOUT= 1
###### To redirect the errors from a command result we do :command 2>filename
###### To redirect the error-FREE output :command  1>filename
###### So if we redirect our commands output to /dev/null we will get error free result :command 2>/dev/null
### Symbolic linking
###### Symbolic linking is same as Windows shortcut.
###### Symbolic linking is a process of creating a linked shortcut form of file to some pre-existed file or folder.
###### For example: you can create program is some file and to create a shortcut format of that file you will use symbolic linkin.
###### Also if a file path is too long we can create a symbolic linking.
###### Symbolic linked files shows ‘l’ in listing of ls command. Also there will be a ‘->’ to show the linked file.
###### Syntax: ln -s source_filePATH myfilename_
### alias
###### Used to give a name to some bunch of commands.
###### Example: if i wanted to name ls -la ‘rex so any time i want to get output of ls -la i just type rex : aliasrex='ls-la'
###### But this doesn’t work after you closed the terminal.
###### If you want to make it work…
- [ ] You will add it to your shell config file
###### Example for bash and fish,zsh.....
- [ ] Bash = ~/.bashrc
- [ ] Zsh = ~/.zshrc
- [ ] Fish = ~/.config/fish/config.fish
### Tmux - Terminal Multiplexer
###### Tmux is used to classify our terminal work.
###### You can install it using apt. On kali it is built-in
###### Then to start it just type ‘tmux’\
###### To Create config file type
○ nano .tmux.conf
○ Type this
- [ ] unbind C-b
- [ ] unbind l
- [ ] set -g prefix C-a
- [ ] unbind %
- [ ] bind e split-window -h
- [ ] bind o split-window -v
- [ ] set -g base-index 1
- [ ] setw -g pane-base-index 1
○ Save it | exit tmux and open again
### Cont…
###### To split horizontally : 
○ ^A then o
###### To split vertically
○ ^A then e
###### To exit
○ ^A then x or
○ just type ‘exit’
###### To create tab
○ ^A then c
###### To rename the tab
○ ^A then ,(comma)
###### To switch tabs
○ ^A then (numbers)
○ TO switch partitions
■ ^A then (arrow)
###### … for more you can google but be aware of our super key is ^A
### Wget
###### Is a tool used to download files from websites/servers.
###### Syntax : ○ wget [options] [link]
###### wget https://tldp.org/LDP/intro-linux/intro-linux.pdf
### find
###### ON terminal if you want to search for files/folders/musics/videos, we can use find command.
###### It is very essential tool
###### Syntax:
○ find [search path] [options] [search word]
###### More commands
- [ ] find / -name “linux”
- [ ] find /home -perm 777
- [ ] find -type f | find -type d
