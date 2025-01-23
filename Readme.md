# Git Commands Explained

This guide provides a quick reference to some essential Git commands.

## Initializing a Git Repository

* `git init`: Creates a new Git repository in the current directory.

## Listing Files

* `git ls`: Lists all files tracked by Git in the current repository.

## Viewing Commit History

* `git log`: Displays the commit history, including commit messages and IDs.

## Examining Commit Details

* `git show <commit_id>`: Shows detailed information about a specific commit, including the commit message, author, date, and code changes.

## Renaming Files

* `git mv <old_filename> <new_filename>`: Renames a file tracked by Git. 
**Note:** The file must be staged before using this command.

## Removing Files

* `git rm <filename>`: Removes a file from the Git repository. 
**Note:** The file must be staged and committed before using this command.

## Resetting to a Specific Commit

* `git reset --hard <commit_id>`: Discards all local changes made after the specified commit and resets the working directory to match that commit.
* `git reset --soft <commit_id>`: Moves the HEAD pointer to the specified commit but keeps the working directory unchanged.

## Creating Git Aliases

* `git config --global alias.<alias_name> "<git_command>"`: Creates a custom alias for a frequently used Git command. You can then use the alias instead of the full command.

## Branching and Merging

* `git checkout -b <branch_name>`: Creates a new branch named `<branch_name>` and switches to that branch.
* `git branch`: Lists all branches in the current repository and indicates the currently active branch.
* `git merge <branch_name>`: Merges the changes from the specified branch (`<branch_name>`) into the current branch.

## Deleting Branches

* `git branch -d <branch_name>`: Deletes the specified branch (`<branch_name>`).

## Creating Annotated Tags

* `git tag -a <tag_name> -m "<message>"`: Creates an annotated tag named `<tag_name>` with the provided message (`<message>`).

## Pulling Changes

* `git pull`: Downloads the latest changes from the remote repository and merges them into the current branch. This is equivalent to running `git fetch` followed by `git merge`.

## Changing the Remote Repository URL

* `git remote set-url origin <new_url>`: Updates the URL for the remote repository named "origin" to the new URL provided (`<new_url>`).

## Viewing Remote Repository URL

* `git remote -v`: Displays information about the configured remote repositories, including their URLs.

## Stashing Changes

* `git stash`: Temporarily saves uncommitted changes in the working directory and working tree, leaving the working directory clean. This is useful when you need to switch branches or make a quick fix but don't want to commit your current changes yet.
* `git stash pop`: Restores the most recently stashed changes and removes them from the stash list.
* `git stash list`: Lists all stashed changes.
* `git stash apply`: Applies the most recently stashed changes without removing them from the stash list.
