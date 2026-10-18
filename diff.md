# The diff Command

## Summary 
The `diff` command compares the contents of file1 and file2 and writes to the standard output the list of changes necessary to convert one file into the other.  No output is produced if the files are identical. 

## Basic command structure

 diff [OPTIONS] FILE1 FILE2

## Possible Flags

### -b
The '-b' flag causes any amount of white space at the end of a line to be treated as a single newline character (the white-space characters preceding the newline character are ignored) and other strings of white-space characters, not including newline characters, to compare equally.

### -C Lines
The '-C' flag produces a **diff** command comparison with a number of lines of copied context equal to the value specified by the Lines variable. The -C flag modifies the output slightly. The output begins with identification of the files involved and their creation dates. Each change is separated by a line with a dozen * (asterisks). The lines removed from File1 are marked with a - (minus sign ) and those added to File2 are marked with a + (plus sign). Lines changed from one file to the other are marked in both files with an ! (exclamation point). Changes that lie within the specified copied context lines of each other are grouped together as output.

### -c
The '-c' flag produces a **diff** command comparison with three lines of copied context. The -c flag modifies the output slightly. The output begins with identification of the files involved and their creation dates. Each change is separated by a line with a dozen * (asterisks). The lines removed from File1 are marked with a - (minus sign ) and those added to File2 are marked with a + (plus sign). Lines changed from one file to the other are marked in both files with an ! (exclamation point). Changes within the specified copied context lines of each other are grouped together as output.

### -D [String]
The '-D' flag causes the **diff** command to create a merged version of File1 and File2 on the standard output. The C preprocessor controls are included so that a compilation of the result without defining String is equivalent to compiling File1, while defining String yields File2.

### -e
The '-e' flag produces output in a form suitable for use with the ed editor to convert File1 to File2. When using this flag, the following shell program may help maintain multiple versions of a file. Only an ancestral file ($1) and a chain of version-to-version ed scripts ($2, $3, ...) made by the diff command need to be on hand. The latest version appears on the standard output as follows: (shift; cat $*; echo '1,$p') | ed - $1

Extra commands are added to the output when the -e flag is used to compare directories, so the result is a shell script for converting text files that are common to the two directories from their state in Directory1 to their state in Directory2.
* Note: Editing scripts produced by the -e or -f flags cannot create lines consisting of a single . (period).

### -f
The '-f' flag produces output in a form not suitable for use with the ed editor, showing the modifications necessary to convert File1 to File2 in the reverse order of that produced under the -e flag.

### -h
The '-h' flag performs an alternate comparison that may be faster if the changed sections are short and well separated. The -h flag works on files of any length. The -c, -C, -D, -e, -f, and -n flags cannot be used with the -h flag. All other flags except the -b flag are ignored when used with the -h flag.

### -i
The '-i' flag ignores the case of letters. For example, a lowercase a is treated the same as an uppercase A.

### -l
The '-l' flag is a long output format. Each result from the diff command text file comparison is piped through the pr command for pagination. Other differences are remembered and summarized after all text file differences are reported.

### -n
The '-n' flag produces output similar to that of the -e flag, but in the opposite order and with a count of changed lines on each insert or delete command. This is the form used by the revision control system (RCS).

### -r
The '-r' flag causes application of the diff command recursively to common subdirectories encountered.

### -s
The '-s' flag reports files that are the same and otherwise not mentioned.

### -S [File]
The '-S' flag ignores files whose names collate before the file specified by the File variable when comparing directories. The -S flag only applies to the directories specified in the Directory1 and Directory2 parameters. If you use the -r flag with the -S flag, the -S flag does not work recursively in the Directory1 and Directory2 subdirectories.

### -t
The '-t' flag expands tabs in output lines. Typical output or the -c flag output adds characters to the front of each line, which may affect indentation of the original source lines and makes the output listing difficult to interpret. This flag preserves the original source's indentation.

### -u
The '-u' flag produces a diff command comparison with three lines of unified context.
The output is similar to that of the -c flag, except that the context lines are not repeated; instead, the context, deleted, and added lines are shown together, interleaved.

### -U Lines
The '-U' flag produces a diff command comparison with a number of lines of unified context equal to the value specified by the Lines variable. The output is similar to that of the -C flag, except that the context lines are not repeated; instead, the context, deleted, and added lines are shown together, interleaved.

### -w
The '-w' flag ignores all spaces and tab characters and treats all other strings of blanks as equivalent. For example, if ( a == b ) compares equally to if(a==b).

## Output
The default (without -e, -c, or -n --rcs options) output contains lines
     of these forms, where XX, YY, ZZ, QQ are line numbers respective of file
     order.

     XXaYY        At (the end of) line XX of file1, append the contents of
                  line YY of file2 to make them equal.
     XXaYY,ZZ     Same as above, but append the range of lines, YY through ZZ
                  of file2 to line XX of file1.
     XXdYY        At line XX delete the line.  The value YY tells to which
                  line the change would bring file1 in line with file2.
     XX,YYdZZ     Delete the range of lines XX through YY in file1.
     XXcYY        Change the line XX in file1 to the line YY in file2.
     XX,YYcZZ     Replace the range of specified lines with the line ZZ.
     XX,YYcZZ,QQ  Replace the range XX,YY from file1 with the range ZZ,QQ from
                  file2.

     These lines resemble ed(1) subcommands to convert file1 into file2.  The
     line numbers before the action letters pertain to file1; those after
     pertain to file2.  Thus, by exchanging a for d and reading the line in
     reverse order, one can also determine how to convert file2 into file1.
     As in ed(1), identical pairs (where num1 = num2) are abbreviated as a
     single number.
## Examples 
1. To compare two files, enter:
diff chap1.back chap1

This displays the differences between the files chap1.bak and chap1.

2. To compare two files while ignoring differences in the amount of white space, enter:
diff  -w prog.c.bak prog.c

If two lines differ only in the number of spaces and tabs between words, the diff -w command considers them to be the same.

3. To create a file containing commands that the ed command can use to reconstruct one file from another, enter:
diff  -e chap2 chap2.old >new.to.old.ed

This creates a file named new.to.old.ed that contains the ed subcommands to change chap2 back into the version of the text found in chap2.old. In most cases, new.to.old.ed is a much smaller file than chap2.old. You can save disk space by deleting chap2.old, and you can reconstruct it at any time by entering:
(cat new.to.old.ed ; echo '1,$p') | ed - chap2 >chap2.old

The commands in parentheses add 1,$p to the end of the editing commands sent to the ed editor. The 1,$p causes the ed command to write the file to standard output after editing it. This modified command sequence is then piped to the ed command (| ed), and the editor reads it as standard input. The - flag causes the ed command not to display the file size and other extra information because it would be mixed with the text of chap2.old.


Go back to the [main list of commands](index.md)
