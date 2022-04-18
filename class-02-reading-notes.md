# Class 02 Reading Notes

## Text Editor 
Software that allows you write and edit text with ease!

### Ideal Features:
- **Code Completion**: displays possible suggestions as youre typing to speed up the process and reduce typos. Provides the necessary closing tag/bracket/quotation so that you dont forget. 
- **Syntax Highlighting**: Adds highlight or color to make text more noticeable. Assigns color to different elements to make them easier to spot. Makes everything easier to read and makes mistakes easier to find.
- **A Selection of Themes**: Adjust the appearance of your editor to help reduce eye strain and fatigue. A common set up has a dark back ground and bright text.
- **A Selection of Extensions**: As your experience grows, your text editor should too! Add extensions to enhance your performance while coding. Extensions add functionality. 

Most computers have a basic text editor intalled, for Mac it is called **Text Edit**. 

**Helpful clues**: 
- Be sure that you're typing in plain text - you shouldnt be able to bold, italic, or underline text - if you can, a setting needs to be changed. 
- Keep organized with folders! Store your entire website in a folder with sub-folders within. 
- Be sure you're saving with appropriate extensions - for example: HTML File saved with '.html'

**Third Party Options**: Notepadd++, Text Wrangler, BB Edit, Visual Studio Code, Atom, Brackets, and Sublime text - BE SURE to research the editor beforehand to make sure it is compatible with your computer and provides you with all the tools you need! 

As you become more experienced and want to experiment with more complicated code, consider an **IDE** which stands for Integrated Developemnt Environment. This is a combination of a text editor, a file manager, a compiler, and a debugger all in one!

## The Command Line 
Also known as the terminal - your system in text form! Type commands and recieve feedback.

#### How do I get to the terminal?
- MAC: Applications ➡️ Utilities ➡️ Terminal **OR** hit 'command + space' ➡️ Spotlight ➡️ type Terminal 
- LINUX: Applications ➡️ System OR Applications ➡️ Utilities **OR** right click on desktop ➡️ open in terminal 
- WINDOWS: You will need an SSH Client (ex: Putty) if you intend to remote log in to another terminal 


#### The terminal is open, now what?
Prompt ➡️ Command ➡️ Command Line Arguments 

- Add **SPACES** between the command & first command line argument 
- The **FIRST LINE ARGUMENT** is also called an **OPTION**, they modify the behavior of the command, they start with a dash (-)

When you hit **ENTER** the command runs, typically a list of outputs will appear under the command **OR** a task will be performed with no display (unless there is an error). Once the command is completed, a new prompt will appear.

**SHORTCUTS** - be quicker and prevent typos by accessing your commands history. Use the ⬆️ and ⬇️ arrow keys to explore previously used commands, then edit the command with the ⬅️ and ➡️ arrow keys. 

## The Shell 
Located within the terminal, the shell defines how the terminal acts and appears after running commands 

**BASH** is the most common shell, which stands for Bourne Again Shell 

- Run the command 'echo $SHELL' to find out what shell you're using 

## Basic Navigation 
Let's move around the system!

#### First of all, where am I?
Use the command 'pwd' which stands for Print Working Directory, to find out where you currently are in the system

#### What's here?
Use the command 'ls' which stands for List, to tell you what is in the location you're currently at
- Add an **OPTION** to your command 
  -   Command line option (-l) makes a long listing 
  -   Command line argument (/etc) does not list the current directory but instead lists its contents
  -   Command line option + argument (both -l and /etc) will make a long listing of the directory /etc

## Paths 
A means to get to a particular file or directory on the system 

#### Two Types of Paths
1. **ABSOLUTE** specifies a location in relation to the root directory. They always begin with a forward slash (/)
2. **RELATIVE** specifies a location in relation to where we currently are in the system. Does not begin with a forward slash (/)

#### Building Paths 
- A ~ (tilde) is a shortcut for your home directory 
- A . (dot) is a reference to your current directory 
- A .. (dot dot) is a reference to the parent directory 

Change your directory with the command 'cd [location]' - **NOTE** with no argument, 'cd' will take you to your home directory 

**SHORTCUT** Tab Completion: while typing a path, hit the **TAB KEY** to search for an autocomplete action. If nothing appears, then there are a lot of options, you can still list them by hitting tab again. 

## Files 
Everything is a file - text files, a directory, your keyboard, your monitor, etc!

- Linux is extensionless meaning that it knows what kind of file a particular file is without a specified extension. For example: a photo will be known as a photo whether the file ends in .jpg, .txt, or .exe! 
- To find out what type of file something is, use command: **file [path]**
- Linus is **case sensitive**!! Watch out or capitol and lowercase letters in the file names and even your commands!
- **SPACES** separate items! If your directory name has a space in it, type the command between quotes (ex: 'holiday photos') **OR** use an escape character (\) before the character which you want to nulify (ex: holiday\ photos)

**HIDDEN FILES**
- If the name begins with a . (full stop), then it is hidden
- You can create a hidden file by adding the . at the beginning, and you can un-hide a file by deleting the . 
- Add option -a to show hidden files as well! 

[Return home](https://khofstetter94.github.io/reading-notes/)

