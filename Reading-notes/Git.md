# Git
## Here I will put my notes about the Git topic from Read02b

## What is Git And Why we use it

Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.
Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.

Git work Locally to trace our work and organize it to a versions using the version controll system that it has 

### here an image show us how the whole process work
![vcsGitLocal](https://blog.udemy.com/wp-content/uploads/2015/08/image066.png)

## Version Control
Version Control is a system that allows you to revisit various versions of a file or set of files by recording changes. Through version control, one can revert a file or project to a previous version, track modifications and modifying individuals, and compare changes. By utilizing a Version Control System (VCS), mistakes with files can easily be rectified.


## Some git command and instructions
Fistly as we know before we can work with git from our terminal
to work with the git commands we should know some of terminal command that control our position and creating files and move between the folder without Gui like (mkdir, cd , cd .., ls )
After make revision to them here the main commands we use them to work with the Git and Setup it 

## git clone the github repositry link
this command we should use it to download our repo file locally to our computer

## git add .
this to tell the git to start trace our work 

## git status
to see our file status if there's a change that we didn't upload or we haven't pushed

## git commit -m"any message you want "
this commant to commit our work locally and the message should be show whats the changes that we did

## git push origin main 
this command send our new changes directly to the github to save it online 
after this we have to put our github account username and password

## another photo that will help to figure the whole process
![GitWork](https://blog.udemy.com/wp-content/uploads/2015/08/image006.png)