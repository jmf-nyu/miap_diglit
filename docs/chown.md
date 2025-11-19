# The chown Command

## Summary 
The `chown` command allows you to change the owner of a file or directory. The value of the Owner parameter can be a username from the user database or a numeric user ID. Optionally, a group can be specified instead of an owner.

## Basic command structure
For all descriptions below, the dollar sign indicates that BASH command prompt.

$ `chown [-f][-h][-R] Owner[:Group]{directory path}`
$ `chown -R [-f][-H|-L|-P] Owner[:Group]{directory path}`

Notes: Only the root user can change the owner of a file, and the group of a file can only be changed by a root user or owner. If you own the file but are not a root user, you can change the group only to a group of which you are a member. 

The -H, -L, and -P flags are mutually exclusive, although it will not be considered an error if multiple are specified; the command will just be determined by the last flag specified.

## Possible Flags

### `-f`
The `-f` flag suppresses all error messages except usage messages.

### `-h`
The `-h` flag changes the ownership of an encountered symbolic link and not that of the file or directory pointed to by the symbolic link. If the -h flag is not specified and a symbolic link is encountered, the chown command will change the ownership or the file or directory pointed to by the link, instead of the link itself.

### `-H`
If the -R option is specified and a symbolic link referencing a file of type directory is specified on the command line, the chown command shall change the user ID (and group ID, if specified) of the directory referenced by the symbolic link and all files in the file hierarchy below it.

### `-L`
If the -R option is specified and a symbolic link referencing a file of type directory is specified on the command line or encountered during the traversal of a file hierarchy, the chown command shall change the user ID (and group ID, if specified) of the directory referenced by the symbolic link and all files in the file hierarchy below it.

### `-P`
If the -R option is specified and a symbolic link is specified on the command line or encountered during the traversal of a file hierarchy, the chown command shall change the owner ID (and group ID, if specified) of the symbolic link if the system supports this operation. The chown command shall not follow the symbolic link to any other part of the file hierarchy.

### `-R`
If the -R flag is specified, the chown command descends the directories recursively, changing the ownership for each file. When a symbolic link is encountered and the link points to a directory, the ownership of that sirectory is changed the but directory is not further transversed. When the `-h` flag is also specified and a symbolic link is encountered, the ownership of that link is changed but not the file or directory it points to.  If the -h, -H, -L or -P flags are not also specified, when a symbolic link is encountered and the link points to a directory, the group ownership of that directory is changed but the directory is not traversed further.


## Output
The chown command doesn't produce any output upon success. 

## Examples 
* If you want to see hidden files in a nice list format run $ `ls -la ~`. The `~` would indicate your home folder.
* To get a the contents of an entire directory structure starting at a parent folder: $ `ls -alRt`. If you'd like, you can use a redirect, such as `>` to send the output to a text file. Here's an example: $ `ls -alRt ~/Desktop > ~/Desktop/report.txt`

Go back to the [main list of commands](index.md)
