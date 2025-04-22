## DevOps Lab 5 – Subversion  
[https://github.com/ShriRadhey-Mishra/Lab_5.git]

Subversion, just like git, is another Version Control System, which we can use instead of Git. Subversion is a centralized VCS unlike git which is a distributed VCS. In this lab, we performed and understood the working of some basic subversion (svn) commands such as:

- `svn checkout <repo_url>`: We use this command to check out a working copy from a remote SVN repository to our local system.  
- `svn add <file_name>`: This command is used to add new files or directories to version control in our local working copy.  
- `svn commit -m "<message>"`: After adding or modifying files, this command commits our changes to the remote SVN repository with a log message.  
- `svn update`: This command updates our local copy with the latest changes from the remote repository.  
- `svn status`: Displays the status of files in our working directory, showing which files are modified, added, or missing.  
- `svn branch` (usually via `svn copy`): Subversion doesn’t have a separate command for branching; instead, we create a branch by copying the trunk to a branch directory using:  
  `svn copy <repo_url>/trunk <repo_url>/branches/<branch_name> -m "creating branch"`  
- `svn merge`: To merge changes from a branch back to the trunk, we use:  
  `svn merge <repo_url>/branches/<branch_name>` from the trunk directory.  
- `svn resolve`: Used to resolve conflicts after a merge operation.

Using these commands, we can check out a working copy from a remote SVN repository, create or modify files, add them to version control, commit the changes to the repository, and even create and merge branches as needed.

---
