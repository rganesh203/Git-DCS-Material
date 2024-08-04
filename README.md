# Git-DCS-Material
GitHub and Git Tutorial for zero to pro.
A beginner's tutorial demonstrating how Git version control works and why it is crucial for data science projects.

https://images.datacamp.com/image/upload/v1651047046/image8_0e61d0dad8.png

What is Git?
Git is a distributed, open-source version control system. It enables developers and data scientists to track code, merge changes and revert to older versions - AWS. It allows you to sync changes with a remote server. Due to its flexibility and popularity, Git has become an industry standard as it supports almost all development environments, command-line tools, and operating systems. 

How does Git work?
Git stores your files and their development history in a local repository. Whenever you save changes you have made, Git creates a commit. A commit is a snapshot of current files. These commits are linked with each other, forming a development history graph, as shown below. It allows us to revert back to the previous commit, compare changes, and view the progress of the development project - Azure DevOps. The commits are identified by a unique hash which is used to compare and revert the changes made.  

A graph of the development history

Branches
The branches are copies of the source code that works parallel to the main version. To save the changes made, merge the branch into the main version. This feature promotes conflict-free teamwork. Each developer has his/her task, and by using branches, they can work on the new feature without the interference of other teammates. Once the task is finished, you can merge new features with the main version (master branch). If you want to learn how to clone a branch, check out this tutorial on Git Clone Branch.

Adding new feature to repository

Commits
There are three states of files in Git: modified, staged, and commit. When you make changes in a file, the changes are saved in the local directory. They are not part of the Git development history. To create a commit, you need to first stage changed files. You can add or remove changes in the staging area and then package these changes as a commit with a message describing the changes.  

Three states of files in Git

What are the benefits of Git?
Track changes: It allows developers to view historical changes. Development history makes it easy to identify and fix bugs.
IDE Integration: Due to its popularity, Git integration is available in all development environments, for example VSCode and JupyterLab.
Team collaboration: A developer team can view their progress, and by using branches, they can work individually on a task and merge changes with the main version. Pull requests, resolving merge conflicts, and code review promote team collaboration. 
Distributed VSC: In a distributed system, there is no centralized file storage. There are multiple backups for the same project. This approach allows developers to work offline and commit changes. 
Git for Data Science Projects
Git provides version control for scripts, metrics, data, and models. By using Git extension git-lfs, you can store and version a large database and machine learning models. In a typical data science project, you have a Jupyter notebook, dataset, model, metadata, and model metrics. The metadata includes files containing meta-information about the machine learning model, features, model parameters, and automation files. All of these are necessary for monitoring the progress of AI applications and resolving issues. 

Track data science experiments help scientists revert accidental changes, select the best experiment based on the performance metric, and collaborate with other teammates. The diagram below shows how changes to data or code affect the metadata and output of the model. Tracking these changes can also help other teammates come up with a better solution. Learn all about Git in the latest blog from Summer Worsley.

Collaboration with GitHub
GitHub is a cloud software development platform. It is commonly used for saving files, tracking changes, and collaborating on development projects. In recent years, GitHub has become the most popular social platform for software development communities. Individuals can contribute to open-source projects and bug reports, discuss new projects and discover new tools. 

Data scientists and machine learning engineers are following the path of software developers and integrating the workflow with GitHub. By doing this, they can share their research work, allow community contribution, and collaborate with data teams. You can find all kinds of data science and machine learning projects, guides, tutorials, and resources on this platform. For students, the platform has become an opportunity to gain work experience and eventually land a job in a prestigious company. 

Portfolio
Most technical recruiters will ask for the portfolio projects or GitHub profile. This helps them determine whether a candidate is a good fit for their company. It is highly recommended to create a GitHub profile and update it regularly. Hiring managers are always on the lookout for candidates that are highly experienced in software development and contribute to open-source projects. Being able to analyze the GitHub portfolio helps them prepare questions for technical interview sessions. 

GitHub Profile

GitHub enables data scientists to showcase their projects, and it can also count as work experiences on your resume. Showcasing portfolio projects also creates opportunities to work together, launch a startup, and research work. 

Portfolio Projects

Features
GitHub also provides various other features that are as important as showcasing a portfolio. It is necessary to learn about each feature so that you can incorporate them into your data science projects. 

