![Shell Basics Banner](/assets/Holberton.png)

# Shell I/O Redirections and Filters – Holberton School Project

## Introduction
This project was my first deep dive into what really happens when data flows through the shell: text going from commands to files, from files back into commands, and from one command to another through pipes and filters.  
After learning the basics of navigation and permissions, I needed to understand how to *shape* data on the command line: select, filter, sort, extract, transform, and redirect it.  
Working on this module forced me to pay attention to details like quotes, special characters, and the difference between standard input, standard output, and standard error. It also made me much more comfortable chaining commands together instead of relying on a single “magic” tool.  
This README summarizes the concepts I learned and what each exercise taught me in practice.

---

## Concepts Learned

### Shell / I/O Redirection and Filters
- Redirecting **standard output** to a file (`>` and `>>`).
- Reading **standard input** from a file (`<`).
- Using **pipes** to send the output of one command to the input of another (`|`).
- Combining multiple commands and filters:
  - `head`, `tail`
  - `cat`, `wc`
  - `sort`, `uniq`
  - `grep`
  - `tr`
  - `find`
- Overwriting vs appending to files safely.

### Special Characters and Quoting
- Meaning and usage of:
  - Whitespace and word splitting
  - Single quotes vs double quotes
  - Backslash escaping
  - Comments with `#`
  - Pipes `|`
  - Command separators `;`
  - Tilde `~` expansion
- How to correctly escape complex strings and filenames containing special characters.

### System Files and Other Man Pages
- Displaying text (`echo`, etc.).
- Concatenating files and printing to standard output.
- Reversing strings and transforming characters.
- Cutting parts of lines (fields and columns).
- Understanding:
  - `/etc/passwd` format (user accounts)
  - `/etc/shadow` format (password hashes)
  - `/etc/ssh/sshd_config` role and structure.
- Basic log parsing and text processing patterns for real-world data (web server logs, word lists, etc.).

---

## Tasks

### `0-hello_world`
**Instruction:** Print “Hello, World” followed by a newline to standard output.  
**Constraints:** Output must go to standard output only.  
**What I learned:** The simplest form of output redirection and how to reliably print text from a script.


### `1-confused_smiley`
**Instruction:** Display the confused smiley `"(Ôo)'`.  
**Constraints:** Proper quoting/escaping of special characters.  
**What I learned:** How to use quotes and escapes so the shell prints a complex string exactly as intended.


### `2-hellofile`
**Instruction:** Display the content of `/etc/passwd`.  
**Constraints:** File must be read-only; no modifications.  
**What I learned:** How to safely inspect system files using basic commands and redirections.


### `3-twofiles`
**Instruction:** Display the content of `/etc/passwd` **and** `/etc/hosts`.  
**Constraints:** Both files must be printed in sequence.  
**What I learned:** Concatenating multiple files and understanding the difference between single and multiple arguments.


### `4-lastlines`
**Instruction:** Display the last 10 lines of `/etc/passwd`.  
**Constraints:** Use the appropriate tool for “tail” behavior.  
**What I learned:** How to quickly focus on the end of a file, which is very common in log analysis.


### `5-firstlines`
**Instruction:** Display the first 10 lines of `/etc/passwd`.  
**Constraints:** None beyond using the right filter.  
**What I learned:** How to inspect file headers or the beginning of configuration files.


### `6-third_line`
**Instruction:** Display the **third line** of the file `iacta`.  
**Constraints:** **Not allowed to use `sed`**. File will be in the working directory.  
**What I learned:** How to combine existing tools to extract a specific line without relying on one single “obvious” command.


### `7-file`
**Instruction:** Create a file named exactly  
`\*\\'"Best School"\'\\*$\?\*\*\*\*\*:)`  
containing the text `Best School` followed by a newline.  
**Constraints:** Filename must match exactly; requires careful quoting/escaping.  
**What I learned:** Dealing with extremely complex filenames and mastering quotes and backslashes.


### `8-cwd_state`
**Instruction:** Write the output of `ls -la` into `ls_cwd_content`.  
If the file exists, overwrite it; if not, create it.  
**Constraints:** Output must replace previous content.  
**What I learned:** Using redirection to capture command output into a file safely.


### `9-duplicate_last_line`
**Instruction:** Duplicate the last line of `iacta`.  
**Constraints:** `iacta` is in the working directory and must be modified in place.  
**What I learned:** How to append specific parts of a file back into the same file using pipes and redirections.


### `10-no_more_js`
**Instruction:** Delete all regular `.js` files in the current directory and all subdirectories.  
**Constraints:** Only regular files; directories must be preserved.  
**What I learned:** Combining `find` with filters and actions to clean a tree of files by extension.


### `11-directories`
**Instruction:** Count the number of directories and subdirectories in the current directory.  
**Constraints:**  
- Do **not** count `.` and `..`  
- Hidden directories **must** be counted  
**What I learned:** Using `find` and filters to count directories, and understanding how special entries are treated.


