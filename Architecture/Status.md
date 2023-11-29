# Work Flow 

## 1-Initialization:

### Begin by initializing a Git repository in your working directory using the git init command. At this point, Git is unaware of any file details.

## 2-Untracked State:

### Files in the working directory are initially untracked. Git doesn't monitor changes in these files.

## 3-Staging Transformation:

### To start tracking changes, add the file to the staging area using the git add command. This action transforms the file into a tracked state.

## 4-Staging Area (Index):

### The staging area serves as a holding area where changes are selectively gathered before committing them. It acts as an intermediate step between the working directory and commits.

## 5-Commit Creation:

### With changes staged, proceed to create a commit using the git commit command. A commit represents a snapshot of the project at a specific moment, marking a significant point in the version history.

###
![WF](https://res.cloudinary.com/practicaldev/image/fetch/s--M_fHUEqA--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://thepracticaldev.s3.amazonaws.com/i/128hsgntnsu9bww0y8sz.png)

# File status

## 1- Untracked(U) :
### In this stage, the Git repository is unable to track the file, which means that the file is never staged nor it is committed.

## 2- Tracked :

## A- Unmodified (M) :
### Either never changed since tracked, or commited and never changed afterwards

## B- Modified :

### Either doesn't have a snapshot or been changed since last commit

## c- Staged :
### Had some changes and ready to be committed


###

![FS](https://raw.githubusercontent.com/ahmedsami76/AraBigData/a4b6d07d50e36eded3e80966eedb903579f2e34d/Git/images/git7.jpg)