Open-source: GitHub provides a complete ecosystem for open-source projects. You can sponsor maintainers, contribute to a project, use the open-source tool in your existing project, and promote your work. 
Community Collaboration: GitHub has become a community platform where issues, feature requests, code, and documentation contributions can be discussed. 
Explore: GitHub Explore tab helps you discover new projects, trending tools, and developer events. 
GitHub Gists: You can share the snippet of your code or embed it in a blog or website. 
GitHub CLI: It allows you to perform merge requests, review code, check issues, and monitor progress from the command line program. 
Free Storage: unlimited private and public repositories storage.
Web hosting: You can publish your portfolio site or documentation. GitHub pages provide easy to build and deploy website experience. 
Codespace: a cloud development environment integrated with your GitHub repository. 
Project: a customizable, flexible tool for planning and tracking the work on GitHub.
Automation: GitHub Action automates development workflow such as build, test, publish, release, and deployment.
Sponsor: You can support your favorite open-source project or developers by paying a monthly or one-time fee. It also allows developers to use third-party payment platforms such as ko-fi. 
Basic Commands
Before we jump into managing data science projects, let's learn about the most common Git commands that you will be using in every data science project. The basic commands include initializing the Git repository, saving changes, checking logs, pushing the changes to the remote server, and merging. 

git init create a Git repository in a local directory.
git clone <remote-repo-address>: copy the entire repository from a remote server to remote directory. You can also use it to copy local repositories.
git add <file.txt>: add a single file or multiple files and folders to the staging area.
git commit –m “Message”: create a snapshot of changes and save it in the repository. 
git config use to set user-specific configurations like email, username, and file format. 
git status shows the list of changed files or files that have yet to be staged and committed.  
git push <remote-name> <branch-name>: send local commits to remote branch of repository.  
git checkout -b <branch-name>: creates a new branch and switches to a new branch.
git remote –v: view all remote repositories.
git remote add <remote-name> <host-or-remoteURL>: add remote server to local repository. 
git branch –d <branch-name>: delete the branch.
git pull merge commits to a local directory from a remote repository. 
git merge <branch-name>: after resolving merge conflicts the command blends selected branch into the current branch.
git log show a detailed list of commits for the current branch.
Complete Development with GitHub

If you are interested in learning more commands, check out the Git cheat sheet by Gitlab. 

Getting started
In this section, we are going to use Git to track a data science project and GitHub as a remote server. We will learn how to install Git, create and clone a repository from GitHub, run machine learning experiments, and push changes (notebook, model, data) to GitHub using Windows PowerShell 7.  

Installing Git
Git supports all operating systems. You can install it using command-line tools or directly download and install the setup. 

Linux

For Debian/Ubuntu-based operating systems use `apt-get install git`, and if you are using another Linux-based system, check out the complete list of installing commands here.

macOS

If you have homebrew installed, use this command to download and install Git: `brew install git`. You can also download the binary installer and run the setup.

Windows

Installing Git on Windows is hassle-free. Just go to the download page, click on the specific Windows version, and download and install the setup. If you have a winget tool, you can install it by typing `winget install --id Git.Git -e --source winget` in PowerShell. 

After installing Git, make sure you have configured the user name and email. This information is used to sign the commits. 


git config --global user.name "your-user-name"
git config --global user.email "your@email.com"

For more in-depth information on how to install Git, click here. 

Initializing the Project
If you have a GitHub account, click on the + button and select a new repository. After that, type the repository name and add a simple description. It will create an empty public repository. 

Creating project

There are many ways to clone remote repositories to the local directory, and GitHub provides a detailed guide on how to clone, add remote, and initialize a Git project.  

GitHub Clone

We can simply clone the repository by providing an HTTPS link. Make sure you are in the working directory using the command prompt or PowerShell. 


git clone https://github.com/kingabzpro/DataCamp-Git.git

>>> Cloning into 'DataCamp-Git'...
>>> warning: You appear to have cloned an empty repository.

cd .\DataCamp-Git\

Powered By 
OR

Create a new directory called “DataCamp-Git” and initialize Git using a simple command. After that, add a connection to the remote repository so that you can sync your work with GitHub.


mkdir DataCamp-Git
cd .\DataCamp-Git
git init

>>> Initialized empty Git repository in C:/Repository/GitHub/DataCamp-Git/.git/

git remote add origin https://github.com/kingabzpro/DataCamp-Git.git

Powered By 
OR

If you already have a project in a directory, just initialize Git using `git init` and add GitHub remote, as shown above. 

