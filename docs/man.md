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

* Special files (usually found in /dev)
* File formats and conventions eg /etc/passwd
* Miscellaneous (including macro packages and conventions), e.g. groff(7)
* System administration commands (usually only for root)
* Kernel routines [Non standard]

## Basic command structure
For all descriptions below, the dollar sign indicates that BASH command prompt.

$ `man [options] [name of command]`

## Possible Flags

### `-a`
By default, man will exit after displaying the most suitable manual page it finds.  Using this option forces man to display all the manual pages with names that match the search criteria. [Source](https://man7.org/linux/man-pages/man1/man.1.html)

### `-I`
The `-I` flag earch for manual pages case-sensitively. [Source](https://man7.org/linux/man-pages/man1/man.1.html)

### `-u`
The `-u` flag causes man to update its database caches of installed manual pages.  This is only needed in rare situations, and it is normally better to run mandb(8) instead. [Source](https://man7.org/linux/man-pages/man1/man.1.html)


## Output
The `man` command has a general output for information regarding whichever command you are searching the manual for more information on. 
