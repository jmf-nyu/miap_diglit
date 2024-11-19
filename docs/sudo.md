
# The sudo Command

## Summary 
The `sudo` command allows users to run programs with the security priviledges of another user. When trusted users precede an administrative command with `sudo`, they are prompted for their password. Once authenticated and assuming the command is permitted, the administrative command is executed as if by the root user. 

## Basic command structure
The basis format of the `sudo` command is as follows. For the description below, the dollar sign indicates that BASH command prompt.

$ `sudo <command>`

Note: If the user tries to run this command without including `sudo` and does not have the necessary permissions, the host system will return a message stating that access is denied. By including `sudo`, the user can now retrieve and edit the file's contents at the privileged level.

## Possible Flags 

### `-p`
The `-p` flag uses a custom password prompt with optional escape sequences.

### `-u`
The `-u` flag is used when you want to run the command as a user other than the default target user (usually root). 

## Output
The `ls` command has many different kinds of outputs as described below:
* **Standard output** with no flags, which displays the names of directories and files within the directory where the command is run:
![screenshot of ls output](ls_no-flags.png)

* **Output with `-l` flag**, which displays directories and files in a list form with metadata in colums:
![screenshot of ls list output](ls_l-flag.png)

## Examples 
* If you want to get the lastest updates or upgrade your server, run $ `sudo apt update` and $ `sudo apt upgrade`.
* If you want to reboot your machine, run `sudo reboot`.
* To install software, run `sudo apt install <software>`.

Go back to the [main list of commands](index.md)

