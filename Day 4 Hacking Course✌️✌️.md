
![[Further on Linux.pdf]]
# Further On Linux
## Topics
- [ ] LINUX FILE HIERARCHY
- [ ] VIM
- [ ] NANO
- [ ] LINUX USER MANAGEMENT
### Linux File Hierarchy
![[Pasted image 20240729210401.png]]
##### Linux/UNIX have a special file system than windows.
##### File system is a directory structure that the OS uses.
### System Files
##### System Files are files used by the system software(OS)
##### Windows:System files appear under the Local disk C:
##### Linux:System files appear under the root directory(/)
![[Pasted image 20240729211056.png]]
## File Structure In Detail
1. /(Root)
- [ ] Every single file and directory starts from the root directory.
- [ ] The only root user has the right to write under this directory.
- [ ] Root is the root user's home directory.Which is not the same as/
2. Bin-Binary Executables
- [ ] Essential command binaries that need to be available in single-user mode; for all users. EXAMPLE:cat,ls,cp,pwd
3. /Boot-Boot loader files
- [ ] Kernel initrd, vmlinux,grub File are located under /Boot
4. /dev-Essential Device Files
- [ ] These include terminal devices, usb, or any device attached to the system.
5. /etc-etc cetera
- [ ] Contains Configuration files required by all programs.
6. /home - Home directory
 ![[Pasted image 20240804222955.png]]
- [ ] Home directories for all users to store their personal files. ○ example: /home/nathan,/home/rexder.
7. /lib - Libraries essential for the binaries in /bin & /sbin
- [ ] Library filenames are either ld *or lib*.so.*
○ Example: ld-2.11.1.so,
libncurses.so.5.7
8. /media - Mount points for
removable media such as CD-ROMs
- [ ] Temporary mount directory
for removable devices.
○ Examples, /media/cdrom for
CD-ROM; /media/floppy for
floppy drives; /media/cd
recorder for CD writer.
9. /mnt - Temporarily mounted file
- [ ] Temporary mount directory
where sysadmins can mount
filesystems.
10. /opt - Optional application
software packages
- [ ] Contains add-on applications
from individual vendors.
○ Add-on applications should be
installed under either /opt/ or
/opt/ sub-directory.
11. /sbin - Essential system binaries
- [ ] Just like /bin, /sbin also
contains binary executables.
○ The linux commands located
under this directory are used
typically by system
administrator, for system
maintenance purpose.
12. /tmp - Temporary Files
- [ ] Directory that contains
temporary files created by
system and users.
○ Files under this directory are
deleted when system is
rebooted.
13. /usr - User Utilities
- [ ] Contains binaries, libraries, documentation, and
source-code for second level programs.
○ - /usr/bin contains binary files for user programs. If
you can’t find a user binary under /bin, look under
/usr/bin. For example: at, awk, cc, less, scp
○ - /usr/sbin contains binary files for system
administrators. If you can’t find a system binary
under /sbin, look under /usr/sbin. For example: atd,
cron, sshd, useradd, userdel
○ - /usr/lib contains libraries for /usr/bin and
/usr/sbin
○ /usr/src holds the Linux kernel sources,
header-files and documentation.
### Text Editors
##### Programs That used for text processing.
##### Linux command line text editors.
- [ ] VIM
- [ ] NANO
- [ ] EMACS
- [ ] NEO VIM
- [ ] ......
##### Linux Graphical Text editors.
- [ ] SUBLIME
- [ ] VS CODE
- [ ] GEDIT
- [ ] PLUMA
- [ ] ...
### VIM
##### Before vi the primary editor used on Unix was the line editor.
###### User was able to see/edit only one line of the text at a time.
##### Then then vi editor improved and developed VIM. (VI improved).
##### The vim editor is:
###### a very powerful
###### but at the same time it is cryptic
###### It is hard to learn, specially for windows users
##### It have mainly to modes
###### Command mode -> where you can do commands
###### Input mode -> where you can write
## Vim
##### Vim Is By default on *Command* mode when you open it. To get on *insert mode* you have to type 'i' (INSERT).
##### To get back to command mode you press ‘esc’
#### Inside Command mode you can:
###### Save
###### Save & quit
 ###### Force Quit & Save
 ###### Undo
 ###### Execute bash commands
##### Save Type :w+ enter.
##### Quit Type :q+ enter.
##### Quit Type :wq!+ enter FORCE Quit!
##### Undo Type :undo+ enter.
##### Execute Commands Type :%!Your command.
## Nano
##### The GNU nano text editor is a user-friendly, free and open-source text editor that usually comes pre-installed in modern Linux systems.
#### Saving Exiting & Undo_Redo
###### Ctrl + S - save
###### Alt + U - Undo
###### Alt + E - Redo
###### Ctrl + X - Exit
#### Paste,Copy & Paste all over the linux is 
###### Ctrl+shift+C - copy
###### Ctrl+shift+X - Cut
###### Ctrl+shift+V - Paste
# EXERCISE IN YOUR LINUX
1. Create A text file called “takeme.txt” using vim
a. Text: “ This is The Inserted Text from Planet Mars!”
b. Save and Exit
2. Create Another text file called “Day3_MoreLinux.md”
using nano
a. Text: “This is day 3 course note.”
b. Save and exit
3. Open Day3_MoreLinux.md Read the file “takeme.txt” using
nano and add it to “Day3_MoreLinux.md”
## Linux User Management
##### On Computer system, person who uses the computer is called “user”.
##### Every Users have Group.
##### Users have their own file & applications.
##### To know our name on linux -> “ who am i “.
##### Those users have power/privilege.
##### On linux there's 2 kinds users.
- [ ] Root Id=0
- [ ] Normal User id start with 1-999
##### The root user have the power to do everything on linux ,but if users want to have a root access they add sudo in front of the command .
## Creating Users
##### On linux, to create users you can use the following commands.
- [ ] Useradd -> simple
- [ ] Adduser -> Detailed
##### Useradd command.
- [ ] sudo useradd username
##### Adduser command.
- [ ] sudo adduser username
##### The User files are stored inside /etc/passwd.
##### The User password are stored inside /etc/shadow.
##### When you create a user it creates a group with that name.
### Checking /etc/passwd
This happened what shall i do?
![[Pasted image 20240804235747.png]]
## To access root user
![[Pasted image 20240805000054.png]] 
###### sudo su