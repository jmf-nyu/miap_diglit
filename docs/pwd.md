# The pwd Command

## Summary 
Command `pwd` stands for __print working directory__. It outputs the name of the directory you are currently in, called *working directory*.

## Basic command structure
For all descriptions below, the dollar sign indicates that BASH command prompt.

$ `pwd`

When navigating through files and directories in the terminal, `pwd` shows where you are in the filesystem.

## Possible Flags

### `-L`
The `-L` flag shows files that are normally hidden by BASH. These are files that begin with a `.` such as [.DS_Store](https://en.wikipedia.org/wiki/.DS_Store), [.bashrc](https://en.wikipedia.org/wiki/Bash_(Unix_shell)#Startup_scripts), or .bash_history.

### `-P`
The `-l` flag gives a column view of files and directories. It also gives information about those files and directories including permissions, last date modified and size.

## Output
The `pwd` command writes to standard output the full path name of your current directory (from the root directory). All directories are separated by a / (slash). 
The root directory is represented by the first /, and the last directory named is your current directory. 
* **Standard output**
![screenshot of pwd output](docs/$pwd_Codecademy.png)

* **Output with `-l` flag**, which displays directories and files in a list form with metadata in colums:
![screenshot of ls list output](ls_l-flag.png)

## Examples 
* If you want to see hidden files in a nice list format run $ `ls -la ~`. The `~` would indicate your home folder.
* To get a the contents of an entire directory structure starting at a parent folder: $ `ls -alRt`. If you'd like, you can use a redirect, such as `>` to send the output to a text file. Here's an example: $ `ls -alRt ~/Desktop > ~/Desktop/report.txt`

Go back to the [main list of commands](index.md)