Simple Commit
Before we add files to our repository, make sure you are in the correct local directory. 

We will start simple and create a README file with the heading DataCamp-Git. Then, we will add it to the staging area by using `git add`. 


echo "# DataCamp-Git" >> README.md
git add README.md


Git status shows that we are on the main branch and the `README.md` file is staged and ready to be committed.  


git status

>>> On branch main
>>> No commits yet
>>> Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md


To create our first commit, we will use `git commit` with a message. As we can observe, the first commit is added under the ed9c886 hash.


git commit -m "first commit"

>>> [main (root-commit) ed9c886] first commit
>>> 1 file changed, 1 insertion(+)
>>> create mode 100644 README.md


Adding Project Files
We will use the DataCamp workspace MasterCard Stock Price with LSTM and GRU and download files. The author of the project has preprocessed the data and training time series data on the LSTM and GRU models. Learn more about the project by reading Recurrent Neural Network Tutorial (RNN).

To save the model file, we have added a new code cell in the project's Jupyter notebook. The new script will create a new directory called “model” and save both LSTM and GRU models. 

!mkdir -p model
model_lstm.save('model/LSTM')
model_gru.save('model/GRU')

As we can see, the Git repository has a data folder containing CSV files, the model folder with the model’s weight and metadata. 

Git Data Folder

We will now stage all the files. You can add any directory, file, or data after the initial command. 


git add .\data .\model LSTM_GRU.ipynb RNN.png

OR

If you want to add all files to the staging area, then use dot. 


git add .

Powered By 
Commit and Push
We will commit all the changes with a simple message, and the output shows all the new files in create mode. 


git commit -m "project files added"

>>> [main aa3e19a] project files added
>>>  10 files changed, 5020 insertions(+)
>>>  create mode 100644 LSTM_GRU.ipynb
>>>  create mode 100644 RNN.png
>>>  create mode 100644 data/Mastercard_stock_history.csv
>>>  create mode 100644 data/Mastercard_stock_info.csv
>>>  create mode 100644 model/GRU/saved_model.pb
>>>  create mode 100644 model/GRU/variables/variables.data-00000-of-00001
>>>  create mode 100644 model/GRU/variables/variables.index
>>>  create mode 100644 model/LSTM/saved_model.pb
>>>  create mode 100644 model/LSTM/variables/variables.data-00000-of-00001
create mode 100644 model/LSTM/variables/variables.index

Syncing with GitHub remote repository requires a remote name and branch name `git push <remote-name> <branch-name>`. If you have only one remote and one branch, then using `git push` will work.  

After `git push`, the pop-up window will ask for the credentials, just add your GitHub username or password. You can also generate Personal access tokens and add them instead of the password. Learn more by reading the Git Push and Pull Tutorial.


git push

>>> Enumerating objects: 21, done.
>>> Counting objects: 100% (21/21), done.
>>> Delta compression using up to 4 threads
>>> Compressing objects: 100% (19/19), done.
>>> Writing objects: 100% (21/21), 1.83 MiB | 1.59 MiB/s, done.
>>> Total 21 (delta 2), reused 0 (delta 0), pack-reused 0
>>> remote: Resolving deltas: 100% (2/2), done.
>>> To https://github.com/kingabzpro/DataCamp-Git.git
>>>  * [new branch]      main -> main

We are going to check our GitHub repository kingabzpro/DataCamp-Git to see whether we have successfully pushed the changes to remote. The GitHub repository has all the files, data, and models.

Remote push to GitHub
Remote push to GitHub

Git Branches
It is recommended to work with branches: for example, if you want to work on project documentation, create a documentation branch using `git checkout` or `git branch`. Make changes in the README file and when you have finalized the changes, merge the branch with the base. 

In our case, we have created and switched to a new branch called `readme`.

git checkout -b readme

Let’s edit the README file by adding a description to the project and link the RNN DataCamp workspace and tutorial. After that, we will stage changes and save a snapshot of changes with a message.


git add README.md
git commit -m "project description and links to blog"

>>> [readme f3b8b9b] project description and links to blog
>>>  1 file changed, 8 insertions(+)

Powered By 
The remote repository doesn't have a readme branch. To create a new branch and push changes, we will use “readme:readme”. The output of the command shows that new branches have been created and both local and remote `readme` branches are synced. 


