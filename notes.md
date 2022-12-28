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

    info on all commits. press "q" to exit scrolled log.
    using this we can also see on which branch we work on. (HEAD -> branchName).
    when having many changes, easier to see log via "git log --oneline" to collapse all into one liners
	
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

Difference between files:

    "git diff" will show the difference between files if there are any

Resetting back to an old version:

    "git reset id" will return the changes to an older commit.
    obtain the necessary id using the git log command.

Branches, Merging & Deleting:

    Moving between branches:
    "git branch" will show us all branches in the project.
    "git switch -c NAME" will copy the current branch into a new branch with the new name. History of the old branch will also be copied.

    Merging:
    "git merge branchName" will merge changes from the specified branchName INTO the current branch.
    so to use it, we will usually switch back to the main branch, and then use the command with the name of the other branch to merge into.

    Deleting a branch:
    "git branch --delete NAME" will delete the branch provided.

Git FLOW:
    
    1. Create new branch for a feature or a fix.
    2. Make changes on the new branch
    3. Merge changes into master
    4. Delete old branch