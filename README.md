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
 ![Watch the video](https://www.youtube.com/watch?v=dygYh2qsx64)
[![Watch the video](data:image/jpeg;base64,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)](https://www.youtube.com/watch?v=dygYh2qsx64)

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

    
