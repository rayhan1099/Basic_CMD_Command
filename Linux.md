
					Ubuntu linux Commands
			

1- apt-get update
This command will update your package lists. Remember, this will not update software. Run Command #2 or #3 followed by this command. Note that apt-get require root permission. You should add sudo before apt-get.

2- apt-get upgrade
This command will download and update installed software. But it will not install or remove extra packages.

3- apt-get dist-upgrade
To upgrade all the packages on your system, and, if needed for a package upgrade, installing extra packages or removing packages.

4- apt-get install <package-name>
You may download and install new packages or software named <package-name> using above commands. E.g. run sudo apt-get install gimp in your terminal to install Gimp image manipulation software. Notice the sudo before apt-get.

5- apt-get -f install
Sometimes while installing a software it fails. This might happen due to failure in downloading software itself or dependency. To fix broken installation run the above command.

6- apt-get remove <package-name>
If you don’t like a software you can get rid of that by simply running above command. Don’t forget to change <package-name> with real one. This will uninstall the software but not the dependent packages.

7- apt-get purge <package-name>
To completely remove a software and it’s dependent packages run the apt-get purge command.

8- apt-get autoclean
This command will remove all Debian (.deb) files that are no longer installed. You may find this files in /var/cache/apt/archives

9- apt-get clean
This will empty whole cache files. A lot of space could be freed if you frequently install and uninstall softwares.

10- apt-get automove
It will remove old dependent files and footprints installed by previous applications.

11- dpkg –configure -a
configure installed package

12- sudo nano /etc/apt/sources.list
display repository source list in nano editor

13- sudo apt-get download <package-name>
download but not install package

14- Ctrl + c
It kills process with a signal SIGINT. Don’t confuse with Ctrl+C in Windows or Ctrl+Z. Ctrl+Z is used to suspend a process while In Windows Ctrl+C is copy command.

15- Ctrl + Shift + c
This is a copy command.

16- Ctrl + Shift + v
This is paste command like Ctrl+v in Windows.

17- nano <filename>
nano is command line text editor. In terminal by running the above command you could edit file named <filename>.

18- sudo nano <filename>
This is same command as we mentioned earlier except it will edit file with privilege of super user.

19- gedit <filename>
gedit is GUI text editor like notepad in Windows. It will start editing file named <filename> in gedit window.

20- sudo gedit <filename>
This is again same as above except it will edit files with SU privilege. It is worth to mention this command because many beginners starts editing a file and later they realize they forget to get proper privilege.

21- sudo poweroff
This will shut down the system as the name suggest.

22- sudo halt
Halt is supposed to be same as poweroff by many beginners. But it’s not unless you explicitly mention to poweroff using either -p or–poweroff.So if you want to poweroff your system then use sudo halt –p or sudo halt –poweroff.

23- sudo reboot
This will simply reboot your system.

24- Ctrl + Alt + t
Open Ubuntu Terminal Window, the command line interface. This is a preinstalled software comes with every standard Ubuntu.

25- pwd
print work directory: e.g. if you are at your home directory then it will print something like /home/<username>

26- ls
list directory: This command will list the items of a directory. If you don’t specify a directory then it will list work directory, the place where you currently are.

27- cd
change directory. It will change your work directly as you specify. You will have to specify a directory.g. cd /home will change your work directory to /home regardless where you are.

28- cd ..
change directory one level up.

29- cd ~
change to home directory. Suppose if your username is tom then cd ~ will change your work directory to /home/tom.

30- cp
Copy Command. It will copy a file or directory. It is similar to Copy-Paste in GUI.

31- mv
Move or rename files. It is like renaming a file or cut-paste in GUI.

32- rm
remove file or directory.

33- rmdir
remove empty directory. This will not remove content of the directory but it will delete a directory if it is empty.

34- mkdir
make directory. It will create a new directory. We will need to specify a name.

35- man
Ubuntu will help you instantly and has a built in manual. Simply apend any command with man or type executes man. e.g. man mkdir

36- sudo
sudo basically allow a standard user to execute a command with root or superuser privilege.

37- adduser <username>
As the name suggest it will add another user. You may also use useradd, which is a little bit different from the adduser.

