# Minishell

**A simple Unix shell, your own basic Bash**

---


Minishell is a minimal shell program written in C that allows you to interact with your system via command lines, mimicking the behavior of popular shells like Bash.

You will deepen your understanding of process management, file descriptors, signals, and command parsing.

---

## Features (Mandatory)

- Display a prompt and read user input with history support.
- Execute commands by searching executables in `PATH`, or using relative/absolute paths.
- Implement built-in commands:
  - `echo` (with `-n` option)
  - `cd` (with relative or absolute paths)
  - `pwd`
  - `export`
  - `unset`
  - `env`
  - `exit`
- Handle input/output redirections:
  - `<` (input redirect)
  - `>` (output redirect)
  - `>>` (append output)
  - `<<` (here-document)
- Support pipes (`|`) to chain commands.
- Interpret single (`'`) and double (`"`) quotes properly.
- Expand environment variables (`$VAR`) and special variables like `$?`.
- Handle signals like Ctrl-C, Ctrl-D, Ctrl-\ like Bash:
  - Ctrl-C: cancels current input and shows prompt
  - Ctrl-D: exits the shell
  - Ctrl-\: ignored
- Use at most one global variable for signals.
- Avoid memory leaks and conform to the Norm coding standard.

---

## Bonus Features

- Logical operators `&&` and `||` with parentheses support, allowing command chaining with conditions.
- Wildcard expansion (`*`) for files in the current directory.

---

## How to Build and Run

1. Clone the repo and :

   ```bash
   cd minishell
   make
   ./minishell
