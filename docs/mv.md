# The mv Command

## Summary 
The `mv` command moves files. The mv command can either rename files or move them to a different directory or location. 

## Basic command structure
For all descriptions below, the dollar sign indicates that BASH command prompt.

For renaming files: 
$ `mv [source file name] [destination file name]`

For moving file to different location 
$ `mv [source file name] [destination path]`

## Possible Flags

### `-f`
The `-f` flag makes it so you are not prompted for confirmation before overwriting the destination file. 

### `-i`
The `-i` flag 

### `-n`
When used the `-l` flag, the `-h` flag displays file size in human-readable units such as kilobytes, megabytes, and gigabytes.

## -i
The `i` command has many different kinds of outputs as described below:
* **Standard output** with no flags, which displays the names of directories and files within the directory where the command is run:
![screenshot of ls output](ls_no-flags.png)

## -v
![screenshot of ls list output](ls_l-flag.png)

## Examples 
* If you want to see hidden files in a nice list format run $`ls -la ~`. The `~` would indicate your home folder.
* To get a the contents of an entire directory structure starting at a parent folder: $`ls -alRt`. If you'd like, you can use a redirect, such as `>` to send the output to a text file. Here's an example: $`ls -alRt ~/Desktop > ~/Desktop/report.txt`

Go back to the [main list of commands](index.md)
