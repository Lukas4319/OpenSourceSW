### Version Control and Collaboration
* It's essential to use a version control system for software development and other documentation works.
* Basic solution : Making copies
* We need a systematic management system for version control and collaboration.
#### change VS snapshots
* change : Storing data as changes to the base version
* snapshots : Storing data as snapshots
---
### Git config : First-time setup
1. System level : --system option. Affects all uses and repositories on the system (administrative) *(file: /etc/gitconfig)*
2. Global (user) level: --global option. Affects all repositories of a current user *(file: ~/.config/git/config)*
3. Local level: --local option. Specific to the current repository *(file: .git/gitconfig)*
* Each level overrides values in the previous level: system -> global -> local
---
### git command
* $ git init : Initializing a Repository in an Existing Directory
* $ git status : Checking Repository Status
* $ git add [file_name] : Adding a new file to be staged (tracked)
  *  Tip : If there is a problem on nano (in Windows), you can edit the file in any other text editor
* $ git add . : Adding all files to be staged (tracked)
* $ git rm --cached [file_name] : Unstaging a file
* .gitignore : Ignoring a file
  * .a : ignore all .a file
  * !lib.a : but do track lib.a even though you're ignoring .a files above
  * /TODO : only ignore the TODO file in the current directory, not suvdir/TODO
  * build/ : ignore all files in any directory named build
  * doc/*.txt : ignore doc/notes.txt, but not doc/server/arch.txt
  * doc/**/*.pdf : ignore all .pdf files in the doc/ directory and any of its subdirectories
    * Tip : If there is a problem on nano (in Windows), you can edit the file in any other text editor
* $ git commit -m “commit message” : Commit
* $ git branch, $ git branch -m master main : Change branch name
