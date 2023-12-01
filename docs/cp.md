# The cp Command

## Summary 
The `cp` command stands for copy. This command is used to copy files or groups of files or directories. It creates an exact image of a file on a disk with a different file name. cp command requires at least two filenames in its arguments.

## Basic command structure
For all descriptions below, the dollar sign indicates that BASH command prompt.

$ `cp [Source_file] [Dest_file]`

Note: If the 2nd file doesn’t exist, then first it creates one, and content is copied to it. But if it existed then it is simply overwritten without any warning. So be careful when you choose the destination file name.

## Possible Flags

### `-i`
The `-i` stands for Interactive copying. With this option the system first warns the user before overwriting the destination file. cp prompts for a response, if you press y then it overwrites the file and with any other option leaves it uncopied.

### `-b`
The `-b` flag creates the backup of the destination file in the same folder with the different name and in different format. 

### `-f`
If the system is unable to open destination file for writing operation because the user doesn’t have writing permission for this file then by using `-f` option with cp command, destination file is deleted first and then copying of content is done from source to destination file.

### `-r or -R`
Copying directory structure. With this option cp command shows its recursive behavior by copying the entire directory structure recursively.  

### `-p`
With `-p` option cp preserves the following characteristics of each source file in the corresponding destination file: the time of the last data modification and the time of the last access, the ownership (only if it has permissions to do this), and the file permission-bits. 

### `*`
The star wildcard represents anything i.e., all files and directories. Suppose we have many texts documents in a directory and want to copy it to another directory, it takes lots of time if we copy files 1 by 1 or command becomes too long if specify all these file names as the argument, but by using * wildcard it becomes simple.

## Output
The `cp` command is an essential tool which is used for copying files or groups of files and directories in Unix-Like operating systems. If we talk about its syntax it takes at least two filenames in as an argument (source and destination). As mentioned, the command has three principles: copying two file names, copying one or more arguments, and copying two directory names. Then we also mention the multiple options available while using `cp` command: `-i` , `-b` , `-f“ , `-r` , `-p`. To work with easy in Unix shell for file management one should know the proper working of `cp` command. 

Go back to the [main list of commands](index.md)
