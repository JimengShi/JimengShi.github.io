---
layout:     post
title:      Ubuntu Common Commands
subtitle:   Share some common commands and shortcuts of Ubuntu
date:       2021-03-01
author:     Jimeng
header-img: img/southeast_view.jpg
catalog: true
tags:
    - Ubuntu, Linux
---

## 1. Sudo
    $ sudo: SuperUser DO
Sudo allows you to run programs or other commands with administrative privileges, 
just like “Run as administrator” in Windows.


## 2. Apt-Get
Apt-get is used to install, update, upgrade and remove any package. 
Here is the list of different apt-get commands:


### 2.1 Sudo apt-get update    
    $ sudo apt-get update
    
Apt-get update with super user privileges is the first command you need to run 
in any Linux system after a fresh install. 
This command updates the database and let your system know if there are newer packages available or not.
    

### 2.2 Sudo apt-get upgrade 
    $ sudo apt-get upgrade
    $ sudo apt-get upgrade <package-name>
    
After updating the package database, next step is to to upgrade the installed packages. 
And if you like to upgrade a particular package, you should tweak the above command, 
and replace the <package-name> with your desired package.


### 2.3 Sudo apt-get upgrade 
    $ sudo apt-get install
    $ sudo apt-get install <package-name>
    
Install some packages.


### 2.4 Sudo apt-get remove
    $ sudo apt-get remove
    $ sudo apt-get remove <package-name>
    
Sudo apt-get remove <package-name> removes package. 
You only have to know the exact package name of the software you want to uninstall.
If you don’t know the package name, use below command to list all the packages 
installed on your system and then copy the package name you want to remove:

    $ dpkg --list


### 2.5 Sudo apt-get purge
    $ sudo apt-get purge
    
It is used to remove a software completely from your system with its configuration or data files 
so that no longer personalized settings will be available during reinstallation.


### 2.6 Sudo apt-get autoremove
    $ sudo apt-get autoremove
    
It is used to remove any unnecessary packages. Unnecessary means, whenever you install an application, 
the system will also install the software that this application depends on.
It is common in Ubuntu that applications share the same libraries. 
When you remove the application the dependency will stay on your system.
So it's used to remove unwanted software dependencies after uninstalling a package.


## 3. Ls [1]
ls (list) command lists all files and folders in your current working directory. 
You can also specify paths to other directories if you want to view their contents.

    $ ls
    
List the contents of the current working directory


    $ ls [directory path here]
    
List the contents of another directory:
    
    
    $ ls /
    
List the contents of the root directory


    $ ls .. 
    
List the contents of the parent directory one level above.


    $ ls ../.. 
    
List the contents of the parent directory two levels above.


    $ ls ~
    
List the contents in the users's home directory


    $ ls -d */
    
List only directories


    $ ls *
    
List the contents of the directory with it's subdirectories.


    $ ls -s (the s is lowercase)
    
List files or directories with their sizes


    $ ls -l (list files in long format)
    
    
List the contents of the directory in a table format with columns including:
- content permissions
- number of links to the content
- owner of the content
- group owner of the content
- size of the content in bytes
- last modified date / time of the content
- file or directory name

    
    $ ls -lh (List files in long format with readable file sizes)
    
List the files or directories in the same table format above, 
but with another column representing the size of each file/directory


    $ ls -a 
    
List files or directories including hidden files or directories. 
In Linux, anything that begins with a is considered a hidden file.


    $ ls -l -a or ls -a -l or ls -la or ls -al
    
List files or directories in a table format with extra information including hidden files or directories


    $ ls -t
    
List files or directories and sort by last modified date and time in descending order (biggest to smallest).
You can also add a -r flag to reverse the sorting order like so: ls -tr


    $ ls -S (the S is uppercase) 
    
List files or directories and sort by date or time in descending order (biggest to smallest).
You can also add a -r flag to reverse the sorting order like so: ls -Sr


    $ ls > output.txt
    
