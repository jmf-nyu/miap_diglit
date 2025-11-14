# The Reboot Command

## Summary 
The `reboot` command can be used to reboot a remote server.  

## Basic command structure
For all descriptions below, the dollar sign indicates that BASH command prompt.

$ `reboot [options] [directory path]`

Note: If you do not specify a directory path, running `ls` will show you the contents of the current directory you are in within your terminal window, i.e., your current working directory.

## Possible Flags


## Output
* **Standard output** with no flags, which displays the names of directories and files within the directory where the command is run:
![screenshot of ls output](ls_no-flags.png)

* **Output with `-l` flag**, which displays directories and files in a list form with metadata in colums:
![screenshot of ls list output](ls_l-flag.png)

## Examples 
* If you want to see hidden files in a nice list format run $ `ls -la ~`. The `~` would indicate your home folder.
* To get a the contents of an entire directory structure starting at a parent folder: $ `ls -alRt`. If you'd like, you can use a redirect, such as `>` to send the output to a text file. Here's an example: $ `ls -alRt ~/Desktop > ~/Desktop/report.txt`

Go back to the [main list of commands](index.md)

