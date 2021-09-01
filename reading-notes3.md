# Git Workflow

## Local Repository Structure

1. Working Directory: Where the files reside
2. Index: The area used for stageing
3. Head: Points to the most recent commit

Working directory -- add --> Index -- commit --> Head

## Saving Changes

- files can are either tracked or untracked
- Tracked
  - modified, unmodified, or staged
  - part of the most recent snapshot
- Untracked
  - not in the last snapshot and not in the staging area

## The Life Cycle of File Status

untracked       Unmodified        Modified          Staged
    |               |                |                 |
    |               |-> Edit File -> |                 |
    |-> Add File -> |                |                 |
    |               |                |-> Stage File -> |
    |<- Remove File-|                |                 |
    |               |<- Commit File--|-----------------|

## Tracking and Staging a New File

**Single File**
` git add filename `

**All Files**
` git add * `

## Commiting a File

- after staging one or more files, you should commit the changes and leave a descriptive message

` git commit -m "made change x,y,z" `

## Pushing Changes

- finally, push the changes to a remote repository (github)

` git push origin main `