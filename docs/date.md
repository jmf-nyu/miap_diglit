# The date command

## Summary 
The `date` command sets and shows the system date and time. 

## Basic command structure 
For all descriptions below, the dollar sign indicates that BASH command prompt.

$ `date [options] [+format]`

Note: If no option or format is given then the 'date' command will print the current locale's date and time. 

## Possible Flags 

### `-d` 
The `-d` flag displays the given date/time string. The date displayed can be given as a word: today, yesterday, etc. or as a phrase: "Jan 12 2012" 
<img width="343" height="58" alt="Screenshot 2025-11-18 at 8 53 05 PM" src="https://github.com/user-attachments/assets/7ced446b-239d-4532-9010-c9edc9d360b7" />


### `-r` 
The `-r` flag displays the time when a specified file was last modified. Use the filename or path/to/filename.
<img width="489" height="74" alt="Screenshot 2025-11-18 at 9 09 09 PM" src="https://github.com/user-attachments/assets/c66d87c2-1203-4e48-bf54-c4a8b5793251" />

### `-s`
The `-s` flag sets the system date and time. That being so, it also requires superuser privileges. Use "YYYY-MM-dd HH:MM:SS" 

### `-u`
The `-u` flag shows the date/time in UTC instead of the local timezone. 

## Output options 
The `date` command has many different kinds of outputs as described below:
* **Standard output** with no flags or +formats, which displays the local date and time of the system.

* **Output** with `-r` gives the last modification date of a file within the directory.

* **Output** with `[+format]` adjusts what part of the time or date is displayed. For example `+%Y` outputs the year (YYYY), `+%m` outputs the month (MM), and `%d` (dd) outputs the day. 
<img width="262" height="92" alt="Screenshot 2025-11-18 at 9 51 58 PM" src="https://github.com/user-attachments/assets/c45ab0b0-e702-4f76-a6b6-cc844270b14b" />

## Examples
* If you wanted to check the last modification date of a file, but in the MM/DD/YY format run $ `date -r path/to/filename +%D`.
* If you want to see the time as the 12-hour format, as opposed to the standard use of 24 hours, run $ `date +"%I %p"`.

Go back to the [main list of commands](index.md)
