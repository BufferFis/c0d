# Linux Basics and Forensics

## Introduction
This workshop covers essential Linux commands and concepts necessary for participating in Capture The Flag (CTF) competitions. It's designed for beginners and focuses on practical skills for navigating Linux systems and performing basic forensics tasks.

## Linux File System Structure
Linux uses a hierarchical file system structure. Key directories include:

- `/` (root): The top-level directory
- `/home`: User home directories
- `/etc`: System configuration files
- `/bin` and `/sbin`: Essential system binaries
- `/usr`: User utilities and applications
- `/var`: Variable data (logs, temp files)
- `/tmp`: Temporary files

## Essential Linux Commands

### Navigation and File Management
- `pwd`: Print working directory
- `ls`: List files and directories
  - Options: `-l` (long format), `-a` (show hidden files)
- `cd`: Change directory
  - `cd ..` to go up one level, `cd ~` to go to home directory
- `mkdir`: Create a new directory
- `touch`: Create an empty file or update timestamps
- `cp`: Copy files or directories
- `mv`: Move or rename files or directories
- `rm`: Remove files or directories
  - Use `-r` for directories, but be cautious!

### Viewing File Contents
- `cat`: Display entire file content
- `head`: Show the beginning of a file
- `tail`: Show the end of a file
- `less`: View file contents page by page

### File Permissions
- `chmod`: Change file permissions
  - Example: `chmod 777 file.txt`

### Searching and Filtering
- `grep`: Search for patterns in files
  - Example: `grep "password" file.txt`
- `find`: Search for files and directories
  - Example: `find . -name "flag.txt"`

### Other Useful Commands
- `file [filename]`: Determine file type
- `strings [filename]`: Extract readable text from binary files
- `tar -xvf [filename]`: Extract tar files
- `gunzip [filename]`: unzip .gz files

## Basic Forensics with The Sleuth Kit (TSK)
The Sleuth Kit is a collection of command-line tools for digital forensics.

Key TSK commands:
- `mmls`: Display partition information
- `fls`: List files and directories in an image
- `icat`: Output contents of a file given its inode number
- `blkcat`: Display contents of disk blocks

## CTF Tips
- Always check file permissions and hidden files
- Use `strings` on binary files to find readable text
- Combine commands with pipes (`|`) for efficient searching
- Practice regularly to improve your skills

## picoCTF questions
 - https://play.picoctf.org/practice/challenge/301 
 - https://play.picoctf.org/practice/challenge/300 
 - https://play.picoctf.org/practice/challenge/137 
 - https://play.picoctf.org/practice/challenge/285

## Solutions written to you (As i nuked my laptop i got nothing to work with) 
- I will share the solution of the hardest question which is shared in the end, you can go through it and figure it out on your own [wink wink]
- https://ctftime.org/writeup/33100
- This link has multiple write ups on it, you guys can go through a 

## Further Resources
- [Linux Command Line Cheat Sheet](https://cheatography.com/davechild/cheat-sheets/linux-command-line/)
- [OverTheWire Bandit Wargame](https://overthewire.org/wargames/bandit/) for practicing Linux skills
- [PicoCTF](https://picoctf.org/) for beginner-friendly CTF challenges
