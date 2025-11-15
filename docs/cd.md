# The cd Command

## Summary 
The `cd` command allows you to move between directories. Also known as `chdir` (change directory), is a command-line shell command used to change the current working directory in various operating systems. The cd command takes an argument, usually the name of the folder you want to move to. `cd` is frequently included built directly into a command-line interpreter.

## Basic command structure
For all descriptions below, the dollar sign indicates that BASH command prompt.

$ `cd [directory path]`

Note: If you do not specify a directory path, running `cd` will land you on your home directory. 

## Possible arguments

### `/`
The `/` argument can change the directory to the root directory. The root directory is the first directory in your filesystem hierarchy. 
![screenshot of cd](cd.png).
Above, / represents the root directory.
#### How to move inside a directory from a directory
This command is used to move inside a directory from a directory. 
$ `cd dir_1/dir_2/dir_3`
Here, replace “dir_1/dir_2/dir_3” with your sub directory name or location you want to move in. For example:
![screenshot of cd1](cd1.png)

### `~`
The `~` is used in `cd` command to change the directory to the home directory from any location in Linux System.

### `..`
When used the `..` argument in `cd` command which is used to move to the parent directory of current directory, or the directory one level up from the current directory. “..” represents parent directory.


## Examples 
* You can also use `\` this in between if you don’t want to use double or single quotes.
`cd /users/jprincipesalazar/Documents/MIAP/Digital\literacy`
![example 01](cd_example.png)

Go back to the [main list of commands](index.md)
