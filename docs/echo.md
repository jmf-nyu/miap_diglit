# The echo Command

## Summary 
The `echo` command displays input text to standard output. It's often used in a shell script to log status, provide feedback to users, and for debugging. By default the output is displayed in the terminal but can be redirected to a file or piped to another process.

## Basic command structure

`echo [option] [string]`

## Possible Flags

### `-n`
The `-n` flag means it will not output the trailing newline.

### `-e`
The `-e` flag is used to enable the interpretation of backslash escapes. This allows you to add additional flags in your text block to format the text output.
#### When -e is added, a variety of other sequences can be added on including:
* \t adds a horizontal tab
* \v adds a vertical tab
* \n adds a new line
<img width="627" height="40" alt="echo-e-n-option" src="https://github.com/user-attachments/assets/0942bd5b-f763-4831-8af6-8ba152d9ef30" />

#### You can also use the echo command with variables
<img width="509" height="40" alt="echo-variable" src="https://github.com/user-attachments/assets/94dcab7a-00c5-418a-ab1b-6d22025ca7de" />

## Output
The `echo` command has different options for output locations as described below:

**Output displayed in command line**
* This is the default ouput unless a different location is specified

**Output redirected into a file**
* Example: You could use the echo command to log the date you started work on a specific project.

<img width="803" height="56" alt="echo-to-file" src="https://github.com/user-attachments/assets/7a3dc2c1-fbb3-4099-8600-dfaf6c9fd167" />

These are just the simplest examples of how to use the 'echo' command, but it is a widely used and extremely versatile tool. 

Go back to the [main list of commands](index.md)
