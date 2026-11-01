# 🐧 LINUX LEARNING JOURNEY
## DAY 2 – Linux Commands & Shell Basics

### 1. PATH – Environment Variable

Command:
```bash
echo $PATH
```
- PATH is an environment variable.
- It contains a list of directories.
- When we execute a command, the shell searches these directories to locate its executable program.
- Directories are separated by `:`.

Example:
```bash
/usr/local/bin:/usr/bin:/bin
```

### 2. which – Find Command Location

Command:
```bash
which python3
```
- Displays the location of an executable command.
- Helps us understand where a program is installed.

### 3. cat – Display File Contents

Command:
```bash
cat notes.txt
```
- Displays the contents of a file.
- Can also combine multiple files.

Create a file with content:
```bash
cat > notes.txt
```
Type the content and press `Ctrl + D` to finish.

### 4. .zprofile – Zsh Configuration File

- `.zprofile` is a configuration file for the Zsh shell.
- It executes commands when a Zsh login session starts.
- It can be used to configure environment variables and PATH.

Example:
```bash
echo "Welcome to Linux!"
```

Note:
- `.bashrc` – Bash interactive shell configuration.
- `.zshrc` – Zsh interactive shell configuration.
- `.zprofile` – Zsh login shell configuration.

### 5. pwd – Present Working Directory

Command:
```bash
pwd
```
Displays the current directory location.

### 6. cd – Change Directory

Command:
```bash
cd Documents
```
Moves into the Documents directory.

Other useful commands:
```bash
cd ..     # Go one directory level up
cd ~      # Go to home directory
cd /      # Go to root directory
```

### 7. Important Practical Commands

```bash
echo $PATH
which python3
cat /etc/os-release
pwd
ls -la
```

### DAY 2 – KEY LEARNINGS

1. PATH helps the shell locate executable programs.
2. cat displays file contents.
3. which identifies executable locations.
4. .zprofile configures Zsh login sessions.
5. pwd shows the current location.
6. cd changes the current directory.

### DAY 2 – PRACTICE GOAL

Understand how Linux searches for commands, reads files, and manages shell configuration.

**Learning principle:** Don't memorize commands. Understand what happens behind every command.
