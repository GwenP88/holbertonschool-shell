![Shell Basics Banner](/assets/Holberton.png)

# Shell Init Files, Variables and Expansions – Holberton School Project

## Introduction
In this project, I moved from simply “using” the shell to actually understanding how it starts, how it remembers things, and how it interprets what I type.  
Instead of just running commands, I worked with initialization files, environment and local variables, expansions, arithmetic, and aliases. That’s where the shell starts to feel programmable instead of just interactive.  
This project forced me to read man pages carefully, reason about the difference between what is local to a shell session and what is inherited by child processes, and understand how a simple line like `ls -l *.txt` is parsed and expanded before it is executed.  
This README summarizes the main concepts I learned and how each task contributed to that learning.

---

## Concepts Learned

### Shell Initialization Files
- Role of `/etc/profile` and `/etc/profile.d/` for system-wide initialization.
- Role of `~/.bashrc` for user-specific interactive shell configuration.
- When each file is read (login vs non-login, interactive vs non-interactive).

### Variables and Parameters
- Difference between **local** (shell-only) variables and **global** (environment) variables.
- What **reserved variables** are and how they affect shell behavior.
- Creation, update and deletion of variables with simple assignments and `unset`.
- Roles of `HOME`, `PATH`, `PS1` in everyday shell usage.
- Meaning of **special parameters** (e.g. `$?`, `$#`, `$0`, `$1`, etc.).
- Use of `$?` to read the exit status of the last command.

### Expansions and Substitution
- What “expansion” means: how the shell transforms a command line before execution.
- Differences between **single quotes** and **double quotes** and when to use each.
- Command substitution with `$(...)` and backticks `` `...` ``.

### Shell Arithmetic
- Using shell arithmetic expansion to perform integer operations.
- Converting numbers between bases (binary, decimal, hexadecimal, and custom encodings).
- Formatting numeric output, including floating point formatting.

### Aliases
- Creating aliases to customize commands.
- Listing existing aliases.
- Temporarily bypassing an alias (e.g. using backslash before the command).

---

## Tasks

### `0-alias`
**Instruction:** Create an alias named `ls` with value `rm -f *`.  
**Constraints:** Alias must override `ls` until explicitly bypassed.  
**What I learned:** How aliases can completely change the behavior of common commands and how to bypass them with `\command`.

---

### `1-hello_you`
**Instruction:** Print `hello user` where `user` is the current Linux username.  
**Constraints:** The message must adapt to the current user.  
**What I learned:** How to use variable expansion to access the current user and build dynamic output.

---

### `2-path`
**Instruction:** Add `/action` to the `PATH` as the **last** directory.  
**Constraints:** Append to the existing `PATH`, do not overwrite it.  
**What I learned:** Modifying `PATH` safely so that new locations are searched after the standard directories.

---

### `3-paths`
**Instruction:** Count the number of directories in `PATH`.  
**Constraints:** Must handle empty entries correctly.  
**What I learned:** How to work with colon-separated lists and use shell tools to count items.

---

### `4-global_variables`
**Instruction:** List all **environment** variables.  
**Constraints:** Use the appropriate command(s) to display global variables.  
**What I learned:** The difference between environment variables and other shell variables, and how to inspect what the shell exports to child processes.

---

### `5-local_variables`
**Instruction:** List all **local variables**, environment variables, and functions.  
**Constraints:** Must show more than just the exported environment.  
**What I learned:** How to see the complete state of the shell: variables, environment, and defined functions.

---

### `6-create_local_variable`
**Instruction:** Create a new **local** variable `BEST` with value `School`.  
**Constraints:** Variable should remain local to the current shell.  
**What I learned:** Defining variables that are not exported and thus not visible to child processes.

---

### `7-create_global_variable`
**Instruction:** Create a new **global** variable `BEST` with value `School`.  
**Constraints:** Must be exported so that child processes see it.  
**What I learned:** How to promote a variable from local to environment and why that matters for scripts and subprocesses.

---

