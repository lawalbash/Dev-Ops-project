# LINUX BASE FILE MANIPULATION 

## Prerequisites 

- Cloud service provider - AWS 

- Launch a Linux Instsnce (Ubuntu preferably) 

- Prior knowledge on how to SSH into virtual host 

- INSTALLING UBUNTU SERVER 

Update to authenticate into the virtual server 

'sudo apt update'

The sudo command short for "superuser do" is used in linux to perform tasks that require administrative or root permissions. This is the result below for using the sudo command:

![Alt text](images/Capture1.JPG)

2- PWD COMMAND

'pwd'

The pwd command is used to find the path of your current/present working directory. It has also has two acceptable options that can be used with it; -l which prints environment cariable content including symbol links, -P prints the actual path of the current directory.

![Alt text](images/Capture2.JPG)

- CD COMMAND

'cd /home/ubuntu/CommandsLinux or cd CommandsLinux'

The cd command is used to navigate through Linux folders/directories.

![Alt text](images/4.JPG)

- LS COMMAND

'ls'

The ls command is used to list files and directories within a system. Running the command without a flag will only show the current working directory's content.

![Alt text](images/Capture5.JPG)

Here are some flags that can be used with the ls command:

"ls -R", "ls -R, "ls -a" : This lists all the files in the subdirectories 

![Alt text](images/Capture8.JPG) 

- CAT COMMAND

'cat filename.txt'

The Concatenate or cat command is used to list, combine and write file contents to the standard output.

![Alt text](<images/Capture new cat.JPG>) 

The "tac filename" can also be used but the contents are going to be displayed in reverse order. 

![Alt text](<images/Capture new tac.JPG>) 

- CP COMMAND

'cp filename /destination_directory/'

The cp command is used to copy files or directories and their contents 

![Alt text](<images/Capture new cp file.JPG>)

- MV COMMAND

'mv filename /destination_directory/'

The mv command is used for the purpose of moving a file or directory to another directory or used to rename a file.

![Alt text](<images/capture new mv2.JPG>) 

- MKDIR COMMAND

mkdir [option/flag] directory_name

The mkdir command is used to create one or multiple directories at once and set permissions. Ensure you are authorize to make a new folder in the parent directory.

![Alt text](<images/Capture new mkdir.JPG>) 

To create another directory in your already created directory, we use this syntax;

'mkdir parent_directory/new_directory'

![Alt text](<images/Capture mkdir music.JPG>)

- RMDIR COMMAND 

'rmdir -p /directory_name/'

The rmdir command, in the other hand is used to remove/permanently delete empty directory or directories.

![Alt text](<images/Capture rmdir.JPG>) 

- RM COMMAND 

rm filename

We use the rm command to remove files within a directory, and its action is not reversible. So we must take caution while in the use of the command. 

![Alt text](<images/Capture 10.JPG>) 

To remove multiple files at once, we use this syntax;

'rm filename1 filename2 filename3'

![Alt text](<images/Capture new rm.JPG>) 

- TOUCH COMMAND

'touch filename'

The touch command is used to create new empty files.

![Alt text](<images/Capture 11.JPG>) 

- LOCATE COMMAND 

'locate -i filename1*filename2 '

The locate command is used to locate a file in the database system. The -i arguement is used to turn off case sensitivity incase you don't remember the file's exact name, while the * is used to look for contents which contains two or more words.

![Alt text](<images/Capture new locate.JPG>) 

- FIND COMMAND

'find [option] [path] [expression]'

The find command is used to search for files within a specific directory and performs subsequent operations

![Alt text](<images/Capture new find.JPG>)

- DF COMMAND

'df [options] [file]' 

The df command is used to report the system's disk space usage, the information is shown in percentage and kilobyte (KB).

![Alt text](<images/Capture new df.JPG>) 

- DU COMMAND

'du directory_path'

checks a file or directory’s storage consumption.

![Alt text](<images/Capture new du.JPG>) 

- HEAD COMMAND

'head [option] [file] '

The head command is used to view the first ten lines of a text file. Adding an option lets you change the number of lines shown.

![Alt text](<images/Capture new head.JPG>)

- TAIL COMMAND

'tail [option] [file]'

The tail command on the other hand is used to read the last ten lines of a text file. It allows users to check wether a file has new data or to read error messages.

![Alt text](<images/Capture new tail.JPG>) 

- DIFF COMMAND

'diff [option] file1 file2'

The diff command short for difference, is used to compare two contents of a file line by line. After analyzing them, it will display the parts that do not match.

![Alt text](<images/Capture new diff.JPG>) 

- TAR COMMAND

'tar [options] [archive_file] [file or directory to be archived]'

The tar command is used to archive multiple files into a tar file,which is a common linux format similar to the ZIP with optional compression

![Alt text](<images/Capture new tar.JPG>)

## FILE PERMISSIONS AND OWNERSHIP 

- CHMOD COMMAND 

'chmod [option] [permission] [file_name]'

The chmod command is a command that modifies a file or directory's read, write and execute permissions.

