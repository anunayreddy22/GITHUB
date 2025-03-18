# GIT AND GITHUB

Git is a version control system which lets you track changes you make to your files over time. With Git, you can revert to various states of your files (like a time traveling machine). You can also make a copy of your file, make changes to that copy, and then merge these changes to the original copy.

You can run this command on the command line: git --version. This shows you the current version installed on you PC. The next thing you'll need to do is to set your username and email address. Git will use this information to identify who made specific changes to files.

To set your username, type and execute these commands: git config --global user.name "YOUR_USERNAME" and git config --global user.email "YOUR_EMAIL". Just make sure to replace "YOUR_USERNAME" and "YOUR_EMAIL" with the values you choose.

Now to initialize your project, simply run git init. This will tell Git to get ready to start watching your files for every change that occurs. It looks like this:

![Screenshot--95-](https://github.com/user-attachments/assets/45f4130a-a7e9-48e2-8ed3-c96ef5b36b02)

The first line has information about my PC and the path to where the folder exists. The second line is the command git init, and the third line is the response sent back telling me that my repository (repo) has been initialized. It is considered empty because we have not told Git what files to track. A repository is just another way to define a project being watched/tracked by Git.

What is GitHub?
GitHub is an online hosting service for Git repositories. Imagine working on a project at home and while you are away, maybe at a friend's place, you suddenly remember the solution to a code error that has kept you restless for days.

You cannot make these changes because your PC is not with you. But if you have your project hosted on GitHub, you can access and download that project with a command on whatever computer you have access to. Then you can make your changes and push the latest version back to GitHub.

In summary, GitHub lets you store your repo on their platform. Another awesome feature that comes with GitHub is the ability to collaborate with other developers from any location.

Add and commit file(s)
Before we "add" and "commit" our files, you need to understand the stages of a file being tracked by Git.

Committed state
A file is in the committed state when all the changes made to the file have been saved in the local repo. Files in the committed stage are files ready to be pushed to the remote repo (on GitHub).

Modified state
A file in the modified state has some changes made to it but it's not yet saved. This means that the state of the file has been altered from its previous state in the committed state.

Staged state
A file in the staged state means it is ready to be committed. In this state, all necessary changes have been made so the next step is to move the file to the commit state.

TO ADD FILES IN GIT
**git add .** (All files)  
**git add about.txt**  (specific file)
**git status** (to know current status of the file)

When you add files it will be in staged stage state. we need to commit them.

TO COMMIT FILES IN COMMIT

**git commit -m "first commit"**

Now the file is in commited state

**git log** => to see the commits

**git diff** => to look differences in our current files from previous saved version.

**git checkout filename**  => rollback to last version 

Create and push remote repositories.

**git remote add origin url**(this is the url of our remote repository)

then 

**git push -u origin main**  main is the branch name 

if we want to remove all the files from staging area then use => **git rm --cached -r.**

Lets now learn what is **.gitignore**

Suppose we have a file which have passwords, API keys which we dont want to commit on github , so inorder for this we should add the imp files in .gitignore file (**touch .gitignore**)
if we want  to ignore log files then add this *.txt (now files with .txt extension will be ignored) in .gitignore file.














