## What is Version Control?

> Version Control is a system that records and manages changes to files over time. It allows multiple people to collaborate on a project by keeping track of modifications made to the files, providing a history of changes, and enabling the ability to revert to previous versions if needed. Version control systems also facilitate branching, merging, and concurrent work on different parts of the project.

## What is cloning in Git?

> In the context of Git, cloning refers to the process of creating a copy of a repository from a remote source, such as a Git server or another local repository. The clone command in Git allows you to fetch the entire repository, including all its files, commit history, and branches, onto your local machine. This enables you to work on the project independently and synchronize changes with the remote repository when necessary.

## What is the command to track and stage files?

> The command to track and stage files in Git is git add. This command is used to add files to the staging area, which is a preparatory step before committing changes. By staging files, you are indicating that you want to include them in the next commit. For example, git add filename.txt would add the file named "filename.txt" to the staging area.

## What is the command to take a snapshot of your changed files?

> To take a snapshot of your changed files in Git, you use the command git commit. This command creates a new commit with a unique identifier that represents a snapshot of the changes you have staged. When executing git commit, you typically provide a commit message that describes the changes made. For example, git commit -m "Added new feature" would create a commit with the message "Added new feature."

## What is the command to send your changed files to Github?

**git add .** : This command stages all the modified and new files in the current directory and its subdirectories.

**git commit -m** "Commit message": This command creates a commit with a message describing the changes made.

**git push origin branch-name:** This command sends the committed changes to the remote repository, specifically to the branch named "branch-name." The "origin" refers to the remote repository's name, such as the GitHub repository you want to push to.







