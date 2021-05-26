> # **GIT**
---
> ## **Contents**
- [Introduction](#Introduction)
- [Concepts](#Concepts)
- [Basic Commands](#Basic-Commands)
- [Intermediate GIT Commands](#Intermediate-GIT-Commands)
- [Conclusion](#Conclusion)
---
> ### **Introduction**
---

Git is a distributed version control system. It can track changes in computer files. With the help of GIT multiple developers can coordinate betwween their work. Any one can made changes on files and commit for helping others. We can back to previous stage of a file using branches of GIT. Git provides local and remote repositories.

---

> ### **Concepts**
---
- [Contents](#Contents)


* Keeps track of code history
* Takes snapshots of files
* User can visit any snapshot at any time
* User can commit while taking snapshots
* User can also stage files before comitting

---

> ### **Basic Commands**
---
- [Contents](#Contents)

* **$git config** : This command is used to set the username and email address of the user who want to commit the changes in his repository.
    
    * ``` $git config -global user.name [user name]```

    * ```$git config -global user.email [email address]```

* **$ git add filename**  : Add file to Index

* $ git add *  : Add all files to Index

* **$ git status**  :  Check status of working directory

* **$ git commit**  :  Commit changes to index

* **$ git commit -m [type a message]**  :   It is used to record a file in its version history. And we can add a message at the end of commit to identify why we make a change in the file. 

* **git commit -a**  : This command is used for make changes to all files.

* **$git diff** : This command is used to display all the differences between the files until the changes have not yet been staged.

* **$git diff -staged** : This command is used to display all the differences files in staging area and all latest updated files.

* **$git diff** **[first branch] [second branch ]** : This command is used to display the differences between two branches. 

* **$git reset filename** : This command is used to unstage a file.

* **$ git push**  : Push to remote repository

* **$ git pull**  :  Pull last updated file from remote repository

* **$ git clone**  :  Clone repository into a new directory
---
> ### **Intermediate GIT Commands**
---
* **git reset [commit]** : This command is used after completeing a commit. This command can undo all the previous changes. Best command for local repository.

* **git reset -hard [commit]** : discard all the previous history and specified the last commit.

* **git rm [file]** : this command is used to delete the file from the current directory. It is also used to stage the deletion process.

* **git log** : represents the version history of the current working log.

* **git log -follow [file]** :  gives the version history of a current file.

* **git show [commit]** : display the metadata of all content related changes of a perticular commit.

* **git tag [commit ID]** : This is used to give a perticular tag to the code which is commited.

* **git branch** : list down all the branches that is present in the current repository.

* **git branch [branch name]** : this is used to create a new branch.

* **git branch -d [branch name]** : used to delete the current specified branch.

* **git checkout [branch-name]** : This is used to switching between branches.
---
> ### **Conclusion**
---
- [Contents](#Contents)

When a developer practicing or developing codes for a perticular project he or she needs to create a backup of his or her source codes. Also when a program is under developing we have to make changes on it time to time. So we also need to create backup of all the versions of those codes. This is a very hard job to do. And if we save all this in our local hard drive then it is not backed up. Back up means mimimum two copies of same file in different drives.
GIT gives us a **local repository** and a **remote repository**. We can save files to our local repository and **commit changes** for different versions. Thats why it is called a **Version Control System**. And we can also send these files to a **remote repository provided by GITHUB**.It is very helpfull for more than one developer as a team working on a single project.

---
- [Contents](#Contents)





