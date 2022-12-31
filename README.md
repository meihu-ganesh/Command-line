# Command-line

<!-- # Command Line Interface
- Command Line Interface (CLI) facilitates the users to perform powerful operations on a computer with simple commands.
- Command is a text instruction to a computer program to perform a specific task.
![link](./images/cmd.webp)
## What is Shell?
- Shell is the  software that interprets and executes the various commands that we provide.
- Terminal is a text input/output environment.
### Different Shells
- Bourne Shell (sh)
- Bourne-Again Shell (bash)
- C Shell (csh)
- Korn Shell (ksh)
- Z Shell (zsh)
## Opening Terminal
Bash is one of the most commonly used shell in Linux distributions.
- Open the Dash (Super Key) or Applications and type terminal.
- Shortcut: ``Ctrl + Alt + T`` -->




## Listing Files & Directories
`ls` &nbsp;  is used to list files and directories.
```bash
ls
```
### Using Additional Options
- `ls -l -h` option provides details in human readable format.
![link](./images/ls_detail.webp)
- Some options require values arguments/values to be passed.
    - `--block-size` &nbsp; option rounds the file size to nearest values.
    - Inputs: &nbsp;`KB , MB`
![link](./images/ls-size.webp)
## Get Options for Commands
`help` &nbsp; displays a list of options that you can use with the command. 
```bash
ls --help
```   
This Command will be helpful when you don’t know about its parameters and return type etc.
## Clear the Screen
- `clear` &nbsp; command clears the terminal.
- Shortcut: &nbsp; `Ctrl+L`
```bash
clear
```
## Get User Manual for Commands
- `man` &nbsp; displays the user manual of a command .
- Here we pass the command as an argument.
#### syntax : 
```bash
man <command>
```
#### example :
```bash
man ls
```
- Type &nbsp; `q` &nbsp; to exit the manual
## Get System Date & Time 
`date` &nbsp; displays the system date and time.
```bash
date
```
## Get Current User
`whoami` &nbsp; displays the current logged in user
```bash
whoami
```
## Previous Commands
- Shell keeps track of the commands you have typed in.
- Use up ( ⬆) and down ( ⬇) arrows to access the commands.
## History
- `history` &nbsp; displays the history of the commands you have typed in so far.
- By default, It shows the last 500 recent commands.
```bash
history
```
## Bash History
Bash maintains the history to *. bash_history* file.
```bash
cat .bash_history
```
## Exit
`exit` &nbsp; to close/end a shell session.
```bash
exit
```
# Working With Files
## Creating a File
`touch` &nbsp;  creates an empty file.
```bash
touch filename
```
## Viewing File Content
`cat` &nbsp; eads contents of file and prints it.
```bash
cat filename
```
## Echo
`echo` &nbsp; output/prints a string in the terminal.
```bash
echo "content"
```
## Writing to Files Using echo Command
Using > (greater than) operator we can redirect the output of echo command to a file.
```bash
echo "Hello World!" > filename
```
## Renaming a File
-`mv` &nbsp; renames the file names.
- *destination* can be a new or existing file.
#### Syntax :
```bash
mv source destination
```
#### Example :
```bash
mv practice.txt exam.txt
```
## Copying Files
`cp` &nbsp; copies src_file to dest_file.
#### syntax :
```bash
cp src_file dest_file
```
#### Example :
```bash
cp exam.txt fun_text.txt
```
**Note :** If dest_file already exist then &nbsp; `cp` &nbsp; overrides the contents of dest_file.
## Deleting a File
`rm` &nbsp; removes (delete) files.
#### syntax :
```bash
rm filename
```
#### example :
```bash
rm exam.txt
```
## Hidden Files
- Linux, by default, hides many of the sensitive system files, in order to avoid accidental changes.
- Hidden files starts with "."
- `ls a` &nbsp; shows the hidden files.
- `ls a` &nbsp; also shows the current and parent directories:
    - `.` represents `Current directory`
    - `..` represents `parent directory`
```bash
ls -a
```
    