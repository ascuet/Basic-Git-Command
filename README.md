# Basic-Git-Command
**Basic Git Command for Beginners**

$ git config --global user.name <your-name>
$ git config --global user.email <your-email>

$ git config --local user.name <your-name>
$ git config --local user.email <your-email>

# Show
$ git branch                                 # Show all local branches
$ git branch -r                              # Show all the remote branch
$ git branch -av                             # Show all local and remote branches

# Create
$ git branch <branch-name>                   # Create a new branch
$ git checkout -b <branch-name>              # Create & checkout to new branch
$ git checkout --orphan <branch-name>        # Create a branch with no commit list

# Push
$ git push origin <branchname>               # Push to remote branch

# Delete
$ git branch -d <branchname>                 # Delete the local branch, show a warning
$ git branch -D <branhcname>                 # Force to delete branch
$ git remote prune origin                    # Cleanup remote deleted branch

$ git add .                                                               
$ git add --all                                     # Add all changes     

# Commit                                                                          
$ git commit -am 'commit message'                   # Add & commit        
$ git commit --allow-empty -m k3;                   # Commit empty change
$ git cherry-pick <commit-hash>                     # Take a commit change of another branch 

# Amend
$ git add task2.txt                                 # Add any file
$ git commit --amend -m 'new message'               # Merge current change to previous commit and will also change the commit hash

# Pull
$ git pull origin <branch-1>                        # Pull the change of 'branhc-1' in current branch 

# Push
$ git push origin <branchame>                       # Push a branch
$ git push -f origin <branch-name>                  # Overwrite remote branch (by force)

# Merge
$ git merge origin <branch-1>                       # Merge remote 'branch-1' with current branch
$ git mergetool
$ git merge --squash <privateFeatureBranch>

# Set local folder to response remote url
git remote set-url origin git@XXXXXXXXXXXX

$ git checkout <commit-hash>               # Go to a specific commit
$ git checkout <branch-name>               # Return to present state
$ git checkout <commit-hash> <file-name>   # Only a file will go back to specific commit
$ git checkout <branch-name> -f            # Return to persent state by force
$ git checkout -- <filename1> <filename2>  # Discard all changes of file1 and file2
