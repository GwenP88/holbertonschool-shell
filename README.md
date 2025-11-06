# Holberton School – Shell

> **Training module: Shell, Bash & Unix Commands**

This repository contains all the projects and exercises from the **Shell** module of the **Holberton School** training course.  
Its aim is to teach students how to use the terminal effectively, automate tasks, and understand how the Linux system works through the Bash shell.

- [Presentation](#-presentation)
- [Educational objectives](#-educational-objectives)
- [Project structure](#-project-structure)
- [Script execution](#-script-execution)
- [Technical constraints](#-technical-constraints)
- [Skills acquired](#-skills-acquired)
- [Author](#-author)
- [Licence](#-licence)
- [Acknowledgements](#-acknowledgements)

---

## Introduction

This project is part of the **Holberton School core curriculum** and provides an essential introduction to the Linux environment.  
The goal is to **understand the basics of the Bash shell**, learn how to write **simple but robust scripts**, and master the **fundamental commands** for file management, permissions, and redirections.

Each folder corresponds to a specific topic, with exercises of increasing difficulty.

---

## Learning objectives

- Discover and understand how the **Unix shell** works
- Manipulate **files and directories** from the command line
- Use **redirections**, **pipes** and **filters**
- Manage **permissions** and **access rights**
- Create and execute **automated Bash scripts**
- Use **variables**, **expansions** and **built-in commands**
- Follow **good scripting practices** and Bash syntax

---

## Project Tree Structure

holbertonschool-shell/
│
├── basics/
│   ├── 0-current_working_directory
│   ├── 1-listit
│   ├── 2-bring_me_home
│   ├── 3-listfiles
│   ├── 4-listmorefiles
│   ├── 5-listfilesdigitonly
│   ├── 6-firstdirectory
│   ├── 7-movethatfile
│   ├── 8-firstdelete
│   ├── 9-firstdirdeletion
│   ├── 10-back
│   ├── 11-lists
│   ├── 12-file_type
│   ├── 13-symbolic_link
│   └── 14-copy_html
│
├── init_files_variables_and_expansions/
│   ├── 0-alias
│   ├── 1-hello_you
│   ├── 2-path
│   ├── 3-paths
│   ├── 4-global_variables
│   ├── 5-local_variables
│   ├── 6-create_local_variable
│   ├── 7-create_global_variable
│   ├── 8-true_knowledge
│   ├── 9-divide_and_rule
│   ├── 10-love_exponent_breath
│   ├── 11-binary_to_decimal
│   ├── 12-combinations
│   ├── 13-print_float
│   └── 14-decimal_to_hexadecimal
│
├── io_redirections_and_filters/
│   ├── 0-hello_world
│   ├── 1-confused_smiley
│   ├── 2-hellofile
│   ├── 3-twofiles
│   ├── 4-lastlines
│   ├── 5-firstlines
│   ├── 6-third_line
│   ├── 7-file
│   ├── 8-cwd_state
│   ├── 9-duplicate_last_line
│   ├── 10-no_more_js
│   ├── 11-directories
│   ├── 12-newest_files
│   ├── 13-unique
│   ├── 14-findthatword
│   ├── 15-countthatword
│   ├── 16-whatsnext
│   ├── 17-hidethisword
│   ├── 18-letteronly
│   ├── 19-AZ
│   ├── 20-hiago
│   ├── 21-reverse
│   └── 22-users_and_homes
│
└── permissions/
    ├── 0-iam_betty
    ├── 1-who_am_i
    ├── 2-groups
    ├── 3-new_owner
    ├── 4-empty
    ├── 5-execute
    ├── 6-multiple_permissions
    ├── 7-everybody
    ├── 8-James_Bond
    ├── 9-John_Doe
    ├── 10-mirror_permissions
    ├── 11-directories_permissions
    ├── 12-directory_permissions
    └── 13-change_group

---

## Running Scripts

Clone the repository:
`git clone`
[Link to repository](git clone https://github.com/GwenP88/holbertonschool-shell.git)

Navigate to the project directory:
`cd holbertonschool-shell`

Make a script executable:
`chmod +x script_name`

Run the script:
`./script_name`
All scripts are tested on Ubuntu 20.04 LTS with bash (version 5.x)

---

## Technical Constraints

Interpreter: #!/bin/bash on the first line of each script
No unauthorized commands or options may be used
Files must be executable and free of syntax errors
Scripts must adhere to the format required by Holberton (Betty linter)
Files must not contain superfluous characters (spaces, unnecessary returns)

---

## Skills Acquired

Mastery of basic commands (ls, cd, pwd, mv, cp, rm, mkdir, etc.)
Managing access rights (chmod, chown, chgrp)
Using variables and expansions
Input/output redirection and using pipes
Manipulating text streams (grep, cut, tr, sort, uniq, wc, head, tail, etc.)
Creating automated scripts
Adherence to Bash best practices (syntax, comments, readability)
---

## Author

Gwen Pichot
Web Development Student – ​​[Holberton School](https://www.holbertonschool.fr/)

Haute-Savoie, France
[GitHub Profile](https://github.com/GwenP88)

---

## License

This project is published under the MIT license.

You are free to use, modify, and redistribute it as long as the original license is retained.

---

## Acknowledgments

Project completed as part of the Holberton School – Foundations program
“The best way to learn coding is by doing.”

