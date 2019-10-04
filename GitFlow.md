# GitFlow


**What Is GitFlow?**

GitFlow is a branching model for Git, created by Vincent Driessen. It has attracted a lot of attention because it is very well suited to collaboration and scaling the development team.

**What is Version Control System (VCS)?**

Version control system is a system that records changes to a file or set of files over time so that you can recall specific versions later by using git command or various git tools available online. Suppose you are a developer and want to keep every version of code or after some particular tasks completion a Version Control System (VCS) is very useful tool. It allows you to revert files back to a previous state, compare changes over time, it allow you to take the other developer code changes using git command, see who modified the files over the time, who has done more number of lines of code, various type of statistics on the repository, who has done the code with bug and when, and many more, basically you can entirely do the tracking of the files over the time and go back to any previous changes.

**How does Git record changes over the time work?**

Git story each commit a full copy of all the files, except that, for the content already present in the Git repo, the snapshot will simply point to said content rather than duplicate it. That also means that several files with the same content are stored only once. So a snapshot is basically a commit, referring to the content of a directory structure.
The major difference between Git and any other VCS (Subversion and friends included) is the way Git thinks about its data. Conceptually, most other systems store information as a list of file-based changes. These systems (CVS, Subversion, Perforce, Bazaar, and so on) think of the information they keep as a set of files and the changes made to each file over time

# Git Commands

**git config**

Usage: git config –-global user.name &quot;[name]&quot;

Usage: git config –-global user.email &quot;[email address]&quot;

This command sets the author name and email address respectively to be used with your commits.

![Image of Git Config](/Dependency/git_config.png)

**git init**

Usage: git init [repository name]

This command is used to start a new repository.

![Image of Git Init](/Dependency/git_init.png)


**git clone**

Usage: git clone [url]

This command is used to obtain a repository from an existing URL.

![Image of Git Config](/Dependency/git_config.png)

**git add**

Usage: git add [file]

This command adds a file to the staging area.

Usage: git add \*

This command adds one or more to the staging area.

![Image of Git Config](/Dependency/git_add.png)

**git commit**

Usage: git commit -m &quot;[Type in the commit message]&quot;

This command records or snapshots the file permanently in the version history.

Usage: git commit -a

This command commits any files you&#39;ve added with the git add command and also commits any files you&#39;ve changed since then.

![Image of Git Commit](/Dependency/git_commit.png)
**git diff**

Usage: git diff

This command shows the file differences which are not yet staged.

 Usage: git diff –staged

This command shows the differences between the files in the staging area and the latest version present.

Usage: git diff [first branch] [second branch]

This command shows the differences between the two branches mentioned.

![Image of Git Diff](/Dependency/git_diff.png)

**git reset**

Usage: git reset [file]

This command unstages the file, but it preserves the file contents.

Usage: git reset [commit]

This command undoes all the commits after the specified commit and preserves the changes locally.

Usage: git reset –hard [commit]  This command discards all history and goes back to the specific commit.

**git status**

Usage: git status

This command lists all the files that have to be committed.

![Image of Git Status](/Dependency/git_status.png)
**git rm**

Usage: git rm [file]

This command deletes the file from your working directory and stages the deletion.

![Image of Git RM](/Dependency/git_rm.png)

**git log**

Usage: git log

This command is used to list the version history for the current branch.

Usage: git log –follow[file]

This command lists version history for a file, including the renaming of files also.

![Image of Git Log](/Dependency/git_log.png)

**git show**

Usage: git show [commit]

This command shows the metadata and content changes of the specified commit.

![Image of Git show(/Dependency/git_show.png)

**git tag**

Usage: git tag [commitID]

This command is used to give tags to the specific commit.

**git branch**

Usage: git branch

This command lists all the local branches in the current repository.

Usage: git branch [branch name]

This command creates a new branch.

Usage: git branch -d [branch name]

This command deletes the feature branch.

![Image of Git branch](/Dependency/git_branch.png)

**git checkout**

Usage: git checkout [branch name]

This command is used to switch from one branch to another.

Usage: git checkout -b [branch name]

This command creates a new branch and also switches to it.

![Image of Git Checkout2](/Dependency/git_checkout2.png.png)

**git merge**

Usage: git merge [branch name]

This command merges the specified branch&#39;s history into the current branch.

**git remote**

Usage: git remote add [variable name] [Remote Server Link]

This command is used to connect your local repository to the remote server.

**git push**

Usage: git push [variable name] master

This command sends the committed changes of master branch to your remote repository.

Usage: git push [variable name] [branch]

This command sends the branch commits to your remote repository.

Usage: git push –all [variable name]

This command pushes all branches to your remote repository.

Usage: git push [variable name] :[branch name]

This command deletes a branch on your remote repository.

![Image of Git Push](/Dependency/git_push.png)

![Image of Git Push](/Dependency/git_all1.png)

**git pull**

Usage: git pull [Repository Link]

This command fetches and merges changes on the remote server to your working directory.

**Credit**

[https://dzone.com/articles/top-20-git-commands-with-examples](https://dzone.com/articles/top-20-git-commands-with-examples)