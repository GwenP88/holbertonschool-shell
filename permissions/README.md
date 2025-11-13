# Shell Permissions – Holberton School Project

## Introduction
This project marked a real shift in my understanding of how a Unix system works. After learning how to navigate through directories and write basic scripts in the “Shell Basics” module, I finally had to deal with one of the most sensitive and fundamental aspects of Linux: permissions, ownership, groups, and identity management.  
This is also when I realized how much the security and structure of a system rely on those mechanisms. There is no way to progress in C, DevOps, or system administration without mastering these foundations.  
Working on this module pushed me to read man pages carefully, experiment, break things, fix them, and—most importantly—understand why an action succeeds or fails depending on the active user.  
This README summarizes the key concepts I learned and what each exercise taught me.

---

## Concepts Learned
- Understanding **Linux permissions** (rwx, numeric mode, symbolic mode).  
- Key commands:
  - `chmod`: change permissions  
  - `sudo`: run commands with elevated privileges  
  - `su`: switch user  
  - `chown`: change file owner  
  - `chgrp`: change file group  
- How to represent permissions (owner / group / others) with digits from 0 to 7.  
- How to modify permissions, owners, and groups.  
- Why a normal user **cannot** change file ownership.  
- How to run commands as **root** safely.  
- How to change user ID or become superuser.  
- How to create users and groups.  
- How to display real and effective UIDs and GIDs.  
- How to handle symbolic links safely.  
- How conditional ownership changes work.  

---

## Exercises

### `0-iam_betty`
**Instruction:** Switch the current user to *betty*.  
**Constraint:** Exactly **8 characters** (plus newline).  
**What I learned:** Understanding how to switch users and the difference between real and effective user identity.


### `1-who_am_i`
**Instruction:** Print the effective username of the current user.  
**Constraint:** None.  
**What I learned:** Identifying the effective user that executes a command.


### `2-groups`
**Instruction:** Print all groups the current user belongs to.  
**Constraint:** None.  
**What I learned:** How group membership impacts file permissions.


### `3-new_owner`
**Instruction:** Change the owner of *hello* to betty.  
**Constraint:** Requires elevated privileges.  
**What I learned:** How `chown` works and why only root can change ownership.


### `4-empty`
**Instruction:** Create an empty file named *hello*.  
**Constraint:** None.  
**What I learned:** Creating files without editors and understanding default permissions.


### `5-execute`
**Instruction:** Add execute permission to the owner of *hello*.  
**Constraint:** File must exist in the working directory.  
**What I learned:** Applying targeted permission changes with `chmod`.


### `6-multiple_permissions`
**Instruction:** Add execute permission to owner and group, and read permission to others.  
**Constraint:** None.  
**What I learned:** Combining multiple symbolic permission rules.


### `7-everybody`
**Instruction:** Add execute permission for owner, group, and others.  
**Constraint:** No commas allowed.  
**What I learned:** Modifying permissions symbolically with concise syntax.


### `8-James_Bond`
**Instruction:** Set permissions:  
- Owner: none  
- Group: none  
- Others: all permissions  
**Constraint:** No commas allowed.  
**What I learned:** How to set strict permission patterns using symbolic mode.


### `9-John_Doe`
**Instruction:** Set the file mode of *hello* to `rwxr-x-wx`.  
**Constraint:** No commas allowed.  
**What I learned:** Translating between symbolic and numeric permission formats.


### `10-mirror_permissions`
**Instruction:** Set *hello*’s permissions to match those of *olleh*.  
**Constraint:** Must work for any permission mode.  
**What I learned:** Copying permissions dynamically from one file to another.


### `11-directories_permissions`
**Instruction:** Add execute permission to **all subdirectories**, without changing files.  
**Constraint:** Only directories should be affected.  
**What I learned:** Distinguishing between file types when applying permissions in bulk.


### `12-directory_permissions`
**Instruction:** Create `my_dir` with permissions **751**.  
**Constraint:** Must be created in the working directory.  
**What I learned:** Setting permission modes directly during directory creation.


### `13-change_group`
**Instruction:** Change the group owner of *hello* to *school*.  
**Constraint:** Requires root privileges.  
**What I learned:** Manipulating the group ownership of individual files.


### `14-change_owner_and_group`
**Instruction:** Change both owner and group to *vincent* and *staff* for every file and directory.  
**Constraint:** Must run as root.  
**What I learned:** Applying ownership changes recursively to multiple items.


### `15-symbolic_link_permissions`
**Instruction:** Change the owner and group of *_hello* (a symbolic link).  
**Constraint:** Must modify the **link**, not the target.  
**What I learned:** Handling symbolic link metadata safely using proper flags.


### `16-if_only`
**Instruction:** Change the owner of *hello* to *vincent* only if its current owner is *guillaume*.  
**Constraint:** Conditional ownership change.  
**What I learned:** Implementing safe system operations based on file metadata checks.

---

## Conclusion
This project pushed me to develop a deeper and more structured understanding of Linux systems. Permissions are often seen as a small detail, but they control everything: access, security, processes, and even the behavior of software.  
I learned to reason like a system administrator: check identities, validate permissions, avoid unsafe operations, and understand why each action succeeds or fails.  
It’s a demanding module, but incredibly valuable for all future work in C programming, DevOps, security, and system-level development.  
I now feel more confident navigating Unix at a professional level and understanding the implications of every command I execute.

