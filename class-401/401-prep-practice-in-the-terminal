# Prep: Practice in the Terminal

[Bash Command Line Tutorials](https://ryanstutorials.net/linuxtutorial/)

## The Command Line

- You can have multiple command lines up and running doing different tasks
- "A command line, or terminal, is a text based interface to the system. You are able to enter commands by typing them on the keyboard and feedback will be given to you similarly as text."
- first you type a command then arguments to follow
- "Options are typically used to modify the behaviour of the command. Options are usually listed before other arguments and typically start with a dash ( - )."
- On a Mac you can press 'command + space' to bring up the finder and search for the terminal
- Type 'echo $SHELL' to find out what shell you are currently using

## Basic Navigation

- 'pwd' command stands for Print Working Directory and displays what your current working directory is
- 'ls' command stands for list and will show you what is at your current working directory
- using '-l' after 'ls' will give a long listing with more details about what is available
- "Whenever we refer to either a file or directory on the command line, we are in fact referring to a path. ie. A path is a means to get to a particular file or directory on the system."
- The hierarchical structure of the file system begins with the root directory at the top and is denoted by a '/'
- Absolute paths begin with a '/' and specify a location in relations to the root directory. Relative paths do not begin with a '/' and specify a location in relation to where we currently are in the system
- "~ (tilde) - This is a shortcut for your home directory. eg, if your home directory is /home/ryan then you could refer to the directory Documents with the path /home/ryan/Documents or ~/Documents
- . (dot) - This is a reference to your current directory. eg in the example above we referred to Documents on line 4 with a relative path. It could also be written as ./Documents (Normally this extra bit is not required but in later sections we will see where it comes in handy).
- .. (dotdot)- This is a reference to the parent directory. You can use this several times in a path to keep going up the hierarchy. eg if you were in the path /home/ryan you could run the command ls ../../ and this would do a listing of the root directory.
- Use 'cd \[location]' to change the directory you are in
- Use Tab Completion to auto complete your typing so that you dont have to type the entire thing out

## More About Files

- "under the hood, everything is actually a file"
- common extensions:
  - file.exe - an executable file, or program.
  - file.txt - a plain text file.
  - file.png, file.gif, file.jpg - an image.
- Use command 'file \[path]' to find out what type of file a particular file is
- Linux is case sensitive!
- Spaces in a command are seen as two different command arguments, use quotes or escape characters to have the multiple word title be seen as one or to ignore the spaces
- If the file or directory's name begins with a . (full stop) then it is considered to be hidden
- Add command option '-a' after 'ls' so that hidden files are also displayed

## Manual Pages

- "The manual pages are a set of pages that explain every command available on your system including what they do, the specifics of how you run them and what command line arguments they accept", use command 'man \<command to look up>' to invoke it.
- Do a keyword seach on the manual pages by using command 'man -k \<search term>'
- use '/\<term>' within a manual page to perform a search for a certain term
- Long hand command line options ('--all instead of -a') begin with two dashes, this method is nice because you can better understand what the commands are doing

## File Manipulation

- To make a directory use 'mkdir \[options] \<Directory>'
- a few more examples of how we can supply a directory to be created
  - mkdir /home/ryan/foo
  - mkdir ./blah
  - mkdir ../dir1
  - mkdir ~/linuxtutorialwork/dir2
- Adding the option '-p' creates parent directories as needed
- And '-pv' makes mkdir tell us what it is doing
- To remove a directory use command 'rmdir \[options] \<Directory>', however a directory must be empty to be removed
- Create blank files with command 'touch \[options] \<filename>'
- To duplicate a file or directory use command 'cp \[options] \<source> \<destination>'
- "Using the -r option (which stands for recursive) means that we want to look at a directory and all files and directories within it, and for subdirectories, go into them and do the same thing and keep doing this."
- to move a file use command 'mv \[options] \<source> \<destination>
- To remove or delete a file use command 'rm \[options] \<file>', WARNING: this cannot be undone
- Adding the '-r' recursive option will remove directories and all files and directories contained within, using option 'i' with 'r' which will give you a prompt confirming the deletion and the option to cancel

[CHEAT SHEAT!](https://ryanstutorials.net/linuxtutorial/cheatsheet.php)

[Return home](https://khofstetter94.github.io/reading-notes/)
