# The man Command

## Summary 
The `man` command in Linux is used to display the user manual of any command that we can run on
the terminal. It provides a detailed view of the command which includes NAME, SYNOPSIS,
DESCRIPTION, OPTIONS, EXIT STATUS, RETURN VALUES, ERRORS, FILES, VERSIONS, EXAMPLES,
AUTHORS and SEE ALSO. See [this guide](https://www.nielit.gov.in/gorakhpur/sites/default/files/Gorakhpur/Alevel_unix_27april20_AKM.pdf) for more information.

Every manual is divided into the following sections:

* Executable programs or shell commands
* System calls (functions provided by the kernel)
* Library calls (functions within program libraries
* Games

Special files (usually found in /dev)
File formats and conventions eg /etc/passwd
Miscellaneous (including macro packages and conventions), e.g. groff(7)
System administration commands (usually only for root)
Kernel routines [Non standard]

## Basic command structure
For all descriptions below, the dollar sign indicates that BASH command prompt.

$ `man [options] [name of command]`

## Possible Flags

### `-a`
The `-a` flag helps users search and skips to current screen. This option helps us to display all the available intro manual pages in succession.
See: 
https://www.geeksforgeeks.org/man-command-in-linux-with-examples/

### `-?`
The `-?` flag  displays help (from command line).
See: Terminal


## Output
The `man` command has a general output for information regarding whichever command you are searching the manual for more information on. 
