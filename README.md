Can we have a global .gitignore?
Yes, we can have a global .gitignore that consists rhe losr of files that is ignored by all repos. Examples are files with sensitive information such as credentials, dependencies, log files, etc.


How to find difference between two commits?
In order to know the difference between two commits, 'git diff' is used. Command SHAs of both the commits are mentioned in the command like such: git diff SHA1 SHA2


Write difference between git add and git commit commands.
Git add and git commit commands have very different functionalities.
The main difference is that 'git add' command changes the working directory to staging area and the staging area becomes git repository by using 'git commit'. The changes made in the staging area are not reflected in the git repository until 'git commit' is done. Staging area is used for staging and reviewing the changes. 
Since Git uses version control system, commit can be reverted using 'git revert' command.


How to unstage files?
In order to unstage a file, 'git reset' or 'git restore' commands are used. These commands will take file from staging area to working directory. Unstaging file will not discard any changes made however. 


How to revert a commit?
Commit can be reverted using 'git revert' command. For reverting a command, commit SHA(Short Hash Algorithm) is required. SHA of a commit can be discovered using the 'git log' command. The command for reverting command is- git revert SHA.


Difference between revert and reset.
Git revert and reset are commands used to undo changes to a file, but works differently. Resetting is a way to move the current tip of a branch to a previous commit. Reverting undoes a commit by creating a new one. This makes it safe for undoing changes. This is useful if an unexpected bug is introduced or the change wasn't needed.
