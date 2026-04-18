![holbertonschool-shell Banner](assets/banner.jpeg)

# io_redirections_and_filters

> Because sometimes, the terminal needs a good plumber — and that plumber is me.

---

## 📝 Description

This project is part of my shell scripting journey at Holberton School. It focuses on one of the most powerful features of Unix/Linux: I/O redirections and filters. Through a series of shell scripts, I explore how to manipulate data streams, redirect inputs and outputs, chain commands together using pipes, and filter text with precision. Each script is exactly two lines long, which sounds like a constraint but is really just the universe's way of teaching me to be elegant.

---

## 🎯 Learning Objectives

At the end of this project, I am able to explain what the commands `head`, `tail`, `find`, `wc`, `sort`, `uniq`, `grep`, and `tr` do and how to use them effectively. I understand how to redirect standard output to a file, and how to feed standard input from a file instead of the keyboard. I know how to send the output of one program directly into the input of another using pipes, and how to combine multiple commands and filters with redirections to build powerful one-liners. I can also identify and correctly use special characters such as white spaces, single quotes, double quotes, backslash, comment signs, pipes, command separators, and the tilde. I know how to display a line of text with `echo`, concatenate files with `cat`, reverse a string with `rev`, and remove sections from lines with `cut`. Finally, I understand the structure and purpose of the `/etc/passwd` and `/etc/shadow` files.

---

## 🛠️ Technologies Used

All scripts in this project are written in **Bash** and executed on **Ubuntu 20.04 LTS**. The tools leveraged throughout include core Unix text-processing utilities such as `echo`, `cat`, `head`, `tail`, `find`, `wc`, `sort`, `uniq`, `grep`, `tr`, `rev`, `cut`, and `passwd (5)`. No external dependencies are required — just a terminal and a healthy respect for the pipe character.

---

## ⚙️ Requirements

- **OS:** Ubuntu 20.04 LTS
- **Allowed editors:** `vi`, `vim`, `emacs`
- All scripts must be exactly **two lines long** (`wc -l file` must print `2`)
- All files must end with a **new line**
- The first line of every script must be exactly `#!/bin/bash`
- All files must be **executable**
- The use of backticks, `&&`, `||`, and `;` is **not allowed**
- The use of `sed` and `awk` is **not allowed**
- A `README.md` at the root of the project folder is mandatory

---

## 🚀 Installation

```bash
git clone https://github.com/GwenP88/holbertonschool-shell.git
cd holbertonschool-shell/io_redirections_and_filters
```

---

## ▶️ Usage / Execution

Make a script executable and run it directly:

```bash
chmod +x filename
./filename
```

---

## 📊 Project Progress

<p align="center">
<img src="assets/progress_barre_100.gif" alt="Mandatory tasks progress" width="80%">
</p>

<p align="center">
<sub>Mandatory tasks completion: 100% --- Advanced tasks completion: 100%</sub>
</p>

---

## ✨ Features

### Task 0 - Hello World

- Mandatory
- Print "Hello, World" followed by a new line to standard output
- Must use `echo`
- Outputs `Hello, World` to stdout, ending with a newline

**Files:** `0-hello_world`

---

### Task 1 - Confused smiley

- Mandatory
- Display a confused smiley `"(Ôo)'`
- Must correctly handle special characters (double quotes, single quote)
- Outputs `"(Ôo)'` to stdout

**Files:** `1-confused_smiley`

---

### Task 2 - Let's display a file

- Mandatory
- Display the full content of `/etc/passwd`
- Must use `cat`
- Prints every line of `/etc/passwd` to stdout

**Files:** `2-hellofile`

---

### Task 3 - What about 2?

- Mandatory
- Display the content of both `/etc/passwd` and `/etc/hosts`
- Must concatenate two files in a single command
- Prints both files sequentially to stdout

**Files:** `3-twofiles`

---

### Task 4 - Last lines of a file

- Mandatory
- Display the last 10 lines of `/etc/passwd`
- Must use `tail`
- Outputs only the last 10 lines of the file

**Files:** `4-lastlines`

---

### Task 5 - I'd prefer the first ones actually

- Mandatory
- Display the first 10 lines of `/etc/passwd`
- Must use `head`
- Outputs only the first 10 lines of the file

**Files:** `5-firstlines`

---

### Task 6 - Line #2

- Mandatory
- Display the third line of the file `iacta` (located in the working directory)
- `sed` is not allowed
- Outputs exactly the third line of `iacta`

**Files:** `6-third_line`

---

### Task 7 - It is a good file that cuts iron without making a noise

- Mandatory
- Create a file with a very special name: `\*\\'"Best School"\'\\*$\?\*\*\*\*\*:)` containing the text `Best School` ending with a newline
- Must correctly handle all special characters in the filename
- Creates the file with the exact name and content specified

**Files:** `7-file`

---

### Task 8 - Save current state of directory

- Mandatory
- Write the result of `ls -la` into a file named `ls_cwd_content`, overwriting it if it already exists
- Must use output redirection (`>`)
- Creates or overwrites `ls_cwd_content` with the current directory listing

**Files:** `8-cwd_state`

---

### Task 9 - Duplicate last line

- Mandatory
- Append the last line of the file `iacta` to itself
- The file `iacta` will be in the working directory
- The last line of `iacta` appears twice at the end of the file after execution

