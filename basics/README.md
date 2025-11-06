# Module “Basics” – Shell Scripting

This folder contains the first exercises of the **Shell** module of the **Holberton School** course.

It serves as an introduction to Unix commands and file system manipulation via the terminal.

---

## Overview

The goal of this series of exercises is to learn how to navigate and interact within a Linux environment using the Bash shell.
These exercises lay the necessary foundation for understanding how the system works and for writing automated scripts.
Each file in this folder corresponds to a specific exercise required by the course.

---

## Learning Objectives

Upon completion of this module, students should be able to:
- Navigate a Linux directory tree using basic commands (`pwd`, `ls`, `cd`, etc.).
- Create, move, copy, and delete files and directories.
- Distinguish between different file types and understand symbolic links.
- Manage access rights and understand the concept of permissions.
- Write simple Bash scripts that adhere to Holberton conventions (Betty linter).

---

## Folder contents

basics/
├── 0-current_working_directory
├── 1-listit
├── 2-bring_me_home
├── 3-listfiles
├── 4-listmorefiles
├── 5-listfilesdigitonly
├── 6-firstdirectory
├── 7-movethatfile
├── 8-firstdelete
├── 9-firstdirdeletion
├── 10-back
├── 11-lists
├── 12-file_type
├── 13-symbolic_link
└── 14-copy_html

Each file contains a Bash script that fulfills a specific instruction in the Holberton program.

---

## Exercise Details

| `0-current_working_directory` | Displays the absolute path of the current directory. |
| `1-listit` | Lists the contents of the current directory. |
| `2-bring_me_home` | Changes the current directory to the home directory. |
| `3-listfiles` | Lists the files in the current directory in verbose format. |
| `4-listmorefiles` | Lists all files, including hidden files. |
| `5-listfilesdigitonly` | Lists files, displaying the numeric identifiers of users and groups. |
| `6-firstdirectory` | Creates a directory named `my_first_directory` in `/tmp/`. |
| `7-movethatfile` | Moves a file `betty` from `/tmp/` to `/tmp/my_first_directory/`. |
| `8-firstdelete` | Deletes the file `betty` located in `/tmp/my_first_directory/`. |
| `9-firstdirdeletion` | Deletes the directory `/tmp/my_first_directory/`. |
| `10-back` | Changes the current directory to the previous one. |
| `11-lists` | Lists all files, including those in subdirectories, in a detailed format. |
| `12-file_type` | Displays the type of the file named `iamafile`. |
| `13-symbolic_link` | Creates a symbolic link `__ls__` pointing to `/bin/ls`. |
| `14-copy_html` | Copies all missing or newer `.html` files to the parent directory. |

---

## Execution Instructions

Clone the repository:
[Link to repository](git clone https://github.com/GwenP88/holbertonschool-shell.git)

Navigate to the folder:
`cd holbertonschool-shell/basics`

Make a script executable:
`chmod +x script_name`

Run the script:
`./script_name`
All scripts were designed to run on an Ubuntu 20.04 LTS environment with bash version 5.x.

---

## Technical Constraints

Each script must begin with the shebang:
`#!/bin/bash`
No unauthorized commands should be used. Scripts must be valid and free of syntax errors.

Each file must be executable: `chmod +x script_name`
The code must adhere to Holberton conventions and pass the Betty linter.

---

## Best Practices
Test each command before integrating it into a script.
Check permissions before executing or deleting a file.
Comment important parts of the code to explain the intent.
Always save before modifying a system file.

Run scripts in a test environment before production.

---

## Author

Gwen Pichot
Web Development Student – ​​[Holberton School](https://www.holbertonschool.fr/)

Haute-Savoie, France
[GitHub Profile](https://github.com/GwenP88)

---

## License

This project is released under the MIT license.

You are free to use, modify, and redistribute it as long as the original license remains in effect.

---

## Acknowledgements

Project completed as part of the Holberton School – Foundations program

“The best way to learn coding is by doing.”
