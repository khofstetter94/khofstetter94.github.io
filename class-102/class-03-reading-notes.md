# Git Intro

For full blog, click [here](https://blog.udemy.com/git-tutorial-a-comprehensive-guide/#7_2)

## Version Control System (VCS)

A system that saves multiple versions of a file. This allows tracking of changes, reverting back to a previous version, tracking modifications along with their creators, and comparing changes.

- **Local Version Control**: One database on your hard disk that stores changes to files
- **Centralized Version Control (CVCS)**:  Better for collaboration, entails a single server storing all changes and versions, can be accessed by multiple clients. Team members can track changes and activity from other members.
- **Distributed Version Control (DVCS)**: Allows clients to create mirrored repositories. Data backups can be easily used to replace any lost information. Solves the issue of the CVS being a single point of failure.

### Git

- Git is a DVCS that stores data in a file system made up of snapshots. Git records and saves a snapshot of all changes to a project (commits)
- Git relies on local operations due to important information being found on the local disk, this allows work to be done offline or when not on a VPN
- Git tracks all changes and detects file corruption
- Git makes you jump through hoops in order to completely lose data, preventing accidents
- The states of Git: **Committed** (data stored in a local database), **Modified** (file has been changed, but not committed), **Staged** (Flagged changed version to be commited in next snapshot)

### Let's Get Started

Download Git:

  1. Install as a package
  2. Install via another installer
  3. Download and compile the source code

- Max OS, Windows, and Linux all have different methods for download, click the blog link above to read about the specifics for your system

*If you would like Graphical User Interface (GUI) tools, visit this [link](https://git-scm.com/downloads/guis) for options*

### Initial Customization

**Configuration of Variables**: Use Git tool **git config**
**Identity Setting**: set your username and email address to be used for every Git commit

  In the terminal type:

      git config --global user.name "Jane Smith"

      git config --global user.email "example@email.com"

**Default Text Editor**: Git uses your system's default editor, to switch editors, type into your command line:

      '$ git config --global core.editor (name of editor)'

- **Note** Some editors require specific instructions

**Check Your Setting**: Use the '**git config --list**' command

### Setting Up a Git Repository

**Importing**
To import an existing project or directory into Git, type into your terminal:

1. Switch to target project's directory: $ cd test (cd = change directory)
2. Use the git init command: $ git init
3. Start tracking these files:
    - $ git add *.c
    - $ git add LICENSE
    - $ git commit -m “any message here”

**Cloning**
Clone an existing repository from a particular server with clone command: $ git clone 'the repository's URL'

- This will create copies of all versions of all files for a project.

### Workflow

Local Repository Structure:

1. Working Directory: The actual files reside here
2. Index: The area used for staging
3. Head: Points to the most recent commit

### Saving Changes

- Tracked: files can be modified, unmodified, or staged
- Untracked: files not a part of the last snapshot, do not currently reside in the staging area

### The Life cycle of File Status

unmodified ➡️ edit the file ➡️ modified ➡️ stage the file ➡️ staged ➡️ commit the file ➡️ unmodified

### Tracking and Staging a New File

- Single File: use format 'git add filename'
- All Files: use command '$ git add *'

### Committing a File

After staging, commit the changes and write a commit message of what you did

- $ git commit -m “made change x,y,z”
- To commit all changes - $ git commit -a

### Pushing Changes

- $ git push origin master

This command pushes changes from the local "master" branch to the remote repository named "origin"

### Stashing Changes

- Use 'git stash' to store changes that you dont want to commit yet
- Use 'git stash apply' to retrieve hidden changes

### Remote Repositories

Versions of a project found online or on a network - push and pull data from these repositories!

- Cloned repositories: "origin" is the name of the initial server that got cloned, and "master" is your local branch

### Seeing Your Remotes

- Run 'git remote' command to view short names of remote handles
- Run 'git remote -v' to view all remote URLs and their short names

[Return home](https://khofstetter94.github.io/reading-notes/)
