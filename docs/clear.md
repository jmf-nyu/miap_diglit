# The clear Command

## Summary 
The `clear` command removes all the visible text and outputs from your current terminal window, in other words, it clears your terminal. It looks in the environment for the terminal type and then in the termini database to determine how to clear the screen.

## Basic command structure
For all descriptions below, the dollar sign indicates that BASH command prompt.

$ `clear`

Note: the 'clear' command does not delete your command history, but it erases your scrollback history. It also ignores any command line that may be present. 

## Possible Flags

### `-x`
The `-x` flag clears the visible screen but does not clear the scrollback buffer. This allows you to keep your terminal history by scrolling up or pressing Page Up. 

### `-T type`
The `-T type` flag specifies the specific terminal type instead of using the environment variable. (`TERM` `LINES``COLUMNS`)

### `-V`
The  `V` flag reports the version of `ncurses` associated with the program being used by clear.

## Output
The `clear` command has many different kinds of outputs as described below:
* **Standard output** with no flags, which clears the visible text on the terminal screen:
![screenshot of clear output](clearcommandscreenshot.png)


## Examples 
* If you want to clean up your window and 'start over,' `clear` is a useful command for de-cluttering your workspace.

Go back to the [main list of commands](index.md)
