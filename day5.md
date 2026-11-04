# LINUX LEARNING JOURNEY
# DAY 5 – MOVE, RENAME AND REMOVE COMMANDS

## 1. mv command

`mv` stands for Move.

It is used for:
1. Moving files and directories.
2. Renaming files and directories.

Syntax:

```bash
mv source destination
```

### Example 1: Rename a directory

```bash
mv test renamedTest
```

The directory `test` is renamed to `renamedTest`.

### Example 2: Move a directory

```bash
mv renamedTest random
```

If `random` is an existing directory, `renamedTest` moves inside it.

### Example 3: Move a directory to the current location

```bash
mv random/renamedTest .
```

`.` represents the current working directory.

## 2. rm command

`rm` stands for Remove.

It is used to delete files.

Example:

```bash
rm file.txt
```

This removes the file named `file.txt`.

## 3. Removing directories

If we try:

```bash
rm renamedTest
```

We may get this error:

```text
rm: renamedTest: is a directory
```

Reason:

By default, `rm` does not remove directories.

## 4. rm -r command

`-r` means recursive.

It removes a directory and all its contents, including files and subdirectories.

Example:

```bash
rm -r renamedTest
```

IMPORTANT:

This normally deletes permanently without moving the files to Trash. Always verify the directory name before executing.

## 5. Important path symbols

| Symbol | Meaning |
|---|---|
| `.` | Current directory |
| `..` | Parent directory |
| `~` | Home directory |
| `/` | Root directory |

Examples:

```bash
pwd
```
Displays the current working directory.

```bash
cd ..
```
Moves to the parent directory.

```bash
cd ~
```
Moves to the home directory.

## 6. Difference between cp and mv

### cp – Copy

```bash
cp file.txt backup.txt
```

Creates a copy. The original file remains.

### mv – Move

```bash
mv file.txt backup.txt
```

Moves or renames the original file. It does not leave a second copy at the old location.

## 7. Important Linux Commands – Revision

| Command | Purpose |
|---|---|
| `mv` | Move or rename files and directories |
| `rm` | Remove files |
| `rm -r` | Remove directories recursively |
| `cp` | Copy files |
| `cp -r` | Copy directories recursively |
| `mkdir` | Create directories |
| `mkdir -p` | Create nested directories |
| `touch` | Create empty files |
| `pwd` | Display current directory |
| `ls -la` | Display files, including hidden files |
| `cd` | Change directory |

## 8. Practical Exercise

Execute these commands one by one:

```bash
mkdir day5_practice
cd day5_practice

mkdir test
mv test renamedTest

mkdir random
mv renamedTest random

mv random/renamedTest .

ls -l

rm -r renamedTest

ls -l
```

## 9. Today's Learning Summary

1. Learned how to rename directories using `mv`.
2. Learned how to move directories.
3. Understood the current directory symbol `.`.
4. Learned why `rm` cannot normally remove directories.
5. Understood recursive deletion using `rm -r`.
6. Learned the difference between `cp` and `mv`.

**Learning principle:**

Don't memorize commands blindly. Understand what each command does to your files and directories before executing it.
