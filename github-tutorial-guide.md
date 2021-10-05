## Version Control (VCS)
-A system that records and allows you to view different stages of a project. 
This allows you to view where you made changes to the code, and see where mistakes/errors originated.

-Centralized Version Control (CVCS) helps with the ease of collaboration, storing a file and all of its changes
on a singe server that all team members can access.

-A Distributed Version Control (DVCS) creates backups on a different server that can be moved to the 
CVCS in case of corruption or loss of code.


## Git
-A DVCS that stores each version of your project as a snapshot.
-Relies on local operations
-Tracks all changes to a file, as well as loss or corruption
-Files that are in Git can exist in committed, modified, or staged states.
 -Committed: stored in a local database.
 -Modified: changed but not committed to the database.
 -Staged: checked that a file's changed version can be committed.
 

## Setting up a Git Repository
### Importing
-switch to the target project's directory

-use the 'git init' command

-perform an initial commit by typing:

  -'git add * <!-- -->.c' 
 
  -'git add LICENSE'
 
  -'git commit -m "and message here"'
  
  ### Cloning
  -clone command: 'git clone "repository URL"'
  
  -to rename and clone into another directory: 'git clone "repository URL" mydirectory'
  
  
  ## Check File Status
  -'git status'
  
  
  ## Workflow
  
  ### Local Repository Structure
  
  Working Directory -add-> Index -commit-> Head
  
  ### Saving Changes
  -All files in a working copy of a project can be in two states:
  
   -Tracked: These files can be modified/unmodified/staged and are part of the most recent snapshot
   
   -Untracked: These files can not be modified/staged/ as they are not part of the most recent snapshot


### Life Cycle of File Status

Untracked -add file-> Unmodified -edit file-> Modified

Untracked <-remove file- Unmodified           Modified -stage file-> Staged

Unmodified <-commit file- Staged


#### Check File Status

-'git status'

#### Tracking and Staging a New File

-a single file: 'git add filename'

-all files: 'git add * <!-- --> '

#### Committing a file

-'git commit -m "made change x,y,z"

#### Committing all changes

-'git commit -a'

#### Pushing changes

-'git push origin master'

### Stashing changes

-'git stash'

-to retrieve when ready to work again, use 'git stash apply'