**Files:** `9-duplicate_last_line`

---

### Task 10 - No more javascript

- Mandatory
- Delete all regular files with a `.js` extension in the current directory and all sub-directories
- Must use `find`; directories with `.js` in their name must not be deleted
- All `.js` regular files are removed recursively; `.js` directories are left untouched

**Files:** `10-no_more_js`

---

### Task 11 - Don't just count your directories, make your directories count

- Mandatory
- Count the number of directories and sub-directories in the current directory (excluding `.` and `..`; hidden directories must be counted)
- Must use `find` and `wc`
- Outputs a single integer representing the total number of directories

**Files:** `11-directories`

---

### Task 12 - What's new

- Mandatory
- Display the 10 newest files in the current directory, sorted from newest to oldest, one file per line
- Must use `ls` with appropriate options
- Outputs 10 filenames sorted by modification time, most recent first

**Files:** `12-newest_files`

---

### Task 13 - Being unique is better than being perfect

- Mandatory
- Take a list of words as input (one per line) and print only the words that appear exactly once, sorted
- Must use `sort` and `uniq`
- Outputs only unique words in alphabetical order

**Files:** `13-unique`

---

### Task 14 - It must be in that file

- Mandatory
- Display lines containing the pattern "root" from `/etc/passwd`
- Must use `grep`
- Outputs all matching lines from `/etc/passwd`

**Files:** `14-findthatword`

---

### Task 15 - Count that word

- Mandatory
- Display the number of lines containing the pattern "bin" in `/etc/passwd`
- Must use `grep` with the count option
- Outputs a single integer

**Files:** `15-countthatword`

---

### Task 16 - What's next?

- Mandatory
- Display lines containing the pattern "root" and the 3 lines that follow each match in `/etc/passwd`
- Must use `grep` with the after-context option
- Outputs matching lines plus 3 lines of context after each match

**Files:** `16-whatsnext`

---

### Task 17 - I hate bins

- Mandatory
- Display all lines in `/etc/passwd` that do not contain the pattern "bin"
- Must use `grep` with invert-match
- Outputs all non-matching lines

**Files:** `17-hidethisword`

---

### Task 18 - Letters only please

- Mandatory
- Display all lines from `/etc/ssh/sshd_config` that start with a letter (including capital letters)
- Must use `grep` with a regular expression
- Outputs only lines beginning with an alphabetic character

**Files:** `18-letteronly`

---

### Task 19 - A to Z

- Mandatory
- Replace all `A` characters with `Z` and all `c` characters with `e` from input
- Must use `tr`
- Transforms input according to the character mapping and outputs the result

**Files:** `19-AZ`

---

### Task 20 - Without C, you would live in hiago

- Mandatory
- Remove all `c` and `C` characters from input
- Must use `tr` with the delete option
- Outputs the input with all occurrences of `c` and `C` removed

**Files:** `20-hiago`

---

### Task 21 - esreveR

- Mandatory
- Reverse its input
- Must use `rev`
- Outputs the input with characters reversed

**Files:** `21-reverse`

---

### Task 22 - DJ Cut Killer

- Mandatory
- Display all users and their home directories from `/etc/passwd`, sorted by username
- Must use `cut` and `sort`
- Outputs `username:home_directory` pairs sorted alphabetically

**Files:** `22-users_and_homes`

---

### Task 23 - Empty casks make the most noise

- Advanced
- Find all empty files and directories in the current directory and all sub-directories; display only names (not full paths), including hidden files, one per line
- `basename`, `grep`, `egrep`, `fgrep`, and `rgrep` are not allowed
- Outputs names of all empty files and directories, one per line, ending with a newline

**Files:** `23-empty_casks`

---

### Task 24 - A gif is worth ten thousand words

- Advanced
- List all `.gif` files (including hidden ones) in the current directory and sub-directories; display names without extensions, sorted case-insensitively by byte value, one per line
- `basename`, `grep`, `egrep`, `fgrep`, and `rgrep` are not allowed; only regular files, not directories
- Outputs filenames without `.gif` extension, sorted case-insensitively

**Files:** `24-gifs`

---

### Task 25 - Acrostic

- Advanced
- Decode acrostics by extracting and displaying the first letter of each line from input; output ends with a newline
- `grep`, `egrep`, `fgrep`, and `rgrep` are not allowed
- Outputs the decoded word formed by the first letter of each input line

**Files:** `25-acrostic`

---

### Task 26 - The biggest fan

- Advanced
- Parse web server logs in TSV format from stdin and display the 11 hosts or IP addresses with the most requests, ordered from most to least active
- `grep`, `egrep`, `fgrep`, and `rgrep` are not allowed
- Outputs the top 11 most active hosts/IPs, one per line, sorted by request count descending

**Files:** `26-the_biggest_fan`

---

## 🤝 Contributions & Acknowledgements

A big thank you to the Holberton School staff and peers for the guidance, the well-crafted tasks, and the occasional existential crisis caused by a misplaced pipe. Special appreciation to the creators of `man` pages — unsung heroes of the terminal world.

---

## 👤 Author

**Gwenaelle PICHOT**
- Student at Holberton School
- Track: `holbertonschool-shell`
- Project: `io_redirections_and_filters`