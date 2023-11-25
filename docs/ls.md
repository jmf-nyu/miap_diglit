# The ls Command
Go back to the [main list of commands](index.md)

## Summary 
The `ls` command lists the contents of a directory including both files and directories. The command has many options which are described below. 

## Basic command structure
$ `ls [options] [directory path]`
The dollar sign above indicates the command prompt

## Possible Flags

### `-a`
The `-a` flag shows files that are normally hidden by BASH. These are files that begin with a `.` such as [.DS_Store](https://en.wikipedia.org/wiki/.DS_Store), [.bashrc](https://en.wikipedia.org/wiki/Bash_(Unix_shell)#Startup_scripts), or .bash_history.

### `-l`

## Output

## Examples 
* If you want to see hidden files in a nice list format run $`ls -la ~`. The `~` would indicate your home folder.
* To get a the contents of an entire directory structure starting at a parent folder: $`ls -alRt`. If you'd like, you can use a redirect, such as `>` to send the output to a text file. Here's an example $`ls -alRt > ~/Desktop/report.txt`
