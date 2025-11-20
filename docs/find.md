# The find command

## Summary 
The `find` finds files. By default, it outputs their path relative to where you ran find. But, in addition of providing you with advanced “filters” it actually allows you to run commands on each of those files.

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
The `find` command has many different kinds of options as described below:
* **Standard output with no file path** When you don't specify the file path, add a `.` to the beginning of the command
![screenshot of find output](https://media.geeksforgeeks.org/wp-content/uploads/20230817192915/Screenshot-(548).png)


## Examples 
* If you want to see hidden files in a nice list format run $ `ls -la ~`. The `~` would indicate your home folder.
* To get a the contents of an entire directory structure starting at a parent folder: $ `ls -alRt`. If you'd like, you can use a redirect, such as `>` to send the output to a text file. Here's an example: $ `ls -alRt ~/Desktop > ~/Desktop/report.txt`

Go back to the [main list of commands](index.md)
