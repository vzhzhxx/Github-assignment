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


Added questions:

Write the difference between fetch and pull command.
Fetch command is used to get data from remote projects. Git Fetch tells the local repository that there are changes available in the remote repository without beinging changes in local repository. The syntax is: git fetch.
To bring the changes to the remote repository, git pull command is used. The syntax is : git pull origin branch
_name.


How to handle merge conflicts?
Merge conflicts occur when different branches of a project is made to add certain features. When merging branches, conflict arises when different branches are at working with different objectives.To handle this, confllicts are handled manually. This can be done by using 'git add' command or using Pull requests that makes sure your feature is pushed. 