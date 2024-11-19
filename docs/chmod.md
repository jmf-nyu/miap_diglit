#chmod
##Summary
The chmod command is used to change the access permissions and special mode flags of files and directories. Only the file owner or a superuser can use the chmod command. 

##Basic command structure 
$ sudo chmod [options] mode[,mode] file1 [file2…]
To change the root folder permissions in our Omeka setup, we ran the following command: 
```
$ sudo chmod -R 755 /var/www/html/omeka/
```

##Options
Options that are typically used include:
```
-R
```
Recursive, which will include objects in subdirectories. This option must be input as a capital R to work as intended.
```
-v
```
Verbose, which shows changed objects (and doesn’t show unchanged objects)

##Modes
Modes specify the read, write, and execute access, respectively for the three classes of user, group, and others. This is represented as a numerical value, typically either 3 or 4 characters in length. A mode of 755 is typical, and will make a file readable and executable by all three user groups, and writable by the owner only.

##Output
This command does not output a message. The ls or stat command would need to be used in order to show that the changes were made and saved correctly. To check if the change of the root folder permissions worked as intended in our Omeka setup, the following command would be run: 
```
ls -l /var/www/html/omeka/
```
