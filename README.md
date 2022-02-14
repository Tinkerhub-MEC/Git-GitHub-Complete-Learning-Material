# Git-GitHub-Complete-Learning-Material

## Introduction
### 1. What is Git
<img width="219" alt="image" src="https://user-images.githubusercontent.com/75477017/153740913-bac0938d-2ba1-449a-9020-4dd6549433a4.png">


Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.<br>
It can be used to  track changes in the source code when multiple developers to work together. <br>
When multiple developers work together in a given project it's version keeps on changing and this can be controlled and managed by git.<br>
Git is free and open-source software distributed under the GPL-2.0-only license.<br>

### 2. What is GitHub
<img width="122" alt="image" src="https://user-images.githubusercontent.com/75477017/153740919-16cd4941-a593-4b7c-b789-d0735b8aa3cb.png">


GitHub is a for-profit company that offers a cloud-based Git repository hosting service. Essentially, it makes it a lot easier for individuals and teams to use Git for version control and collaboration.<br>
GitHub’s interface is user-friendly enough so even novice coders can take advantage of Git. Without GitHub, using Git generally requires a bit more technical savvy and use of the command line.<br>
Additionally, anyone can sign up and host a public code repository for free, which makes GitHub especially popular with open-source projects.<br>

## 3. Git Download

For downloading Git first go to <a href="https://git-scm.com/downloads" target="blank">https://git-scm.com/downloads</a> 
<img src="https://www.testingdocs.com/wp-content/uploads/Git-Download-Windows-11-OS.png"><br>
and download the installer as per the instruction given in the webpage for the required OS.Next open the installer and proceed with all the default settings.And after successful installation , you can verify it by typing the following command in terminal : <br>

```git --version```<br>
press enter...<br>
If something version number is displayed it means that git has been successfully installed in your system , if not try installing git again by following the steps given above.
## Git Commands

### 4. Git config
The git config command is a convenience function that is used to set Git configuration values on a global or local project level. These configuration levels correspond to .gitconfig text files. Executing git config will modify a configuration text file. 

### 5. Git Init

This is basically performed to initialise a folder/repository so as to perform git operations like adding, committing etc.<br>
Inorder to initialise local repositry with git we can run the following command to the respective folder location using terminal:<br>

```git init```<br>
      
press enter...<br>
Great... now your local repository has been initialized with git.<br>
<img width="340" alt="image" src="https://user-images.githubusercontent.com/75477017/153740951-d07aa7ec-e361-4681-8c27-e26542dc6026.png">


### 6. Git add
The git add command is used to add file contents to the Index (Staging Area).This command updates the current content of the working tree to the staging area.<br> It also prepares the staged content for the next commit. <br>Every time we add or update any file in our project, it is required to forward updates to the staging area.<br>
```git add --all```

### 7. Git commit 
After you do changes in your code you will do "commit".<br> Commit set a message about the changes you were done. <br>The commit also saves a revision of the code and you can revert the code to any version anytime in one click.<br>
```git commit -m"REQUIRED_COMMIT_MESSAGE"```<br>
REQUIRED_COMMIT_MESSAGE is the one which we add to identify each commits that we hae done.<br>

### 8. Git remote
A remote in Git is basically a bookmark for a different repository from which you may wish to pull or push code. <br>The bookmarked repository may be on your local computer in a different folder, on remote server, or it may even be the repository itself.<br>
```git remote add origin REPOSITORY_URL```<br>
 REPOSITORY_URL is the url of the repository to which we have to push the code.<br>

### 9. Git push
The git push command is used to upload local repository content to a remote repository.<br> Pushing is how you transfer commits from your local repository to a remote repo.<br>Remote branches are configured using the git remote command. <br>
```git push origin BRANCH_NAME```<br>
BRANCH_NAME is the name of the branch from which the code has to be pushed.<br>

### 10. Git branch
Git branches are effectively a pointer to a snapshot of your changes. When you want to add a new feature or fix a bug—no matter how big or how small—you spawn a new branch to encapsulate your changes. ... Instead of copying files from directory to directory, Git stores a branch as a reference to a commit.</br>
```git branch``` shows the list of branches in your project<br> 
```git branch NEW_BRANCH_NAME``` creates a new branch<br>
```git checkout BRANCH_NAME``` switches the branch to your prefered one.


### 11. Git Checkout

The Git Checkout command is used to switch between branches in a repository.<br>
This command is used to switch from one branch to another:<br>

```git checkout branch_name```    <br>

This command creates a new branch and also switches to it:<br>

```git checkout -b branch_name```   

### 12. Git log

Git log is a utility tool to review and read a history of everything that happens to a repository. Generally, the git log is a record of commits.<br>

