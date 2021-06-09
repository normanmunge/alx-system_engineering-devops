# alx-system_engineering-devopS - shell_basics
The files are number from 0-14 and 100-104 for additional commands and tricks. This file explains all the commands numerically for reference. 
Note that all contents in the subsequent directories are executable.

These are just few examples of common bash commands that are used in shells to manipulate files or directories. There might be simpler commands or other ways to execute the same. 

0. `0-current_working_directory` - Shows absolute path of current working directory. (pwd)

1. `1-listit` - Display the contents list of your current directory. (ls)

2. `2-bring_me_home` - Returns a user to the home directory from a working directory. (cd)

3. `3-listfiles` - Displays current directory contents in a long format. (ls -l)

4. `4-listmorefiles` - Displays current directory contents including hidden files in a long format. (ls -la)

5. `5-listfilesdigitonly` - Displays current directory contents with users and group ids numerically including hidden files. (ls -lav). An alternative to this is (ls -lan)

6. `6-firstdirectory` - Creates a directory named `holberton` in the `/tmp/` directory. (mkdir /tmp/holberton)

7. `7-movethatfile` - Moves/Renames the file `betty` from `/tmp/` to `/tmp/holberton`. (mv /tmp/betty /tmp/holberton) 

8. `8-firstdelete` - Deletes the file betty. (rm betty)

9. `9-firstdirdeletion` - Delete the directory `holberton` that is in the `/tmp` directory. (rm -rf /tmp/holberton)

10. `10-back` - Changes the working directory to the previous directory. ( cd - )

11. `11-lists` - lists all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory and the /boot directory (in this order), in long format. ( ls ./ ../ /boot)

NB: `Boot` Directory holds files used in booting the operating system. Be careful not to delete this directory.

12. `12-file_type` - Prints the type of the file named `iamafile` in the `tmp` folder. ( file /tmp/iamafile )

13. `13-symbolic_link` - Create a `symbolic link` to `/bin/ls`, named `__ls__` from a working directory ( ln -s /bin/ls __ls__ ) 

NB: A symbolic link is a term for a file that contains reference to another file or directory in the form of an absolute or relative path. ie ( ln -s soucefile filetolink )

14. `14-copy_html` - Copies all the HTML files from the current working directory to the parent of the working directory, but only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory. ( cp -un *.html ../ ) 
NB: The cp -n ( Do not overwrite existing files) cp -u (Copies non-existent files)

15. `100-lets_move` - Moves all files beginning with an uppercase letter to the directory /tmp/u. ( mv [[:upper:]]* /tmp/u )

16. `101-clean_emacs` - Deletes all files in the current working directory that end with the character ~ (rm -rf *[~]* )

17. `102-tree` - Creates the directories welcome/, welcome/to/ and welcome/to/holberton in the current directory in a tree like format ( mkdir welcome/to/holberton)

18. `103-commas` - lists all the files and directories of the current directory, separated by commas (,). Directory names should end with a slash (/) Files and directories starting with a dot (.) should be listed. The listing should be alpha ordered, except for the directories . and .. which should be listed at the very beginning. Only digits and letters are used to sort; Digits should come first. You can assume that all the files we will test with will have at least one letter or one digit. The listing should end with a new line ( ls -amp )

NB: ls -m ( List files & directories separated by commas), ls -p (Adds a trailing slash / to directories)

19. `holberton.mgc` - Create a magic file holberton.mgc that can be used with the command file to detect Holberton data files. Holberton data files always contain the string HOLBERTON at offset 0. ( magic type string/CT "Holberton" )
NB: Magic file identifies the type of a binary file. It contains lines that describe magic numbers which identify particular type of files. 




   
