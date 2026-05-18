# Basic Linux Commands From learning seesion 3

This README introduces common Linux commands used for navigating the terminal,
working with files and directories, viewing system information, and managing
processes.

## Navigation

| Command | Description | Example |
| --- | --- | --- |
| `pwd` | Shows the current working directory. | `pwd` |
| `ls` | Lists files and directories. | `ls` |
| `ls -la` | Lists all files, including hidden files, with details. | `ls -la` |
| `cd` | Changes to another directory. | `cd Documents` |
| `cd ..` | Moves up one directory level. | `cd ..` |
| `clear` | Clears the terminal screen. | `clear` |

## Files and Directories

| Command | Description | Example |
| --- | --- | --- |
| `touch` | Creates an empty file or updates a file timestamp. | `touch notes.txt` |
| `mkdir` | Creates a new directory. | `mkdir projects` |
| `cp` | Copies files or directories. | `cp file.txt backup.txt` |
| `mv` | Moves or renames files and directories. | `mv old.txt new.txt` |
| `rm` | Deletes a file. | `rm file.txt` |
| `rm -r` | Deletes a directory and its contents. | `rm -r old-folder` |
| `rmdir` | Deletes an empty directory. | `rmdir empty-folder` |

## Viewing and Editing Files

| Command | Description | Example |
| --- | --- | --- |
| `cat` | Displays the full contents of a file. | `cat README.md` |
| `less` | Opens a file for scrolling and reading. | `less README.md` |
| `head` | Shows the first lines of a file. | `head file.txt` |
| `tail` | Shows the last lines of a file. | `tail file.txt` |
| `nano` | Opens a simple terminal text editor. | `nano notes.txt` |
| `vim` | Opens the Vim text editor. | `vim notes.txt` |

## Searching

| Command | Description | Example |
| --- | --- | --- |
| `find` | Searches for files and directories. | `find . -name "*.txt"` |
| `grep` | Searches text inside files. | `grep "error" log.txt` |
| `grep -r` | Searches text recursively in directories. | `grep -r "main" .` |
| `which` | Shows the location of an installed command. | `which python` |

## Permissions

| Command | Description | Example |
| --- | --- | --- |
| `chmod` | Changes file permissions. | `chmod +x script.sh` |
| `chown` | Changes file ownership. | `sudo chown user:user file.txt` |
| `sudo` | Runs a command with administrator privileges. | `sudo apt update` |

## System Information

| Command | Description | Example |
| --- | --- | --- |
| `whoami` | Shows the current logged-in user. | `whoami` |
| `uname -a` | Shows system and kernel information. | `uname -a` |
| `df -h` | Shows disk space usage in a readable format. | `df -h` |
| `du -sh` | Shows the size of a file or directory. | `du -sh Downloads` |
| `free -h` | Shows memory usage. | `free -h` |
| `date` | Shows the current date and time. | `date` |

## Processes

| Command | Description | Example |
| --- | --- | --- |
| `ps` | Shows running processes for the current shell. | `ps` |
| `top` | Displays live system process information. | `top` |
| `kill` | Stops a process by process ID. | `kill 1234` |
| `killall` | Stops processes by command name. | `killall firefox` |

## Package Management

Package commands depend on the Linux distribution.

| Distribution | Command | Example |
| --- | --- | --- |
| Debian/Ubuntu | `apt` | `sudo apt update` |
| Fedora | `dnf` | `sudo dnf install git` |
| Arch Linux | `pacman` | `sudo pacman -S git` |

## Helpful Shortcuts

| Shortcut | Description |
| --- | --- |
| `Tab` | Autocompletes commands, file names, and directory names. |
| `Ctrl + C` | Stops the current command. |
| `Ctrl + L` | Clears the terminal screen. |
| `Ctrl + A` | Moves the cursor to the start of the line. |
| `Ctrl + E` | Moves the cursor to the end of the line. |
| Up Arrow | Shows the previous command. |

## Example Workflow

```bash
pwd
mkdir linux-practice
cd linux-practice
touch notes.txt
echo "Learning Linux commands" > notes.txt
cat notes.txt
ls -la
```

This creates a practice directory, creates a text file, writes text into it,
prints the file contents, and lists the directory contents.