38- passwd <username>
This command will change password for an user named <username>. Root privilege will be require while change other user’s password.

39- time
time command in Ubuntu will not actually show you current date or time. It will actually run and show the summary system resources usages.Tip: run time gedit in terminal. You will see a new gedit window. After a few seconds close the window and see what appears in the terminal. It will be something like:real     112s
user     0m0.560s
sys        0m0.050sCheck this wikipedia article.

40- date
This command will show you the current date and time of your system (including timezone).

41- cal
This will show calender in the terminal.

42- wget
You can use wget command to download things from Internet or other connected networks.

43- ping
You may ping websites and other devices with ping command. This is a part of iputils package. Pinging is something like saying hello to someone and that person reply you back. Which means you are connected and the remote person (or system) is replying you back. Try

ping -c 4 ubuntubeginner.com

When you execute this command your system will say ubuntubeginner.com‘s server ‘hi’ 4 times. -c 4 stands for 4 times.

44- ftp
ftp (file transfer protocol) is used to transfer files for one system to another system.

45- ssh
ssh (secure shell) is used to log into remote system or server. By default Ubuntu comes with SSH program preinstalled.

46- fdisk
fdisk command is used to manipulate (add, remove, delete, change) partition of your system. NOTE: Don’t use this command unless you are sure about the consequences.

47- df
df is a very handy command which show the storage used/free on your the storage drives connected to your system.

48- chmod
chmod is very useful command for beginners. It is used to change file permission. chmod stands for change mode in Linux.

49- chown
chown is used to change owner of a file or directory (or further more). Beware about using chown or chmod commands

50- sudo su
superuser in Ubuntu Desktop is disabled by default. But if you want to act as a superuser (or root) then use this command. You will be asked for password. sudo su will allow the terminal session to run all commands and activity with superuser privilege.Don’t forget to close the root session by using exit command.
WARNING: Acting as su or root could be dangerous. Beginners should consider using sudo.

51- clear
Clear Screen: Use clear command to clear the terminal screen.

52- exit
exit from terminal.

53- free
The command “free” displays the amount of free and used memory in the complete system.
Syntax: free

54- Ps
The command “ps” which is also known as process status command is used to provide information about the processes currently running on the system, including their respective process identification numbers (PIDs).
Syntax: ps

55- uptime
The command “uptime” provides information about how long the system has been running in one line. Result for this command includes the current time, the time duration system has been running for, the number of users who are currently logged on, and the system load averages for the past 1, 5, and 15 minutes respectively.
Syntax: uptime

56- w
The command “w” displays the detailed information about the users who are logged in the system currently.
Syntax: w

57- passwd
The command “passwd” stands for password and it is used to change the password of the user.
Syntax: passwd user_name

58- sudo
The command “sudo -I” is used to continue the session as a root user which has a lot more privileges than normal system user.
Syntax: sudo -i

59- history
The simple command “history” displays the list of all commands entered since the user started the session.
Syntax: history

60- help
The command of “help” provides you help to learn about all the built-in commands.
Syntax: help

Ubuntu Terminal Shortcuts	Function

Ctrl + Shift + T	Open new tab on current terminal

Ctrl + Shift + W	Close the current tab

Ctrl + A		Move cursor to beginning of line

Ctrl + E		Move cursor to end of line

Ctrl + U		Clears the entire current line

Ctrl + K		Clears the command from the cursor right

Ctrl + W		Delete the word before the cursor

Ctrl + R		Allows you to search your history for commands matching what you have typed

Ctrl + C		Kill the current process

Ctrl + Z		Suspend the current process by sending the signal SIGSTOP

Ctrl + L		Clears the terminal output

Alt + F			Move forward one word

Alt + B			Move backward one word

Ctrl + Shift + C	Copy the highlighted command to the clipboard

Ctrl + Shift + V or Shift + Insert	Paste the contents of the clipboard

Up/Down Arrow keys	To scroll through your command history, allowing you to quickly execute the same command multiple times

TAB	Used to complete the command you are typing. If more than one command is possible, you can press it multiple times to scroll through the possible completions. If a very wide number of commands are possible, it can output a list of all possible completions.