Print the output of the preceding command into an output.txt file. 
The key point here is that the result will be outputted into a file and not logged to the command line.
Then you can use the file, or log the contents of the file with cat output.txt


## 4. Cd
    $ cd <folder name>
Cd (change director”) Linux command is used to change the current working directory. 
Some common uses are:

    $ cd /  – Takes you to the root directory.
    $ cd .. – Takes you up one directory level.
    $ cd –  – Takes you to the previous directory.


## 5. Pwd
    $ Pwd 
    
Print working directory displays the full pathname of the current working directory.


## 6. Cp
    $ cp
cp (copy) Linux command allows you to copy a file. 

You should specify both the file you want to be copied and the location you want it copied to 
For example, cp xyz /home/myfiles would copy the file “xyz” to the directory “/home/myfiles”.


## 7. Mv
    $ mv (move) command allows you to move files. 
    
You can also rename files by moving them to the directory they are currently in, 
but under a new name. The usage is the same as cp. 
For example mv xyz /home/myfiles would move the file “xyz” to the directory “/home/myfiles”.


## 8. Rm
    $ rm (remove) command removes the specified file.
    
rmdir (“remove directory”) – Removes an empty directory.
rm -r (“remove recursively”) – Removes a directory along with its content.


## 9. Touch 
    $ touch file1.txt
    
If the file file1.txt doesn’t exist the command above will create it, otherwise,
it will change its timestamps.

    $ touch file1.txt file2.txt file3.txt
    
Create multiple files at once, specify the file names separated by space.


## 10. Cat
Cat(concatenate) command reads data from the file and gives their content as output. 
It helps us to create, view, concatenate files.

    $ cat filename
    
View a single file.


    $ cat file1 file2

View multiple files.


    $ cat -n filename

View contents of a file preceding with line numbers.


    $ cat > newfile

Create and a file named newfile.


    $ cat [filename-whose-contents-is-to-be-copied] > [destination-filename]

The content will be copied in destination file.


    $ cat file1 >> file2
   
Append the contents of one file to the end of another file.


## 11. Mkdir
    $ mkdir (make directory) Allows you to create a new directory. 
    
You can specify where you want the directory created – if you do not do so, 
it will be created in your current working directory.


## 12. History
    $ history
    
history command displays all of your previous commands up to the history limit.


## 13. Df
    $ df: display filesystem
    
It displays information about the disk space usage of all mounted filesystems.

## 14. Passwd
    $ passwd
    $ passwd <user>
    
It is used to change user password using Terminal. 
What you have to do is run the above command, where is the username whose password has to change.


## 15. Shortcuts
- Ctrl + Shift + T: Open new tab on current terminal
- Ctrl + Shift + W: Close the current tab
- Ctrl + A: Move cursor to beginning of line
- Ctrl + E: Move cursor to end of line
- Ctrl + U: Clears the entire current line
- Ctrl + K: Clears the command from the cursor right
- Ctrl + W: Delete the word before the cursor
- Ctrl + R: Allows you to search your history for commands matching what you have typed
- Ctrl + C: Kill the current process
- Ctrl + Z: Suspend the current process by sending the signal SIGSTOP
- Ctrl + L: Clears the terminal output
- Alt + F: Move forward one word
- Alt + B: Move backward one word
- Ctrl + Shift + C:	Copy the highlighted command to the clipboard
- Ctrl + Shift + V or Shift + Insert: Paste the contents of the clipboard
- Up/Down Arrow keys: To scroll through your command history, allowing you to quickly execute the same command multiple times


## Reference
[1] https://www.freecodecamp.org/news/the-linux-ls-command-how-to-list-files-in-a-directory-with-options/#:~:text=The%20ls%20command%20is%20used,them%20via%20the%20command%20line

[2] https://www.tecmint.com/15-basic-ls-command-examples-in-linux/

[3] https://techlog360.com/basic-ubuntu-commands-terminal-shortcuts-linux-beginner/