git push origin readme:readme
>>> remote: Resolving deltas: 100% (1/1), completed with 1 local object.
>>> remote: Create a pull request for 'readme' on GitHub by visiting:
>>> remote:  https://github.com/kingabzpro/DataCamp-Git/pull/new/readme
>>> remote:
To https://github.com/kingabzpro/DataCamp-Git.git
>>>  * [new branch]      readme -> readme

You can observe that we have successfully pushed the local branch to GitHub with a modified version of README.md file. 

Readme branch on GitHub
Readme branch on GitHub

Pull Request
This functionality is common for organizations. For example,  a software developer has worked on a new feature and wants to merge changes to the main remote branch. We will now create pull requests using GitHub GUI by clicking on the pull request button. After that, select the readme branch  which we want to merge with the base (main). You can type a detailed explanation of what features were added and click on the pull request button. 

Pull request from readme to main branch
Pull request from readme to main branch

The maintainer of the repository will compare your changes and merge them when they have passed all the tests. In our case, you are the maintainer, so click on the merge request to blend changes with the main branch. 

GitHub Merge Pull Request
Merge pull request on GitHub

Congratulations, we have successfully created a pull request and merged it with the main branch. You can view the changes on the main branch here. 

If you want to view all the changes within your git repository, just type `git log`, and it will show historical changes to your project. Logging changes in data science projects are important, and Git helps us track all the changes, even large datasets. 

History of Git Logs
History of Git Logs

Conclusion
GitOps are crucial for data application development. They have become an essential skill for all types of IT jobs; even academic researchers are using them to share experimental code with a wider audience. On the other hand, GitHub plays a larger role in promoting open-source projects by providing a free software development ecosystem for all. 

In this tutorial, we have learned about Git and GitHub and why they are important for data science projects. The tutorial also introduces you to basic Git commands and provides hands-on experience on how to track changes in data, model, and code. If you are interested in learning more about Git, then take an Introduction to Git course on DataCamp. You can also learn about the importance of GitHub certification and how it can help your career. 


What is Git?
An open-source distributed version control system. It allows developers to store, version, and visualize changes in a development project. It promotes flexible teamwork and optimized workflow. 

What does Git stand for?
It is not an acronym. According to its creator, Linus Torvalds, “Git can mean anything, depending on your mood.” It is a combination of three random letters that are not used by any UNIX command.  

How do I clone a Git repository?
Just type `git clone <remote repository address>` in a terminal. You can clone local and remote repositories. It supports both SSH and HTTPS protocols.

How to delete a branch in Git?
For deleting a local branch, use `git branch -d <local_branch_name>`, and for deleting the remote branch, use `git push <remote_name> -d <remote_branch_name>`.

How to switch branches in Git?
Switch to an existing branch using `git checkout <branch name>` or create and switch to a new branch using `git checkout -b <branch name>`.

How do I install Git?
For Linux systems use `apt-get install git`, and for other operating systems check out git-scm.com.

Is Git free?
Yes, it is free and open-source under the GPL-2.0 license.

What is Git Bash?
It is a Microsoft Windows application that provides Unix-based shell utilities & experience. 

How to create a new branch in Git?
Use `git branch <new-branch> <base-branch>` command in terminal. To create and switch to a new branch, use `git checkout -b <branch name>`.

What does git pull do?
It updates the local version of a repository from a remote server, and copies all the changes from a remote repository, and merges them with the local directory. This process often requires resolving merge conflicts. 

