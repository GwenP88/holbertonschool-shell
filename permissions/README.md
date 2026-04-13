# permissions

> Learning Linux permissions the hard way — one command, one mistake, one “ah okay I get it now” at a time.

---

## 📝 Description
In this project, I dive into Linux file permissions and user management using Bash. I learn how to control who can read, write, or execute files, and how to manage ownership and groups. This is where I start understanding that Linux is not just about commands — it’s about control (and sometimes frustration).

---

## 🎯 Learning Objectives
By the end of this project, I am able to explain how Linux permissions work without opening :contentReference[oaicite:0]{index=0} in panic mode.

I understand what commands like `chmod`, `chown`, `chgrp`, `sudo`, and `su` actually do, and more importantly, when and why to use them (instead of randomly trying things and hoping for the best).

I know how permissions are structured in Linux, how to read them, and how to convert them into numeric form without feeling personally attacked by octal notation.

I am able to change permissions, ownership, and groups of files, and I finally understand why a normal user can’t just `chown` everything (sad, but fair).

I can run commands with root privileges, switch users, and understand what it really means to become the superuser (spoiler: with great power comes great responsibility).

I also know how to create users and groups, check user IDs, display group memberships, and figure out who I actually am in the system (`whoami` — existential crisis avoided).


---

## 🛠️ Technologies Used
This project is built using Bash scripting on Ubuntu Linux. No fancy frameworks, just the terminal, core commands, and a lot of trial and error.


---

## ⚙️ Requirements
- OS: Ubuntu 22.04 LTS  
- Allowed editors: vi, vim, emacs  
- All scripts must be exactly two lines long  
- All files must end with a new line  
- The first line of all files must be exactly: `#!/bin/bash`  
- A README.md file at the root of the project is mandatory  
- You are not allowed to use backticks, `&&`, `||` or `;`  
- All files must be executable  
- Some tasks must be executed in the sandbox environment

---

## 🚀 Installation
```bash
git clone https://github.com/GwenP88/holbertonschool-shell.git
cd holbertonschool-shell/permissions
```

---

## ▶️ Usage / Execution
All Python scripts can be executed in two ways:

### 1. Direct execution
Make the file executable and run it directly:
```bash
chmod u+x filename
./filename
```

### 2. Using Bash interpreter
Run the script with Bash:
```bash
bash filename
```

---

## 📊 Project Progress
<p align="center">
<img src="assets/progress_barre_100.gif" alt="Mandatory tasks progress" width="80%">
</p>

<p align="center">
<sub>Mandatory tasks completion: 100%</sub>
</p>

---

## ✨ Features

### 0 - My name is Betty
- Mandatory task  
- Switch the current user to `betty`  
- Use exactly 8 characters for the command  
- The script changes the current user successfully  

**Files**: `0-iam_betty`

---

### 1 - Who am I
- Mandatory task  
- Print the effective username of the current user  
- No specific constraints  
- Displays the correct username  

**Files**: `1-who_am_i`

---

### 2 - Groups
- Mandatory task  
- Display all groups the current user belongs to  
- Output depends on the user  
- Shows all associated groups  

**Files**: `2-groups`

---

### 3 - New owner
- Mandatory task  
- Change the owner of file `hello` to `betty`  
- Must be executed with appropriate permissions  
- Ownership of the file is updated  

**Files**: `3-new_owner`

---

### 4 - Empty!
- Mandatory task  
- Create an empty file named `hello`  
- No constraints  
- File is created successfully  

**Files**: `4-empty`

---

### 5 - Execute
- Mandatory task  
- Add execute permission to the owner of `hello`  
- File must exist in working directory  
- Owner can execute the file  

**Files**: `5-execute`

---

### 6 - Multiple permissions
- Mandatory task  
- Add execute to owner and group, read to others  
- Must modify permissions correctly  
- Permissions are updated as expected  

**Files**: `6-multiple_permissions`

---

### 7 - Everybody!
- Mandatory task  
- Add execute permission to everyone  
- No commas allowed  
- All users can execute the file  

**Files**: `7-everybody`

---

### 8 - James Bond
- Mandatory task  
- Set permissions: owner/group none, others all  
- No commas allowed  
- Only others have full permissions  

**Files**: `8-James_Bond`

---

### 9 - John Doe
- Mandatory task  
- Set specific permission pattern  
- No commas allowed  
- Permissions match expected output  

**Files**: `9-John_Doe`

---

### 10 - Look in the mirror
- Mandatory task  
- Set `hello` permissions same as `olleh`  
- Must work for any permission value  
- Permissions are mirrored correctly  

**Files**: `10-mirror_permissions`

---

### 11 - Directories
- Mandatory task  
- Add execute permission to directories only  
- Must not affect regular files  
- Only directories are updated  

**Files**: `11-directories_permissions`

---

### 12 - More directories
- Mandatory task  
- Create `my_dir` with permission 751  
- Must set correct permissions at creation  
- Directory is created with expected mode  

**Files**: `12-directory_permissions`

---

### 13 - Change group
- Mandatory task  
- Change group owner of `hello` to `school`  
- Requires proper privileges  
- Group ownership is updated  

**Files**: `13-change_group`

---

### 14 - Owner and group
- Mandatory task  
- Change owner to `vincent` and group to `staff`  
- Apply to all files and directories  
- Ownership is updated everywhere  

**Files**: `14-change_owner_and_group`

---

### 15 - Symbolic links
- Mandatory task  
- Change owner and group of a symbolic link  
- Must target the link itself  
- Link ownership is updated correctly  

**Files**: `15-symbolic_link_permissions`

---

### 16 - If only
- Mandatory task  
- Change owner of `hello` only if owned by `guillaume`  
- Must check condition before applying  
- Ownership changes only when condition is met  

**Files**: `16-if_only`

---

## 🤝 Contributions & Acknowledgements
- Thanks to my peers and reviewers for their feedback
- Special thanks to the man pages — confusing at first, but always right

---

## 👤 Author
**Gwenaelle PICHOT**
- Student at Holberton School
- Track: holbertonschool-shell
- Project: permissions
