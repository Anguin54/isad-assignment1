# Version Control
This file will explore and explain the version control system that should be used for the project.\
This will inclue what branches will be required, what time they need to be created, and what time they need to be merged into the master branch.\
These times will be explained based on the assumption that the project goes smoothly, and according to plan.\

## How to Use an Online Repository and Local git
There many commands to be used for version control, to commit changes, create branches, and then merge and delete branches. After the software development, it would also be pushed and pulled from a GitHub repository.\

### Command to set up git 
Firstly, to use version control git must be initialised, then the developer id must be given
> $git init
> $git config --global user.name "FirstName LastName" 

### Commands for making files and edits
Then, files need to be created, so that they be edited, staged then changes commited. \
The command to create a file is
> $vim FileName.format
This command will either access a file with the name FileName.format, or create it if it does not exist. \
The commands to stage then commit changes are
> $git add FileName.format
> $git commit -m "Change made"
The message for the commit should be descriptive of what exact change was made to the file.\
Committing does not need to be overly done, and should only be used when significant changes, or progress is made.

### Setting up a GitHub repository 
The overall software needs to be able to be accessed by all the members of the development team. This is done by using an online GitHub repository that everyone has access to.\
First the repository needs to be set up by the administrator, which is done simply online on the GitHub website, and then the access link needs to be distributed to all the members of the development team.\
The command to connect the online GitHub for development access is:
> git remote add origin "https://..."
"https://..." is a placeholder for the actual link to the github. \
'origin' is simply a name assigned to the online GitHub.\

### Commands to use multiple branches - developers.
There is only one branch that exists by default, which is called the master branch. No manual changes should be made in this branch, and instead functionality should be merged into it.\
During the development, secondary branches will be used to implement various features at the same time. This would require creating multiple branches, and also having multiple versions of the software simultaneously. When the task for the branch is completed, the branch would also be need to be pushed to the GitHub repository.\
The commands to create, then move into a branch are:
> $git branch branchName
> $git checkout branchName

### Using the online GitHub repository
The main two actions that are done using the online repository are pushing and pulling branches. \
Developers will be mainly be using the push function to push a branch to the local repo when they have finished implementing functionality in the software. \
The command to push a branch to the origin is:
> $git push -u origin branchName
A project manager would be using the pull (fetch) function to review the implemented functionality, and merge into the master branch when he/she is satisfied with the quality of the functionality.\
The commands to fetch, and subsequently merge a branch to the master from the orign are:
> $git fetch origin branchName
> $git checkout master
> $git merge branchName
If the project manager wants to delete the secondary branch after the merge, but also archive the branch, the commands are as follows:
> $git tag archive/branchName branchName
> $git branch -d branchName

## Branches Required
For each include the name of the branch, the branches purpose, the time it should be created, when it should be merged, and what functionality it should have when it is finished development (summary of the branches purpose again, but some application).\
The initial set up, which is task 1.0 in the wbs, is set up in the master branch, and is implemented from time 0 to 13\
The following table displays the branches needed, the time when the branches should be created, and the time when the branch should be pushed. The time to be created should be the earliest possible start for the tasks, and the time for pushing should be the latest finish for the tasks.\
The unit for time is all in days.\
Branch Name|Time Created|Time for Push|
:----------|:----------:|:-----------:|
VehicleTracking|13|34|
PostBlizzardChecks|13|34|
DataCollectionSystemStatus|13|34|
MonitorLivingQuarters|13|34|