![Alt text](<images/Capture chmod.JPG>) 

- CHOWN COMMAND 

'chown [option] owner[:group] file(s) '

The chown command changes the ownership of files in Linux systems. The user can change their own ownership but not others' unless they have root privileges.

![Alt text](<images/Capture chown.JPG>) 

- JOBS COMMAND

'jobs [option] jobID'

The job command is used to display all the running processes along with their statuses.

![Alt text](<images/Capture job.JPG>)

- KILL COMMAND

'kill [signal_option] PID'

The kill command is used to terminate an unresponsive program manually. It will signal misbehaving applications and instruct them to close their process.

![Alt text](<images/Capture kill.JPG>)

To kill a program using the above syntax, you must know its process identification number (PID). To know the PID of a program, we use the below command;

ps ux

![Alt text](<images/Capture px us.JPG>)

- PING COMMAND

'ping [option] [hostname_or_IP_address]'

The ping command is a basic linux command used for checking  a network or service is reachable, and it is also used to troubleshoot various connectivity issues.

![Alt text](<images/Capture ping.JPG>) 

- WGET COMMAND

'wget [option] [url]'

The wget command lets you download files from the internet, it runs in the background without hindering other running processes.

![Alt text](<images/Capture wget.JPG>) 

- UNAME COMMAND

'uname [option]'

The uname command or in full, unix name command will print detailed information and your linux system and hardware. The informations includes the machine name, operating system and kernel.

![Alt text](<images/Capture 12.JPG>)

- TOP COMMAND

'top'

The top command in linux terminal will display all the running processes and a dynamic real-time view of the current system. It sums up the resource utilization, from the CPU to the memory usage.

![Alt text](images/top.JPG)

- HISTORY COMMAND

'history [option]'

The history command is used in linux to list up to 500 previously executed commands, allowing you to reuse them without re-entering them. However only users with the sudo privileges can execute this command.

![Alt text](<images/Capture history.JPG>)

- MAN COMMAND

'man [command_name]'

The man command provides a user manual of any Linux Terminal utilities, including their names, descriptions, and options.

![Alt text](<images/Capture man.JPG>)

- ECHO COMMAND

'echo "string" or echo string > file'

The echo command is a built-in utility that displays a line of text or string using the standard output.

![Alt text](<images/Capture echo.JPG>) 

- ZIP COMMANDS 

'zip [options] zipfile file1 file2….'

The zip command is used in linux to compress files into a ZIP file, a universal format commonly used in linux.

![Alt text](<images/Capture zip.JPG>)

- UNZIP COMMANDS

Unzip command extracts the zipped files from an archive. Here's the general syntax.

'unzip [option] file_name.zip'

![Alt text](images/Capture32.JPG)

- HOSTNAME COMMAND

'hostname [option]'

This command prints out your system’s hostname (or domain name). The default behavior for this command without any options will print just one word.

![Alt text](<images/Capture hostname.JPG>)

- USERADD COMMANDS

'useradd [option] username'

Useradd command is used to add new users to the system as linux is a multi-user system and only those with root/sudo privileges can run this command.

![Alt text](<images/Capture useradd.JPG>)

- USERDEL COMMAND

To delete a user account we use the userdel command.

'userdel [option] username'

![Alt text](<images/Capture userdelete.JPG>)

- APT-GET COMMAND

'APT-GET COMMAND'

Apt-get is a command line tool for handling Advanced Package Tool (APT) libraries in linux. It is used to retrieve information and bundles from authenticated sources to manage, update, remove and install software and its dependencies.

![Alt text](<images/Capture apt get.JPG>)

- NANO COMMAND

'nano [filename]'

The nano command is a basic text editor.

![Alt text](<images/Capture nano.JPG>)

- VI COMMAND

The vi command is used to edit and create a text file. It also performs other operations like saving, opening, copying and pasting a file. To use the vi command, we use this syntax;

'vi [filename]'

![Alt text](<images/Capture vi.JPG>)

- JED COMMAND

And jed command which stands for "Just Edit". It's basically vi command but it is known for its simplicity and extensibility. To use the jed command, we use this command syntax;

'jed [filename]'

![Alt text](images/Capture24.JPG)

- ALIAS

'alias Name=String'

The alias command will create an alias for any command that you want in your system.

![Alt text](<images/Capture alias.JPG>)

- UNALIAS

'unalias [alias_name]'

The unalias command on the other hand is used to delete an existing alias. 

![Alt text](<images/Capture alias.JPG>)

- SU COMMAND

'su [options] [username [argument]]'


The su command or switch user command is used to switch between existing users on the command line.

![Alt text](<images/Capture 24.JPG>)

- HTOP COMMAND

'htop [options]'

The htop command is an interactive program that monitors system resources and server processes in real time.

![Alt text](<images/Capture htop.JPG>)

- PS COMMAND

'ps'

The ps command or process status command produces a snapshot of all running processes in your system.

![Alt text](<images/Capture ps.JPG>)

