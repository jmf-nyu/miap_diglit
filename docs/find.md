# The find command

## Summary 
The `find` command does something

## Basic command structure
For all descriptions below, the dollar sign indicates that BASH command prompt.

$ `find [path] [options] [expression]]`

Path: Where to start searching (e.g., ~/Documents).

Options: Refine your search (e.g., -type for files/directories).

Expression: Criteria like filenames or sizes.

## Possible Flags

### `-name "FILENAME"`
Finds files or directories matching FILENAME (case-sensitive)

### `-iname "FILENAME"`
Similar to -name, but case-insensitive

### `-type TYPE`
Finds files of a certain type (options below)

f: Regular file

d: Directory

l: Symbolic link

## Output
The `ls` command has many different kinds of outputs as described below:
* **Standard output** with no flags, which displays the names of directories and files within the directory where the command is run:
![screenshot of ls output](https://media.geeksforgeeks.org/wp-content/uploads/20230817192915/Screenshot-(548).png)

* **Output with `-l` flag**, which displays directories and files in a list form with metadata in colums:
![screenshot of ls list output](ls_l-flag.png)

## Examples 
* If you want to see hidden files in a nice list format run $ `ls -la ~`. The `~` would indicate your home folder.
* To get a the contents of an entire directory structure starting at a parent folder: $ `ls -alRt`. If you'd like, you can use a redirect, such as `>` to send the output to a text file. Here's an example: $ `ls -alRt ~/Desktop > ~/Desktop/report.txt`

Go back to the [main list of commands](index.md)
