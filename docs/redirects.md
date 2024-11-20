# Redirects - WIP

## Summary 
Redirection assists in redirecting input & output functionalities to the files or folders we want. There are 2 types of redirection:
### 1. Overwrite Redirection
The `>` command
This will store/save the output of a command to a file & overwrite existing content of that file. 
### 2. Append Redirection
The `>>` command 
This will redirect the standard output of a command on the left of `>>` & append it to the end of the file on the right of `>>` - this will not compromise the existing data of the file it is added to. 


## Basic command structure
For all descriptions below, the dollar sign indicates that BASH command prompt.

$ `ls [options] [directory path]`

Note: If you do not specify a directory path, running `ls` will show you the contents of the current directory you are in within your terminal window, i.e., your current working directory.

## Possible Flags

### `-a`
The `-a` flag shows files that are normally hidden by BASH. These are files that begin with a `.` such as [.DS_Store](https://en.wikipedia.org/wiki/.DS_Store), [.bashrc](https://en.wikipedia.org/wiki/Bash_(Unix_shell)#Startup_scripts), or .bash_history.

### `-l`
The `-l` flag gives a column view of files and directories. It also gives information about those files and directories including permissions, last date modified and size.

### `-h`
When used in combination with the `-l` flag, the `-h` flag displays file size in human-readable units such as kilobytes, megabytes, and gigabytes.

## Output
The `ls` command has many different kinds of outputs as described below:
* **Standard output** with no flags, which displays the names of directories and files within the directory where the command is run:
![screenshot of ls output](ls_no-flags.png)

* **Output with `-l` flag**, which displays directories and files in a list form with metadata in colums:
![screenshot of ls list output](ls_l-flag.png)

## Examples 
* If you want to see hidden files in a nice list format run $`ls -la ~`. The `~` would indicate your home folder.
* To get a the contents of an entire directory structure starting at a parent folder: $`ls -alRt`. If you'd like, you can use a redirect, such as `>` to send the output to a text file. Here's an example: $`ls -alRt ~/Desktop > ~/Desktop/report.txt`

Go back to the [main list of commands](index.md)
