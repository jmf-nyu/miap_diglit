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
The `-i` flag prompts confirmation before moving a file or directory to an existing path name. 

### `-v`
The `-v` flag is to make the output verbose, printing the names and destinations of files after they are moved. 

## Output


## Examples 
* If you want to see hidden files in a nice list format run $`ls -la ~`. The `~` would indicate your home folder.
* To get a the contents of an entire directory structure starting at a parent folder: $`ls -alRt`. If you'd like, you can use a redirect, such as `>` to send the output to a text file. Here's an example: $`ls -alRt ~/Desktop > ~/Desktop/report.txt`

Go back to the [main list of commands](index.md)
