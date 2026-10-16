# The kill Command

## Summary 
The `kill` command sends a signal to terminate a process by specifying its PID (process ID), which you can find with the command `ps`. 

## Basic command structure
For all descriptions below, the dollar sign indicates that ZSH command prompt.

$ `kill [options] PID`

Note: PIDs are numerical values that are assigned automatically, when running the `ps` command in terminal, the PID appears in the first column. That numerical value can then be used in the `kill`. 

## Possible Options
### `-9`
The `-9` flag causes a force kill, a command that cannot be ignored by the process.

### `-STOP`
The `-STOP` flag freezes a process in place, causing it to stop any CPU use.

### `-CONT`
The `-CONT` flag continues a frozen process, causing it to resume.


## Examples 
<img width="481" height="114" alt="Screenshot 2026-10-15 at 8 31 57 PM" src="https://github.com/user-attachments/assets/acf2c2af-71c9-455b-a644-59ede28cca15" />


Go back to the [main list of commands](index.md)