1. Git, Distributed Version Control System (VCS) Introduction. Explore Different types of VCS - GIT
2. Working, Staging & Repository area in GIT Project. Understand the GIT Workflow for Project - GIT
3. Installation of GIT in different OS like windows, Linux and MacOS. Check the version of git
4. Git Configuration Levels. Explore Local, User, and System level config files - GIT
5.  Add Git username and user email in configuration file using Git Config command - GIT
6.  Understand Git help and status command details - GIT
7.  Add and commit file into the GIT staging area and repository area in the GIT Project - GIT
8.  GIT Diff Command. Track changes of file between working, staged & repository area using Diff.
9.  How GIT stores the data. Explore the git SHA1 hash objects in repository with cat-file command.
10.  Rename and Restore files in GIT Repository using the mv and the restore command - GIT
11.  Git Branching. Understand the concept of creating branches in the GIT Project
12.  Practical implementation of the git branching in the project - GIT
13.  Rename and Delete branch using git branch -m and the -d commands in GIT Project - GIT
14.  GIT Merge. Merging two branches. Understand fast forward and recursive strategy methods - GIT.
15.  Resolve conflicts while merging the two branches in the GIT Project - GIT
16. GIT Rebase. When we need to use Git Merge and git Rebase in the Project - GIT
17. Implementing GIT Rebase in project and understand the difference between merge & Rebase - GIT
18. Interactive Rebasing. Rewriting History by Changing & Squashing Multiple Commit Messages - GIT
19. Modify or Change the last or latest commit using the amend command in the GIT Project - GIT
20. GIT Cherry-pick. Handle bugfix or Hotfix by cherry picking a commit into another branch - GIT
21. Detached Head in GIT. How can we handle the detached head state in Project - GIT
22. GIT Reset. Move the branch to specific commits using the git reset in the Project - GIT
23. GIT Reset Command usage in real-time. How we use reset in practical scenarios in project - GIT
24. GIT Stash. When we need to use the stashing when switching the branches in GIT Project - GIT
25. GIT Stashing. Save and retrieve stash data using stash save, pop, list, and apply commands - GIT
26. Handle multiple stashes. Deleting and clear the stash data with stash id in the Project - GIT
27. Git Checkout. Different ways of using the checkout command in the Git Project - GIT.
28. GIT Restore and Switch command. Get the changes of file present in the particular commit - GIT
29. Git Revert Command. Difference between git Reset and the Revert command and when to use in GIT.
30. GITHUB Introduction. Difference between Git vs github. Why we need to use github - GIT.
31. Why we need to use GitHub. Advantages of having a Github Profile as a sort of resume - GIT
32. Git Clone. Cloning the remote repositories into machine using git clone command- GIT
33. Github SSH config Setup in the local machine. Add SSH key pair in the github account - GIT
34. Creating the first repository in GitHub. Get remotes list in the local git Repos project - GIT
35. Add, Rename & Remove Remote origin url to the Git Repo. What is Origin in Remote - GIT
36. Push the local repository Branch & commits to the Github repository using git push command - GIT
37. Pushing the local changes from one branch to another remote branch present in Github Repo - GIT
38. What git push -u mean? Set upstream for the local branch using -u option in push command - GIT
39. Difference between the main and the master branch in the Github Repository - GIT.
40. Remote Tracking Branches. Difference between local branch and the origin remote branch - GIT
41. Checkout the Remote tracking branches in the local git repository - GIT
42. Git Fetch Command. Get the latest changes from the remote repository into your local repo - GIT
43. Usage of the Git Fetch command for latest changes from remote repo in real time project - GIT.
44. Git Pull command. Update the current branch with the latest changes from remote repo in GIT.
45. Implementation of the git pull. Resolve merge conflicts for the changes from remote repo - GIT
46. Git Readme.md file. Learn how to write markdown syntax in the Readme file in Github Repo - GIT
47. What is Github Gist? How to use the Gists? Share & Display the code snippets using Gists - GIT
48. What are Github Pages? Free hosting with Github pages for the websites using github repo - Git
49. Creating Github pages in the Github Repository. Create User website and project sites - GIT
50. What are Pull Requests ? Create Pull request & approve in Github explained with example - GIT
51. Resolve conflicts for the feature branch when Pull request is raised in Github Repo - GIT
52. Add Collaborators and apply branch protection rules in Github for restricting commits - GIT
53. GitHub Fork. Why we use the fork and how to fork the project in the Github Repo's - GIT
54. Github Fork & Clone Workflow. Pull the changes from original to forked repo with Upstream 
55. Git Tagging. Difference between Lightweight Tags & Annotated Tags in the Git
56. Semantic Versioning for a Software. Understanding major, minor & Patch release in Version - GIT
57. Git Tag Commands. View tags list and Search Tags with name, checkout tag, diff between two tags
58. Creating Lightweight Tags in the git repository - GIT
59. Create Annotated Tags in Git Repository. See the details of the tag using git show tagname - GIT
60. Pushing Tags to the Github Remote Repository. Mark the tag as latest release in the github - GIT
61. Git Reflog Command. Get all log details of the reference using git reflog show command - GIT
62. Traversing the reflogs using name qualifiers and also time based qualifiers like yesterday - GIT
63. Get Back the lost commits in a branch with Reflogs - GIT
64. Create Git Aliases for the commonly used git commands - GIT
65. Completing Git Course. What we have learnt in the Git Course? Why we need to learn Git Tool?
