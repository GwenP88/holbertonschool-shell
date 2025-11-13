![Shell Basics Banner](/assets/Holberton.png)

# Holberton School – Shell Projects (Generic README)

## Introduction
This repository gathers all my first Shell projects at Holberton School.  
Through these modules, I moved from simply *using* a terminal to really understanding how a Unix shell works: how it navigates the filesystem, manages permissions, redirects data, initializes the environment, manipulates variables, and interprets expansions.

These projects were my entry point into a more “system-level” mindset: reading man pages, debugging commands, understanding errors instead of just re-running things blindly, and building small scripts that are actually reusable.

This README gives a global overview of the repository and the skills I built across all Shell projects.

---

## Repository Structure

- `basics/`  
  First contact with the shell in practice: navigation, listing files, creating/moving/removing files and directories, symbolic links, and first scripts.

- `permissions/`  
  Focused on Linux permissions, users and groups: `chmod`, `chown`, `chgrp`, execution bits, special modes, and how permissions apply to files, directories and symlinks.

- `io_redirections_and_filters/`  
  Work on data flow in the shell: standard input/output, redirections, pipes, text filters (`head`, `tail`, `wc`, `sort`, `uniq`, `grep`, `tr`, etc.) and log/config parsing.

- `init_files_variables_and_expansions/`  
  Shell configuration and “brain”: init files (`/etc/profile`, `~/.bashrc`), local vs global variables, environment, expansions, arithmetic, aliases and what really happens when you type a command like `ls -l *.txt`.

---

## Cross-cutting Skills and Concepts

### Unix Shell Foundations
- Understanding what the **shell** is and how it differs from the **terminal**.
- Navigating the filesystem: `pwd`, `cd`, `ls`, relative vs absolute paths.
- Creating, moving and deleting files and directories.
- Using man pages and documentation instead of relying on guesswork.

### Filesystem and Permissions
- Reading and interpreting long listings: permissions, owner, group, size, timestamps.
- Managing permissions with `chmod` (symbolic and numeric modes).
- Changing owners and groups (`chown`, `chgrp`) and understanding why only root can change ownership.
- Handling symbolic links and the difference between link and target.

### I/O Redirections and Filters
- Redirecting output to a file (`>`, `>>`) and reading input from a file (`<`).
- Building pipelines with `|` to chain tools instead of writing monolithic scripts.
- Using core text utilities:
  - `head`, `tail` for inspecting file boundaries,
  - `cat`, `wc` for concatenation and counting,
  - `sort`, `uniq` for ordering and de-duplicating,
  - `grep` for pattern matching,
  - `tr`, `rev`, `cut`, etc. for transforming and extracting text.
- Parsing real configuration and system files: `/etc/passwd`, `/etc/shadow`, `/etc/ssh/sshd_config`, log files.

### Shell Init Files, Variables and Expansions
- Global vs local initialization:
  - `/etc/profile`, `/etc/profile.d/` for system-wide configuration,
  - `~/.bashrc` for per-user interactive shell customization.
- Local vs global (environment) variables:
  - Creating, exporting, deleting variables,
  - Understanding key reserved variables: `HOME`, `PATH`, `PS1`, etc.
- Special parameters like `$?` (exit status) and their impact on scripting.
- Expansions:
  - Parameter expansion,
  - Filename expansion (`*.c`, `??.txt`, etc.),
  - Command substitution with `$(...)` and backticks,
  - Correct use of single vs double quotes and escaping.
- Shell arithmetic:
  - Basic operations and integer arithmetic,
  - Base conversions (binary ↔ decimal ↔ hex, custom alphabets),
  - Formatting numeric output (integer and floating-point style).

### Aliases and Customization
- Creating aliases for frequent or complex commands.
- Listing existing aliases and understanding how they override built-ins/binaries.
- Temporarily bypassing aliases (e.g. `\ls`).
- Developing good habits around customization without breaking standard behavior.

---

## Project Overview

### 1. `basics/` – Shell Basics
**Goal:** Learn how to move in the filesystem and automate simple tasks with scripts.  
**Focus:** `pwd`, `ls`, `cd`, `mkdir`, `rm`, `mv`, `cp`, hidden files, long format, symbolic links, and simple directory trees.  
**What I took away:** A solid, practical foundation for working in a Unix environment and writing small scripts that reproduce manual command sequences.

---

### 2. `permissions/` – Shell Permissions
**Goal:** Understand and control who can read, write, or execute what on the system.  
**Focus:** `chmod`, `chown`, `chgrp`, owner/group/others, execute bits on files and directories, permissions on symlinks, and conditional changes.  
**What I took away:** A clear mental model of Linux permissions and the ability to diagnose “Permission denied” issues instead of fumbling around.

---

### 3. `io_redirections_and_filters/` – Shell I/O Redirections and Filters
**Goal:** Learn how to manipulate data streams directly from the command line.  
**Focus:** Redirections, pipes, text filters, log parsing, configuration inspection, and combining simple tools to build powerful pipelines.  
**What I took away:** The habit of thinking in terms of “streams” and “filters” rather than trying to find one big complex command for everything.

---

### 4. `init_files_variables_and_expansions/` – Init Files, Variables and Expansions
**Goal:** Understand how the shell starts, how it stores information, and how it interprets commands before running them.  
**Focus:** Init files, local and environment variables, expansions, arithmetic, aliases, and explanation of what happens when you type a command like `ls *.c`.  
**What I took away:** A much deeper understanding of the shell’s internal logic, and the ability to control my environment instead of just adapting to defaults.

---

## Conclusion
Across these Shell projects, I went from basic usage of the terminal to a much more professional and structured understanding of the Unix shell:

- I can navigate and manipulate the filesystem confidently.
- I know how permissions really work and how to fix them safely.
- I can build pipelines to analyze and transform data directly in the terminal.
- I understand how the shell initializes, expands, and evaluates what I type.
- I can customize my environment with variables and aliases in a controlled way.

These foundations are critical for the next steps of the Holberton curriculum: low-level C programming, DevOps, debugging, and any serious work on Linux systems. This repository is the trace of that learning curve and a toolbox I will keep using and extending.


