# LINUX LEARNING JOURNEY
# DAY 6 – SUDO COMMAND

## 1. What is sudo?

sudo stands for Superuser Do.

It allows an authorized user to execute commands with elevated privileges, usually as the root user.

Root user has almost complete control over the Linux operating system.

Example:

```bash
sudo apt update
```

## 2. Why do we use sudo?

We use sudo when we need permission to perform administrative tasks.

Examples:
1. Installing software.
2. Updating the operating system.
3. Managing system services.
4. Creating files or directories in protected system locations.
5. Changing system configurations.

## 3. Basic syntax

```bash
sudo command
```

Example:

```bash
sudo apt update
```

Here:
- sudo: Requests elevated privileges.
- apt: Ubuntu package management tool.
- update: Refreshes package information.

## 4. Practical sudo commands

### Example 1: Update package information

```bash
sudo apt update
```

It refreshes the list of available software packages.

### Example 2: Upgrade installed packages

```bash
sudo apt upgrade
```

It upgrades installed packages when updates are available.

### Example 3: Install Git

```bash
sudo apt install git
```

It installs Git on Ubuntu.

### Example 4: Create a directory in a protected location

```bash
sudo mkdir /opt/myproject
```

It creates a directory named myproject inside /opt.

## 5. Why does sudo ask for a password?

When we execute a sudo command, Ubuntu may ask for our account password.

Example:

```text
[sudo] password for karthik:
```

Enter your Ubuntu account password and press Enter.

IMPORTANT:
While typing the password, nothing appears on the terminal. No stars or dots are displayed. This is normal.

## 6. Normal user vs sudo

Normal command:

```bash
mkdir myfolder
```

Command with elevated privileges:

```bash
sudo mkdir /opt/myfolder
```

Difference:

- Normal commands use the permissions of the current user.
- sudo allows an authorized user to execute a command with elevated privileges.

## 7. Useful commands for practice

### Check current username

```bash
whoami
```

### Validate sudo credentials

```bash
sudo -v
```

### Update package information

```bash
sudo apt update
```

### Check Git version

```bash
git --version
```

## 8. Important safety rules

1. Do not use sudo for every command.
2. Understand a command before executing it with sudo.
3. Never share your password.
4. Avoid executing unknown scripts with sudo.
5. Be careful with commands such as:

```bash
sudo rm -rf
```

This command can recursively delete files and directories with elevated privileges.

## 9. Today's Learning Summary

1. Learned the meaning of sudo.
2. Understood root user and elevated privileges.
3. Learned why Ubuntu asks for a password.
4. Practised sudo apt update.
5. Practised sudo apt install git.
6. Understood the difference between normal commands and sudo commands.

## 10. Knowledge Check

Question 1: What does sudo stand for?

Answer: Superuser Do.

Question 2: Why do we use sudo?

Answer: To execute authorized commands with elevated privileges.

Question 3: Why does Linux ask for a password?

Answer: To authenticate the user before allowing administrative operations.

Question 4: Should we use sudo for every command?

Answer: No. We should use it only when elevated privileges are required.

LEARNING PRINCIPLE:

Linux permissions protect the operating system. Always understand the command before executing it with administrative privileges.
