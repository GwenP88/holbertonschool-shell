![Shell Basics Banner](/assets/Holberton.png)

# Shell Basics – Holberton School Project

## Introduction
This project marks a key milestone in my journey with Holberton School. Before diving into C language, algorithms, and collaborative projects, I needed to gain a solid understanding of the terminal and understand what really happens ‘under the hood’ when interacting with a machine.  
Shell Basics was my first real contact with the Unix environment in real conditions: writing my own scripts, automating tasks, navigating the tree structure properly, understanding the machine's responses and becoming autonomous thanks to the documentation.  
It's a demanding but formative project: it forced me to understand, not just execute. And that's exactly the Holberton approach — learning by doing, experimenting, and correcting my mistakes.
This README therefore outlines what I learned, the fundamental concepts I integrated, and the details of each exercise completed in this first Shell Basics module.

---

## Concepts learned
- **RTFM**: autonomy, proactive research, systematic reading of documentation.
- **Shebang**: definition of the interpreter to be used to execute a script.  
- **Shell**: programme that interprets user commands.  
- **Terminal vs Shell**:  
  - terminal = input/output interface  
  - shell = interpreter that executes commands  
- **Shell prompt**: entry point ready to receive a command.  
- **History**: recall, re-execution, workflow optimisation.
- File system manipulation (navigation, creation, deletion, permissions).
- Management of hidden files, symbolic links, tree structures.
- Automation using Bash scripts.

---

## Project exercises

### `0-current_working_directory`
**Instruction:** display the absolute path of the current directory.  
**Constraint:** none.  
**What I learned:** understanding the concept of the current directory and the importance of absolute paths.


### `1-listit`
**Instruction:** Display the list of contents in the current directory.  
**Constraint:** None.  
**What I learned:** Quickly read the structure of a folder using basic commands.


### `2-bring_me_home`
**Instruction:** move to the home directory.  
**Constraint:** do not use shell variables.   
**What I learned:** use robust commands that are independent of environment variables.


### `3-listfiles`
**Instruction:** display the content in long format.  
**Constraint:** none.  
**What I learned:** read file permissions, owners, and metadata.


### `4-listmorefiles`
**Instruction:** display the content in long format with hidden files.  
**Constraint:** none.  
**Expected result:** display including `.` and `..`.  
**What I learned:** manipulate and display hidden files on the system.


### `5-listfilesdigitonly`
**Instruction:** display content in long format, numerical IDs, including hidden files.  
**Constraint:** display UID and GID as numbers.   
**What I learned:** interpret system IDs and not just user names.


### `6-firstdirectory`
**Instruction:** Create `/tmp/my_first_directory`.  
**Constraint:** None.  
**What I learned:** Creating directories in system locations.


### `7-movethatfile`
**Instruction:** Move `betty` to `/tmp/my_first_directory`.  
**Constraint:** File initially located in `/tmp`.  
**What I learned:** Manipulating and moving files via script.


### `8-firstdelete`
**Instruction:** delete the file `betty`.  
**Constraint:** file present in the folder.  
**What I learned:** delete cleanly and verify the absence of a file after an action.


### `9-firstdirdeletion`
**Instruction:** delete the `my_first_directory` folder.  
**Constraint:** folder must be empty.   
**What I learned:** differentiate between deleting a file and deleting a folder.


### `10-back`
**Instruction:** return to the previous directory.  
**Constraint:** none.  
**What I learned:** how to navigate efficiently through the directory history.


### `11-lists`
**Instruction:** list in long format: current directory, parent, then `/boot`.  
**Constraint:** be careful with absolute paths.  
**What I learned:** combine multiple locations in a single command.


### `12-file_type`
**Instruction:** display the file type of `/tmp/iamafile`.  
**Constraint:** use the appropriate command.  .  
**What I learned:** analyse the actual nature of a file, regardless of its extension.


### `13-symbolic_link`
**Instruction:** create a symbolic link `__ls__` to `/bin/ls`.  
**Constraint:** link in the current directory.  
**What I learned:** create and use symbolic links to system binaries.


### `14-copy_html`
**Instruction:** Copy only the most recent or non-existent `.html` files to the parent directory.  
**Constraint:** Consider only `.html` files.    
**What I learned:** Manipulate conditional copying based on date comparison.


### `15-lets_move`
**Instruction:** Move all files beginning with a capital letter to `/tmp/u`.  
**Constraint:** `/tmp/u` already exists.   
**What I learned:** How to use patterns (globbing) to filter files.


### `16-clean_emacs`
**Instruction:** delete all files ending with `~`.  
**Constraint:** none.   
**What I learned:** automate the cleaning of files generated by editors.


### `17-tree`
**Instruction:** create `welcome/`, `welcome/to/` and `welcome/to/school`.  
**Constraint:** **maximum 2 lines**, **maximum 2 spaces**.  
**What I learned:** optimising script writing under strict constraints (syntax and compactness).

---

## Conclusion
Thanks to this project, I consolidated the essential skills needed to work in a professional Unix environment: navigation, inspection, file manipulation, automation, rigour, and understanding of how the shell actually works.  
It is a seemingly simple project, but one that was decisive in shaping my methodology. It was also the moment when I truly realised that I was embarking on a demanding, practical journey designed to push me to think like a developer.
