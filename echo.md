# The echo Command

## Summary 
The `echo` command displays input text to standard output. It's often used in a shell script to log status, provide feedback to users, and for debugging. By default theoutput is displayed in the terminal but can be redirected to a file or piped to another process. The command has many options which are described below. 

## Basic command structure
For all descriptions below, the dollar sign indicates that BASH command prompt.

$ `echo [option] [string]`

## Possible Flags

### `-n`
The `-n` flag means it will not output the trailing newline.

### `-e`
The `-e` flag is used to enable the interpretation of backslash escapes. This allows you to add additional flags in your text block to format the text output.
When -e is added, a variety of other sequences can be added on including:
\t adds a horizontal tab
\v adds a vertical tab
\n adds a new line


### `-h`
When used in combination with the `-l` flag, the `-h` flag displays file size in human-readable units such as kilobytes, megabytes, and gigabytes.

## Output
The `echo` command has many different kinds of outputs as described below:

**Output displayed in command line**


**Output piped into a file**
* **Standard output* with no flags, which displays the names of directories and files within the directory where the command is run:
![screenshot of ls output](ls_no-flags.png)

* **Output with `-l` flag*, which displays directories and files in a list form with metadata in colums:
![screenshot of ls list output](ls_l-flag.png)

## Examples 
* If you were working in an archive, you could use the echo command to log the date you started work on a specific project.

<img width="803" height="56" alt="echo-to-file" src="https://github.com/user-attachments/assets/7a3dc2c1-fbb3-4099-8600-dfaf6c9fd167" />

 
* To get a the contents of an entire directory structure starting at a parent folder: $ `ls -alRt`. If you'd like, you can use a redirect, such as `>` to send the output to a text file. Here's an example: $ `ls -alRt ~/Desktop > ~/Desktop/report.txt`

Go back to the [main list of commands](index.md)