```git log```    <br>

This command will display the last commits.

### 13. Git status

The git status command is used to display the state of the repository and staging area. It allows us to see the tracked, untracked files and changes.<br>
This command will not show any commit records or information.<br>

```git status```  <br>

This command lists all the files that have to be committed.

<img width="552" alt="image" src="https://user-images.githubusercontent.com/75128235/153767540-97aa3bb6-68d3-459c-96d0-b1dd8cab6ad6.png">

### 14. Git merge

Git merging combines sequences of commits into one unified history of commits.<br>

```git merge branch_name```   <br>

This command merges the specified branch’s history into the current branch.

<img width="552" alt="image" src="https://user-images.githubusercontent.com/75128235/153768678-49a87164-f0df-47ec-8dd4-789cfbbdc67f.png">

### 15. Git clone

This feature helps us to create a copy of a repository in our local system from the GitHub.<br>
By doing so we can test that code and see the output, if we want we can make additional features etc.<br>
```git clone REPOSITORY_URL```<br><br>
This REPOSITORY_URL will be the url of the required repository which is to be cloned to our local machine.<br><br>
<img width="552" alt="image" src="https://user-images.githubusercontent.com/75477017/153763383-aa08f5b4-f5e5-4954-98e5-d53926d641d3.png"><br>

## Some GitHub Processes 
### 16. GitHub Fork

A fork is a copy of a repository. Forking a repository allows you to freely experiment with changes without affecting the original project.<br>
Once you have forked a repo, you own your forked copy. This means that you can edit the contents of your forked repository without impacting the parent repo.<br>
You can fork any repo by clicking the fork button in the upper right hand corner of a repo page.

### 17. Git pull

The git pull command is used to fetch and download content from the tracking remote repository and immediately update the local repository to match that content.<br>
The git pull command is actually a combination of two other commands, git fetch followed by git merge<br>
The command used to pull recent commits from the tracking remote branch is:<br><br>
```git pull origin BRANCH_NAME``` <br>
BRANCH_NAME is the name of the branch to which pull function has to be done

### 18. Pull request

Pull requests let you tell others about changes you've pushed to a branch in a repository on GitHub.<br>
Once a pull request is opened, you can discuss and review the potential changes with collaborators and add follow-up commits before your changes are merged into the base branch.<br>
To create a pull request:<br>
1. Make your changes in the forked repository/new branch in the same repository<br>
2. Push the changes back to your repo<br>
3. Click the Compare & pull request button<br>
4. Click Create pull request to open a new pull request<br>


### 19. Merge Pull request

Merge a pull request into the upstream branch when work is completed. Anyone with push access to the repository can complete the merge.<br>
To merge a pull request:<br>
1. Under your repository name, click Pull requests.<br>
2. In the "Pull Requests" list, click the pull request you'd like to merge.<br>
3. Choose the merge options for your repository.<br>
4. If prompted, type a commit message, or accept the default message.<br>
5. Click Confirm merge.<br>
6. Optionally, delete the branch. This keeps the list of branches in your repository tidy.<br>
<img width="444" alt="image" src="https://user-images.githubusercontent.com/75477017/153741072-62e12f18-8dbd-40f5-8f01-667abb452fcd.png"><br>
### Here is a funny video which shows the effect of merge XD :)<br>
 [![Watch the video](https://www.youtube.com/watch?v=dygYh2qsx64)


### 20. Fetch & Merge

### 21. Github Pages
This is basically a free front end web hosting service provided by GitHub .<br>
We can even add customised domain names to our websites.<br>
This service can give a glance to clients  on how our web based projects work.<br>
Steps to host:<br>
    1. Push your code to GitHub using git commands from terminal <br>
    2. Go to repository settings of that repository and click "pages".<br>
    <img width="483" alt="image" src="https://user-images.githubusercontent.com/75477017/153762420-2d4cd2f8-00dd-4586-9037-4a371372b4a1.png"><br>
    <img width="500" alt="image" src="https://user-images.githubusercontent.com/75477017/153762505-61efdaa2-4cf8-4be1-8dba-d47c11f3ff33.png"><br>
    3. In that source option change that from none to master(or the branch name which you want to delpoy).<br>
    <img width="527" alt="image" src="https://user-images.githubusercontent.com/75477017/153762612-967c7640-8e49-4f25-bfc2-4acae50dc7f6.png"><br>
    4. Now save it and wait for few seconds.<br>
    5. Now we can see a url that gets popped up this will be the url of our public website.<br>
    <img width="510" alt="image" src="https://user-images.githubusercontent.com/75477017/153762699-4f63fde5-de37-4716-bfcf-5b1a8f12d999.png"><br>

    
