### Kernel  
* Core of OS that controls and communicates with hardware resource

---
### Shell
* Interface that allows users to communicate with kernel : bash, zsh, ...  
* Users runs applications and give commands through shell

---

### shell commands  
* pwd : shows the current path in a hierarchical directory
* cd : change directory
* ls : list files and directories
  * / : root
  * . : current directory
  * .. : upper-level directory
  * ~ : home of current user
  * /[directory name] : absolute path
  * ./[directory name] : relative path
  * ../[directory name] : relative path
  * -l : show detailed information (long format)
  * -lh : smae as above, but size in units
* clear : clears the terminal screen with the current line where the cursor is located at the top of the screen 
* cp : copy files and directories
  * cp *file1 file2* : copies the contents of *file1* into *file2*. If *file2* does not exist, it is created; **otherwise**, ***file2*** **is silently overwritten with the contents of** ***file1.***
  * cp -i *file1 file2* : Like above however, since the "-i" (interactive) option is speccified, if *file2* exists, the user is prompted before it is overwritten with the contents of *file1*
  * cp *file1 dir1* : copy the contents of *file1* (into a file named file1) inside of directory *dir1*
  * cp -R *dir1 dir2* : copy the contents of the directory *dir1*. If directory *dir2* does not exist, it is created Otherwise, it creates a directory named *dir1* within directory *dir2*
* mv : move files and directories or rename them
  * mv *file1 file2* : If *file2* does not exist, then *file1* is renamed *file2*. **If** ***file2*** **exists, its contents are silently replaced with the contents of** ***file1.***
  * mv -i *file1 file2* : Like above however, since the "-i" (interactive) option is specified, if *file2* exists, the user is prompted before it is overwritten with the contents of *file1*.
  * mv *file1 file2 dir1* : The files *file1* and *file2* are moved to directory *dir1*. If *dir1* does not exist, **mv** will exit with an error.
  * mv *dir1 dir2* : If *dir2* does not exist, then *dir1* is renamed *dir2*. If *dir2* exists, the directory *dir1* is moved within directory *dir2*.
* rm : delete files and directories ***permantely and irreversevely!!!***
  * rm *file1 file2* : Delete *file1* and *file2*.
  * rm -i *file1 file2* : Like above however, since the "-i" (interactive) option is specified, the user is prompted before each file is deleted.
  * rm -r *dir1 dir2* : Directories *dir1* and *dir2* are deleted along with all of their contents.
* mkdir : make a new directory
* Wildcards Pattern
  * \* : All filenames
  * g* : All filenames that begin with the character "g"
  * b* .txt : All filenames that begin with the character "b" and end with the characters ".txt"
  * Data??? : Any filename that begins with the characters "Data" followed by exactly 3 more characters
* Wildcards Command
  * cp *.txt text_files : Copy all files in the current working directory with names ending with the characters ".txt" to an existing directory nmaed *text_files*
  * mv dir1 ../*.bak dir2 : Move the suvdirectory *dir1* and all the files ending in ".bak" in the current working directory's parent directory to an existing directory nmaed *dir2*.
  * rm *~ : Delete all files in the current working directory that end with the character "~". Some applications create backup files using this naming scheme. Using this command will clean them out of a directory.
* help : If you use the *help command*, it will give you information about the command.
* man : Area that displays manuals for specific commands or resources.
* exit : Exiting terminal.
