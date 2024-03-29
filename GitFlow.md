# A step by step guide to Git
# Step 1: Create a GitHub account


![Image](Dependency/git_guide1.png)

![Image](Dependency/git_guide2.png)

# Step 2: Create a new repository

A repository is like a place or a container where something is stored; in this case we're creating a Git repository to store code. To create a new repository, select New Repository from the + sign dropdown menu (you can see I've selected it in the upper-right corner in the image above).

![Image](Dependency/git_guide3.png)

Enter a name for your repository (e.g, "Demo") and click Create Repository.



# Step 3: Create a file

Create a new file from terminal and ignore the rest for now.

Open the Terminal program on your PC. 

or then again on Windows you can utilize cmd and guid it to the organizer where you stored the repo. 

with directions like cd,mkdir and rm.


![Image](Dependency/git_guide5.png)


Type git and hit Enter. If it says command bash: git: command not found, then install Git with the command for your Linux operating system or distribution. Check the installation by typing git and hitting Enter; if it's installed, you should see a bunch of information about how you can use the command.

In the terminal, type:

mkdir Demo
This command will create a directory (or folder) named Demo.

Change your terminal to the Demo directory with the command:

cd Demo
Then enter:

echo "#Demo" >> README.md
This creates a file named README.md and writes 

cat README.md
This will show you what is inside the README.md file, if the file was created correctly. 


To tell your computer that Demo is a directory managed by the Git program, enter:

git init
Then, to tell the Git program you care about this file and want to track any changes from this point forward, enter:

git add README.md

# Step 4: Make a commit

So far you've made a document and informed Git concerning it, and now it's an ideal opportunity to make a submit. Submit can be thought of as an achievement. Each time you achieve some work, you can do an git commit  to store that variant of your record, so you can return later and see what it resembled by then. At whatever point you roll out an improvement to your record, you make another rendition of that document, not the same as the past one.

# Step 5: Connect your GitHub repo with your computer

Now, it's time to connect your computer to GitHub with the command:

 **git config**

Usage: **git config –-global user.name &quot;[name]&quot;**

Usage: **git config –-global user.email &quot;[email address]&quot;**

This command sets the author name and email address respectively to be used with your commits.

![Image of Git Config](/Dependency/git_config.png)

Now you can learn basic commands of the git from this document.


# GitFlow


## **What Is GitFlow?**

GitFlow is a branching model for Git, created by Vincent Driessen. It has attracted a lot of attention because it is very well suited to collaboration and scaling the development team.

## **What is Version Control System (VCS)?**

Version control system is a system that records changes to a file or set of files over time so that you can recall specific versions later by using git command or various git tools available online. Suppose you are a developer and want to keep every version of code or after some particular tasks completion a Version Control System (VCS) is very useful tool. It allows you to revert files back to a previous state, compare changes over time, it allow you to take the other developer code changes using git command, see who modified the files over the time, who has done more number of lines of code, various type of statistics on the repository, who has done the code with bug and when, and many more, basically you can entirely do the tracking of the files over the time and go back to any previous changes.

## **How does Git record changes over the time work?**

Git story each commit a full copy of all the files, except that, for the content already present in the Git repo, the snapshot will simply point to said content rather than duplicate it. That also means that several files with the same content are stored only once. So a snapshot is basically a commit, referring to the content of a directory structure.
The major difference between Git and any other VCS (Subversion and friends included) is the way Git thinks about its data. Conceptually, most other systems store information as a list of file-based changes. These systems (CVS, Subversion, Perforce, Bazaar, and so on) think of the information they keep as a set of files and the changes made to each file over time

# Git Commands

## **git config**

Usage: **git config –-global user.name &quot;[name]&quot;**

Usage: **git config –-global user.email &quot;[email address]&quot;**

This command sets the author name and email address respectively to be used with your commits.

![Image of Git Config](/Dependency/git_config.png)

## **git init**

Usage: **git init [repository name]**

This command is used to start a new repository.

