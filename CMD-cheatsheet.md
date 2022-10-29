title	description
CMD CheatSheet
The most commonly used cmd commands are given here.
Table of Contents
CMD CheatSheet for Developers
RAA (Run As Administrator)
File and Folder Management:
Applications and Processes:
Disk Management:
System Information:
Network:
Command Line Setup:
CMD CheatSheet for Developers
RAA (Run As Administrator)
File and Folder Management:
Command	Description
?	Help or sometimes shows related commands to some commands.
cd	- To open directory
- cd directory-name.
copy	Copies files to another location
dir	List directory content.
del	Used to delete one or more files.
expand	Decompresses compressed files.
fc	File compare- fc a.txt b.txt.
find	Find files.
ftype	Display file type and mapping.
mkdir	Make a directory.
move	Moves files from one folder to another.
print	Prints out the text file contents.
rd
rmdir	- Removes the directory
- rmdir [dir]
- rd [dir]
ren	Rename.
replace	Replaces files in one directory with files of the same name in another directory.
robocopy	Uses an advanced tool to copy files and directories.
tree	Show all system folder in tree manner.
type	Displays the contents of text files.
xcopy	The xcopy command can copy one or more files or directory trees from one location to another.
🔼Back to Top

Applications and Processes:
Command	Description
schtasks	Executes a command or start a scheduled application (Task Scheduler).
shutdown	- Shutdown your computer, control system shutdown using additional commands
- shutdown
- shutdown/?
- shutdown/i
tasklist	Display a list of currently-running tasks
taskkill	- Kills the running task
- taskkill /im [programme-name]
- taskkill /im notepad.exe
- taskkill /f /im notepad.exe
reg	Starts registry editor
runas	Launches the task as another user
🔼Back to Top

Disk Management:
Command	Description
chkdsk	- Scan the disk/drive errors
- chkdsk [disk-name]:
- chkdsk C:
defrag	Starts disk defragmentation.
compact	Displays and change the compression of files in NTFS partitions.
format	Formats the disk.
Recover	Recovers data from a bad or damaged disk.
sfc	- System file checker, scans all system files and repairs them if required
- sfc /scannow
vol	Displays volume label and serial number for the disk.
🔼Back to Top

System Information:
Command	Description
date	Show/Set date.
hostname	Shows hostname of the computer.
powercfg	- Gives report of the power setting
- powercfg /?
- powercfg /list
systeminfo	To get system-related information.
time	Displays or sets the system time.
ver	Display operating system version.
finger	Information about the user.
whois	This command is useful when users want to find the domain name or the IP address.
ftp	Transfer file to a ftp server.
getmac	Display mac address.
mode	Used to configure system devices.
print	Print a specified text file to a specified printing device.
🔼Back to Top

Network:
Command	Description
ipconfig	Display IP network settings.
ping	- Test the ability of the source computer to reach a specified destination computer
- Show the list of usage and options in cmd
- Get a response from the website network
- ping [website name]
- ping [ip address]
nslookup	Finds IP address by resource name.
route	This command is used to check and make changes to the route table of the computer.
arp	Shows a table with IP addresses converted into physical addresses.
netsh	- Allows you to display or modify the network configuration of a computer that is currently running
- Commands used for various properties related to network
- netsh (step-1)
- netsh> /?
netsh wlan	- Command extension to the netsh
- netsh (step-1)
- netsh> wlan /?
🔼Back to Top

Command Line Setup:
Command	Description
cls	Clear screen.
color	Changes text and background color.
echo	Print the after echo text once.
prompt	Changes the command line prompt (print the after text until you close the cmd)
pause	Pause your window until you press any key.
title	Title your command prompt.
timeout xxx	Countdown wait in terminal- xxx in seconds.
exit	Exit from the cmd window.
reset	The reset command executed as reset session.
🔼Back to Top
