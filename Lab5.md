### Standard Output
* By default, standard output is screen.
* Redirect output using ">" after a command (e.g.,ls) to create and sace the output in a file
* Command "cat" displays the content of a text file.
* Using ">>" appends output to an extising file (if it already exitsts), or create and write to a new file if it doesn't exist.
---
### Standard Input
* By default, standard input is from keyboard.
* Redirect input from a file using "<"
* Mix "<" and ">" together in a single line.
---
### Pipelines "|"
* Pipeline feeds output of previous command to input of next command.
* command1 | command2 | command3 | ...
---
### Expansion
* Special characters expand its meaning when given to shell commands.
  *  echo : Used to print given text to the screen
  *  echo * : Print all files in the current working directory
  *  echo ~ : Shows the current user's home directory address.
---
### Backslash
* Backslash can be used to ignore line change in command ("enter"), to enter a long command in multiple lines.
---
### Permissions
* Linux is multi-user system.
* Files and directories have a permission assigned differently to owner / group / others.
  * File type
      * \- : indicates regular file
      * d : indicates directory
  * Read, write, and execute permissions for the file owner.
  * Read, write, and execute permissions for the group owner of the file.
  * Read, write, and execute permissions for all other users.
#### changing Permissions
* "chmod" changes permissions.
    * Value 777 : **(rwxrwxrwx)** No restrictions on permissions. Anybody may do anything. Generally not a desirable setting.
    * Value 755 : **(rwxr-xr-x)** The file's owner may read, write, and execute the file. All others may read and execute the file. This setting is common for programs that are used by all users.
    * Value 700 : **(rwx------)** The file's owner may read, write, and execute the file. Nobody else has any rights. This setting is useful for programs that only the owner may use and must be kept private from others.
    * Value 666 : **(rw-rw-rw)** All users may read and write the file.
    * Value 644 : **(rw-r--r--)** The owner may read and write a file, while all others may only read the file. A common setting for data files that ecerybody may read, but only the owner may change.
    * Value 600 : **(rw------)** The owner may read and write a file. All others have no rights. A common setting for data files that the owner wants to keep private.
* Change the permission of a file “word.txt” that only the owner (you) can read and write, but all the others (including others in the group) can only read it. No execution is needed for all users.
---
### Superuser
* A superuser has all system administation authority
* Some commands need superuser’s privilleges.
* Put “sudo” before the command if you are a superuser.
* Type “exit” to get out of a superuser session.
---
### Text Editors
* ***vi, vim*** : The granddaddy of Unix text editors, **vi**, is infamous for its obtuse user interface. On the bright side, **vi** is powerful, lightweight, and fast. Learning **vi** is a Unix rite of passage, since it is universally available on Unix-like systems. On most Linux distributions, an enhanced version of **vi** called **vim** is provided in place of vi. **vim** is a remarkable editor and well worth taking the time to learn it. (**Interface** : command line)
* **Emacs** : The true giant in the world of text editors is Emacs originally written by ***Richard Stallman.*** Emacs contains (or can be made to contain) every feature ever conceived of for a text editor. It should be noted that **vi** and Emacs fans fight better religious wars over which is better. (**Interface** : command line)
* ***nano*** : **nano** is a free clone of the text editor supplied with the **pine** email program. **nano** is very easy to use but is very short on features compared to **vim** and **emacs. nano** is recommended for first-time users who need a command line editor. (**Interface** : command line)
* [**gedit**] : **gedit** is the editor supplied with the GNOME desktop environment. gedit is easy to use and contanis enough features to be a good beginners-level editor. (**Interface** : graphical)
* **kwrite** : **kwrite** is the "advanced editor" supplied with KDE. It has syntax highlighting, a helpful feature for programmers and script writers. (**Interface** : graphical)
---
### Shell Script
* Write and run a shell script.
* **Tip** : If there is a problem on nano (in Windows), you can edit the file in any other text editor(e.g., notepad)
---
### command
#### History
* Type "history" to see previous command history. Or, save it to a text file.
#### wget
* download files from the internet directly to your active directory
#### curl
* fetching, uploading, and managing data over the Internet (curl \[options] \[URL])
#### grep
* 'grep' (Global Regular Expression Print) for searching text within files.
* grep "search_term" file.txt
  * Searches for the exact "search_term" within "file.txt" and prints matching lines.
* **Common Options**
  * '-i': Case-insensitive search (finds "apple" and "Apple").
  * '-v': Invert the match (finds lines *not* containing the search term).
  * '-n': Display line numbers along with matching lines.
  * '-r': Recursive search (searches through all files in a directory and its subdirectories).
* 'grep' supports powerful regular expressions for more complex searches.
  *  '.*' : Matches any character ('.') zero or more times ('*').
  *  '\d': Matches any digit (0-9).
  *  '[abc]' : Matches any single character within the brackets.
  *  '^' : Matches the beginning of a line.
  *  '$': Matches the end of a line.

