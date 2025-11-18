# The chown Command

## Summary 
The `chown` command allows you to change the owner of a file or directory. The value of the Owner parameter can be a username from the user database or a numeric user ID. Optionally, a group can be specified instead of an owner.

## Basic command structure
For all descriptions below, the dollar sign indicates that BASH command prompt.

$ `chown [-f][-h][-R] Owner[:Group]{directory path}`
$ `chown -R [-f][-H|-L|-P] Owner[:Group]{directory path}`

Note: 

## Possible Flags

### `-f`
The `-f` flag 

### `-h`
The `-l` flag gives a column view of files and directories. It also gives information about those files and directories including permissions, last date modified and size.

### `-R`
When used in combination with the `-l` flag, the `-h` flag displays file size in human-readable units such as kilobytes, megabytes, and gigabytes.

Although the 

## Output
The `ls` command has many different kinds of outputs as described below:
* **Standard output** with no flags, which displays the names of directories and files within the directory where the command is run:
![screenshot of ls output](ls_no-flags.png)

* **Output with `-l` flag**, which displays directories and files in a list form with metadata in colums:
![screenshot of ls list output](ls_l-flag.png)

## Examples 
* If you want to see hidden files in a nice list format run $ `ls -la ~`. The `~` would indicate your home folder.
* To get a the contents of an entire directory structure starting at a parent folder: $ `ls -alRt`. If you'd like, you can use a redirect, such as `>` to send the output to a text file. Here's an example: $ `ls -alRt ~/Desktop > ~/Desktop/report.txt`

Go back to the [main list of commands](index.md)