### `12-newest_files`
**Instruction:** Display the 10 newest files in the current directory.  
**Constraints:**  
- One filename per line  
- Sorted from newest to oldest  
**What I learned:** Combining `ls`, sorting, and limiting results to focus on recent changes.


### `13-unique`
**Instruction:** Take a list of words on standard input and print only the words that appear **exactly once**.  
**Constraints:**  
- Input: one word per line  
- Output: one word per line  
- Output must be sorted  
**What I learned:** Using `sort` and `uniq` together to detect truly unique entries.


### `14-findthatword`
**Instruction:** Display lines containing the pattern `root` from `/etc/passwd`.  
**Constraints:** None beyond using pattern matching.  
**What I learned:** Basic text searching with `grep` and how to target specific patterns in system files.


### `15-countthatword`
**Instruction:** Display the **number of lines** in `/etc/passwd` that contain the pattern `bin`.  
**Constraints:** Output must be a count only.  
**What I learned:** Combining pattern matching with line counting to get quantitative information.


### `16-whatsnext`
**Instruction:** Display lines containing `root` **and the 3 lines that follow each match** in `/etc/passwd`.  
**Constraints:** None beyond using the right options.  
**What I learned:** How to inspect context around matches to better understand where and how a pattern appears.


### `17-hidethisword`
**Instruction:** Display all lines in `/etc/passwd` that **do not** contain the pattern `bin`.  
**Constraints:** Must exclude the pattern completely.  
**What I learned:** Inverting matches with `grep` and filtering out unwanted lines.


### `18-letteronly`
**Instruction:** Display all lines of `/etc/ssh/sshd_config` that start with a letter (uppercase or lowercase).  
**Constraints:** Lines starting with comments or whitespace should be ignored.  
**What I learned:** Using regular expressions to filter lines based on their first character.


### `19-AZ`
**Instruction:** Replace all `A` with `Z` and all `c` with `e` in input.  
**Constraints:** Character-by-character transformation only.  
**What I learned:** Using `tr` to map characters and perform basic text transformations.


### `20-hiago`
**Instruction:** Remove all `c` and `C` characters from input.  
**Constraints:** Only characters, not words, must be removed.  
**What I learned:** Using `tr -d` to delete characters from a stream.


### `21-reverse`
**Instruction:** Reverse its input.  
**Constraints:** Entire input must be reversed.  
**What I learned:** How to reverse strings/lines using `rev` (or equivalent tools) and how streams are handled.


### `22-users_and_homes`
**Instruction:** Display all users and their home directories, sorted by user.  
**Constraints:**  
- Based on `/etc/passwd`  
- Output format: `user:home`  
**What I learned:** Extracting specific fields from structured system files and sorting the results.


### `23-empty_casks` (advanced)
**Instruction:** Find all empty files and directories in the current directory and all subdirectories.  
**Constraints:**  
- Only names, no full paths  
- One name per line  
- Hidden files must be listed  
- No `basename`, `grep`, `egrep`, `fgrep`, or `rgrep`  
**What I learned:** Using `find` with tests for emptiness and formatting output without extra helper commands.


### `24-gifs` (advanced)
**Instruction:** List all `.gif` files in the current directory and subdirectories.  
**Constraints:**  
- Hidden files must be listed  
- Only regular files  
- Print names **without** the `.gif` extension  
- Sort by byte value, case-insensitive  
- One file name per line, ending with a newline  
- No `basename`, `grep`, `egrep`, `fgrep`, or `rgrep`  
**What I learned:** Building a more complex pipeline combining `find`, sorting, transformations, and output formatting.


### `25-acrostic` (advanced)
**Instruction:** Decode acrostics by using the **first letter of each line** from standard input.  
**Constraints:**  
- Result must end with a newline  
- No `grep`, `egrep`, `fgrep`, or `rgrep`  
**What I learned:** Using text tools to pick specific characters across many lines and building a hidden message.


### `26-the_biggest_fan` (advanced)
**Instruction:** Parse web server logs (TSV) and display the **11 most active hosts/IPs**.  
**Constraints:**  
- Ordered by number of requests, highest first  
- No `grep`, `egrep`, `fgrep`, or `rgrep`  
**What I learned:** How to parse structured log files with shell tools, aggregate counts, sort them, and extract top results—exactly the kind of workflow used in basic log analysis.

---

## Conclusion
This project taught me that the shell is more than just a command interpreter; it's a powerful data processing environment. By combining redirections, pipes, and small, specialized utilities, I can transform and analyze text files, logs, and configuration files very efficiently. I also learned to pay much closer attention to quotation marks, special characters, and how the shell interprets spaces and symbols. This attention to detail is essential for avoiding subtle bugs and dangerous errors. In short, the "Shell Redirections and Input/Output Filters" project provided me with a practical toolkit for working with real data directly from the command line.