### `8-true_knowledge`
**Instruction:** Print the result of `128 + TRUEKNOWLEDGE` followed by a newline.  
**Constraints:** `TRUEKNOWLEDGE` is provided as an environment variable.  
**What I learned:** Using shell arithmetic expansion with environment variables.

---

### `9-divide_and_rule`
**Instruction:** Print `POWER / DIVIDE` followed by a newline.  
**Constraints:** `POWER` and `DIVIDE` are environment variables.  
**What I learned:** Performing integer division in the shell and handling values coming from the environment.

---

### `10-love_exponent_breath`
**Instruction:** Print the result of `BREATH` to the power `LOVE`.  
**Constraints:** Both are environment variables; result must end with a newline.  
**What I learned:** Using shell arithmetic for exponentiation and chaining environment variables inside arithmetic expressions.

---

### `11-binary_to_decimal`
**Instruction:** Convert a binary number (stored in `BINARY`) to decimal.  
**Constraints:** Input in base 2; output in base 10.  
**What I learned:** Leveraging shell arithmetic with base prefixes to convert between number systems.

---

### `12-combinations`
**Instruction:** Print all two-letter combinations from `aa` to `zz`, except `oo`.  
**Constraints:**  
- Lowercase letters only  
- One combination per line  
- Alphabetical order  
- File size limited to 64 characters  
**What I learned:** Using expansions and loops/brace expansion to generate combinations efficiently under strict size constraints.

---

### `13-print_float`
**Instruction:** Print the value of `NUM` with two decimal places.  
**Constraints:** `NUM` may already contain decimals; output must be rounded/trimmed to 2 decimals.  
**What I learned:** Formatting numeric output to a fixed number of decimal places from within the shell.

---

### `14-decimal_to_hexadecimal`
**Instruction:** Convert a decimal number (stored in `DECIMAL`) to hexadecimal (base 16).  
**Constraints:** Output must be the base-16 representation followed by a newline.  
**What I learned:** Converting from base 10 to base 16 using shell arithmetic and understanding how different bases are represented.

---

### `15-what_happens_when_you_type_ls_*.c` (blog post – advanced)
**Instruction:** Write a blog post explaining, step by step, what happens when you type `ls *.c` and press Enter.  
**Constraints:**  
- Written in English  
- At least one picture at the top  
- Published on Medium or LinkedIn  
- Shared on LinkedIn  
**URL:**  
`https://medium.com/@gpichot_63497/what-happens-when-you-type-ls-c-in-the-shell-b4003714ab70`  
**What I learned:** How to decompose a simple shell command into parsing, expansion, path lookup, process creation, and execution—and how to explain these internal steps clearly to others.

---

### `15-rot13` (listed as task 16)
**Instruction:** Encode and decode text using **rot13**.  
**Constraints:** Assume ASCII text from standard input.  
**What I learned:** Using character mappings and shell tools to build a simple substitution cipher.

---

### `16-odd`
**Instruction:** Print every other line from standard input, starting with the first line.  
**Constraints:** The script must act as a filter in a pipeline.  
**What I learned:** Combining text-processing tools and line numbering/selection to sample input lines.

---

### `17-water_and_stir`
**Instruction:** Add the two numbers stored in `WATER` and `STIR`, where each number is expressed in a custom base (`water` and `stir`), and print the result in base `bestchol`.  
**Constraints:**  
- `WATER` and `STIR` use custom digit alphabets  
- Result must be encoded in another custom alphabet  
**What I learned:** Thinking about numbers abstractly as strings in arbitrary bases and using the shell and its tools to translate between these encodings.

---

## Conclusion
This project gave me a much deeper understanding of how the shell actually works under the surface. I learned how initialization files configure my environment, how variables move (or don’t move) from one process to another, and how expansions and arithmetic are evaluated before a command is even executed.  
I also realized how powerful small features like aliases, command substitution, and arithmetic expansion become when they are combined. They allow me to customize my shell, automate common tasks, and reason precisely about what happens when I type a command like `ls -l *.txt`.  
Overall, this project helped me move from “typing commands” to actually **controlling** the shell environment, which is essential for the rest of the Holberton curriculum and for real-world development and DevOps work.


