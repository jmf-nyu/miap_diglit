# Redirects - WIP

## Summary 
Redirection assists in redirecting input & output functionalities to the files or folders we want. There are 2 types of redirection:

*1. Overwrite Redirection*

The `>` command

> This will store/save the output of a command to a file & overwrite existing content of that file.

The `<` command

> Redirects input from a file to a command

*2. Append Redirection*

The `>>` command 

>This will redirect the standard output of a command on the left of `>>` & append it to the end of the file on the right of `>>`. 
> This will not compromise the existing data of the file it is added to.


The `<<` command

> Redirects input from a file to a command, appends.

## Basic command structure
For all descriptions below, the dollar sign indicates that BASH command prompt.

$ `[command] > [file name]` 

$ `[command] >> [file name]`


## Output
The `ls` command has many different kinds of outputs as described below:
* **Standard output** with no flags, which displays the names of directories and files within the directory where the command is run:
![screenshot of ls output](ls_no-flags.png)

* **Output with `-l` flag**, which displays directories and files in a list form with metadata in colums:
![screenshot of ls list output](ls_l-flag.png)

## Examples 
* To get a the contents of an entire directory structure starting at a parent folder: $`ls -alRt`. If you'd like, you can use a redirect, such as `>` to send the output to a text file. Here's an example: $`ls -alRt ~/Desktop > ~/Desktop/report.txt`

Go back to the [main list of commands](index.md)