![Image of Git Init](/Dependency/git_init.png)


## **git clone**

Usage: **git clone [url]**

This command is used to obtain a repository from an existing URL.

![Image of Git Config](/Dependency/git_config.png)

## **git add**

Usage: **git add [file]**

This command adds a file to the staging area.

Usage: **git add \***

This command adds one or more to the staging area.

![Image of Git Config](/Dependency/git_add.png)

## **git commit**

Usage: **git commit -m &quot;[Type in the commit message]&quot;**

This command records or snapshots the file permanently in the version history.

Usage: **git commit -a**

This command commits any files you&#39;ve added with the git add command and also commits any files you&#39;ve changed since then.

![Image of Git Commit](/Dependency/git_commit.png)

## **git diff**

Usage: **git diff**

This command shows the file differences which are not yet staged.

 Usage: **git diff –staged**

This command shows the differences between the files in the staging area and the latest version present.

Usage: **git diff [first branch] [second branch]**

This command shows the differences between the two branches mentioned.

![Image of Git Diff](/Dependency/git_diff.png)

## **git reset**

Usage: **git reset [file]**

This command unstages the file, but it preserves the file contents.

Usage: **git reset [commit]**

This command undoes all the commits after the specified commit and preserves the changes locally.

Usage: **git reset –hard [commit]**  This command discards all history and goes back to the specific commit.

## **git status**

Usage: **git status**

This command lists all the files that have to be committed.

![Image of Git Status](/Dependency/git_status.png)

## **git rm**

Usage: **git rm [file]**

This command deletes the file from your working directory and stages the deletion.

![Image of Git RM](/Dependency/git_rm.png)

## **git log**

Usage: **git log**

This command is used to list the version history for the current branch.

Usage: **git log –follow[file]**

This command lists version history for a file, including the renaming of files also.

![Image of Git Log](/Dependency/git_log.png)

## **git show**

Usage: **git show [commit]**

This command shows the metadata and content changes of the specified commit.

![Image of Git show](/Dependency/git_show.png)

## **git tag**

Usage: **git tag [commitID]**

This command is used to give tags to the specific commit.

## **git branch**

Usage: **git branch**

This command lists all the local branches in the current repository.

Usage: **git branch [branch name]**

This command creates a new branch.

Usage: **git branch -d [branch name]**

This command deletes the feature branch.

![Image of Git branch](/Dependency/git_branch.png)

## **git checkout**

Usage: **git checkout [branch name]**

This command is used to switch from one branch to another.

Usage: **git checkout -b [branch name]**

This command creates a new branch and also switches to it.

![Image of Git Checkout2](/Dependency/git_checkout.png)

## **git merge**

Usage: **git merge [branch name]**

This command merges the specified branch&#39;s history into the current branch.

![Image of Git Merge](/Dependency/git_merge.png)


## **git remote**

Usage: **git remote add [variable name] [Remote Server Link]**

This command is used to connect your local repository to the remote server.

![Image of Git Merge](/Dependency/git_merge.png)

## **git push**

Usage: **git push [variable name] master**

This command sends the committed changes of master branch to your remote repository.

Usage: **git push [variable name] [branch]**

This command sends the branch commits to your remote repository.

Usage: **git push –all [variable name]**

This command pushes all branches to your remote repository.

Usage: **git push [variable name] :[branch name]**

This command deletes a branch on your remote repository.

![Image of Git Push](/Dependency/git_push.png)

![Image of Git Push](/Dependency/git_all1.png)

## **git pull**

Usage: **git pull [Repository Link]**

This command fetches and merges changes on the remote server to your working directory.

![Image of Git Pull](/Dependency/git_pull.jpeg)

## **Credit**

[https://dzone.com/articles/top-20-git-commands-with-examples](https://dzone.com/articles/top-20-git-commands-with-examples)

# [CLICK HERE TO GO TO README.MD](https://github.com/rutvik2611/miniproject1/blob/master/README.md)