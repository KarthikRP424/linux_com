# DAY 4 – LINUX COMMANDS

## 1. tr command

`tr` stands for Translate.

It is used to translate or replace characters. It can convert lowercase letters into uppercase and uppercase into lowercase.

Example:

Create a file:

```bash
cat > file.txt
my name is karthik
```

Press `Ctrl + D` to save the input.

Convert lowercase to uppercase:

```bash
cat file.txt | tr 'a-z' 'A-Z' > upper.txt
```

Output:

```text
MY NAME IS KARTHIK
```

Convert uppercase to lowercase:

```bash
cat upper.txt | tr 'A-Z' 'a-z' > lower.txt
```

## 2. Pipe ( | )

A pipe connects two commands.

The output of the first command becomes the input of the second command.

Example:

```bash
cat file.txt | tr 'a-z' 'A-Z'
```

Here:
- `cat file.txt` reads the file.
- `|` passes its output to the next command.
- `tr` converts lowercase letters to uppercase.

## 3. mkdir command

`mkdir` stands for Make Directory.

It creates a new directory (folder).

Example:

```bash
mkdir new_one
```

To create nested directories:

```bash
mkdir -p new_one/file_one/file_two
```

The `-p` option creates parent directories if they do not exist.

## 4. touch command

`touch` creates an empty file if it does not exist.

Example:

```bash
touch file.txt
```

It can also update a file's timestamp if the file already exists.

## 5. cp command

`cp` stands for Copy.

It copies files or directories.

Copy a file:

```bash
cp file.txt backup.txt
```

Copy a directory:

```bash
cp -r new_one backup_one
```

## 6. mv command

`mv` stands for Move.

It moves files or directories and can also rename them.

Move a file:

```bash
mv file.txt new_one/
```

Rename a file:

```bash
mv file.txt new_file.txt
```

## 7. rm command

`rm` stands for Remove.

It deletes files.

Example:

```bash
rm file.txt
```

Remove a directory and its contents:

```bash
rm -r new_one
```

IMPORTANT: `rm` normally deletes without moving files to the Trash. Be careful before executing it.

## DAY 4 REVISION

| Command | Purpose |
|---|---|
| `tr` | Translate characters |
| `\|` | Connect commands using a pipe |
| `mkdir` | Create directories |
| `touch` | Create empty files |
| `cp` | Copy files/directories |
| `mv` | Move or rename |
| `rm` | Remove files/directories |
| `cat` | Display file contents |

**Today's key learning:** Linux commands can work together. The pipe (`|`) allows one command's output to become another command's input.
