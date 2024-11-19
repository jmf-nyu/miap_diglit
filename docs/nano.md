# The Nano Command

## Summary 
`nano` is a simple terminal-based text editor. Though not as powerful as Emacs or Vim, it is easy to learn and use. Nano is ideal for making small changes to existing configuration files or for writing short plain text files. It was originally created as a free replacement for the non-free Pico editor. 

## How to use it 
To start nano with an empty file, open a terminal window and at the command-line type `nano`
To open an existing file for editing, type `nano [directory path/file_name.ext]` where file_name.ext is the name of the existing file. For example, to open the file that contains the list of most recently issued commands, make sure you are in your home directory, and at the command line type `nano .bash_history`

A screenshot of the results of `nano .bash_history`:
![Screenshot 2024-11-18 at 8 39 18 PM](https://github.com/user-attachments/assets/6eca5b5d-2889-4539-a92a-06de5b9580fa)


## Editing Text
As is normal in most text editors, text that you type into nano is inserted at the current cursor position. The Delete and Backspace keys also work the same as in other editors. Unlike elsewhere in command line, typing in `nano` works similar to typing in a regular document. 


## Quitting Nano
To quit `nano`, use the Ctrl+X key combination. If the file you are working on has been modified since the last time you saved it, you will be prompted to save the file first. Type y to save the file, or n to exit without saving the file.
