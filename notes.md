Inside IDE Terminal:

Terminal -> "git init"

    this will change files color inside IDE and means git now manages the project    
    This created an invisible ".git" folder that manages all the information


Terminal -> "git add filename"

    add files to "staging" environment. we add files we want to commit later
    "git add --all" will add all files in the folder
	
Terminal -> "git commit -m "message""

    This sends all the files we added with a message of what we did
	
Terminal -> "git log"

    info on all commits.
    using this we can also see on which branch we work on. (HEAD -> branchName).
	
Terminal -> "git status"

    Info on current files, what files are tracked, what arent, what has been modified so far and hasn't been added.
	
Terminal -> "git restore ."

	restores the files back to the last commit

Colors:
   
    grey - synced (Commited)
    Red - Modified
    green - comitted, waiting for commit

Ignoring files:

    Files can be ignored, such as settings, TO DO list, system files etc
    using ".gitignore"

Deleting files:

    Can delete manually via the IDE, but must add & commit afterwards.
    Can also use "git rm filename" to remove a file using git terminal and automatically add it to staging.

Rename files:

    Can manually rename the file via the IDE. Git however will log 2 actions: Deletion and then creating new file with that name.
    can also use "git mv oldName newName"