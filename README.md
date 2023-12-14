# Basic-Git-Command
**Basic Git Command for Beginners**

# Config
```sh
$ git config --global user.name <your-name>
$ git config --global user.email <your-email>

$ git config --local user.name <your-name>
$ git config --local user.email <your-email>
```
# Show
```sh
$ git branch                                 # Show all local branches
$ git branch -r                              # Show all the remote branch
$ git branch -av                             # Show all local and remote branches
```
# Create
```sh
$ git branch <branch-name>                   # Create a new branch
$ git checkout -b <branch-name>              # Create & checkout to new branch
$ git checkout --orphan <branch-name>        # Create a branch with no commit list
```
# Push
```sh
$ git push origin <branchname>               # Push to remote branch
```
# Delete and Add
```sh

$ git branch -d <branchname>                 # Delete the local branch, show a warning
$ git branch -D <branhcname>                 # Force to delete branch
$ git remote prune origin                    # Cleanup remote deleted branch

$ git add .                                                               
$ git add --all                                     # Add all changes     
```
# Commit  
```sh                                                                
$ git commit -am 'commit message'                   # Add & commit        
$ git commit --allow-empty -m k3;                   # Commit empty change
$ git cherry-pick <commit-hash>                     # Take a commit change of another branch 
```
# Amend
```sh
$ git add task2.txt                                 # Add any file
$ git commit --amend -m 'new message'               # Merge current change to previous commit and will also change the commit hash
```
# Pull
```sh
$ git pull origin <branch-1>                        # Pull the change of 'branhc-1' in current branch 
```
# Push
```sh
$ git push origin <branchame>                       # Push a branch
$ git push -f origin <branch-name>                  # Overwrite remote branch (by force)
```
# Merge
```sh
$ git merge origin <branch-1>                       # Merge remote 'branch-1' with current branch
$ git mergetool
$ git merge --squash <privateFeatureBranch>
```
# Set local folder to response remote url
```sh
git remote set-url origin git@XXXXXXXXXXXX
```
# Checkout
```sh
$ git checkout <commit-hash>               # Go to a specific commit
$ git checkout <branch-name>               # Return to present state
$ git checkout <commit-hash> <file-name>   # Only a file will go back to specific commit
$ git checkout <branch-name> -f            # Return to persent state by force
$ git checkout -- <filename1> <filename2>  # Discard all changes of file1 and file2
```
