#Review of Git Commands from Chapter 5

###Git Clone: Clones (copies) a git repository into the file (directory) you are currently in.
###*Git init *directory name*: creates a new repository

###Tracking Files

####Git Status: shows what branch you are on in the repository, lists any files that are staged but not committed, lists untracked files
####Git add: Starts tracking a file
####- Git add will also stage changes made to a file already being tracked.
####- Git commit -m "message" will commit changes you have made.  The message can explain what those changes are.
####-Can also use Git commit -a: commit all changed files.
- be carefule using this command if you have changes in files you aren't ready to push to your repository yet.

###Git commit
####This command shows you the differences between the file in your directory and what's being staged.

### Git Log: will list the chain of commits for a file

###To move or remove files that are being tracked, use Git mv or Git rm

###Gitignore tells git to ignore certain files that are untracked and you typically do not plan to track them.
- This can include large files, intermediate files, and temporary files

###Git reset will undo a stage if you decide you don't want to stage your changes.

###THIS IS ONLY THE BEGINNING!!!


