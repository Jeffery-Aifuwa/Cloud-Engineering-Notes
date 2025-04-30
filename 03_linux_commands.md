# Linux Commands Learned

---

## 🖥️ System Information Commands

- `uname` – Displays system information.
- `uname -a` – Shows detailed system info.
- `uptime` – Shows how long the system has been running.
- `who` – Shows all users currently logged into the system.
- `whoami` – Displays the current logged-in user.
- `free -h` – Displays memory usage in a human-readable format.
- `history` – Lists previously executed commands.
- `date` – Displays the current date and time.
- `ps` – Lists running processes.
- `ps aus` – Lists running processes with detailed information.
- `top` – Shows real-time system resource usage.
- `q` – Quits the top command.
- `df` – Displays disk space usage.
- `df -h` – Shows disk space usage in human-readable format.

---

## 📁 Basic Navigation and File Management Commands

- `pwd` – Prints the current working directory.
- `cd [directory]` – Changes directory.
- `ls` – Lists files and directories in the current location.
- `mkdir [directory]` – Creates a new directory.
- `touch [filename]` – Creates an empty file.
- `cp [source] [destination]` – Copies a file or directory.
- `mv [source] [destination]` – Moves or renames a file.
- `rm [filename]` – Deletes a file.
- `cat [filename]` – Displays the contents of a file.
- `head [filename]` – Shows the first 10 lines of a file.
- `tail [filename]` – Shows the last 10 lines of a file.
- `find [directory] -name "filename"` – Searches for a file in a specific directory.
- `grep "text" filename` – Searches for a specific text within a file.

---

## 🔄 Process Management

- `kill [PID]` – Terminates a process by its Process ID (PID).  
  Example: `kill 1234`
- `pkill process_name` – Terminates a process by name.  
  Example: `pkill firefox`
- `htop` – Interactive process viewer (more user-friendly than `top`).  
  *(Requires installation: `sudo apt install htop`)*

---

## 📦 Additional Linux Commands

- `ln` – Creates a symbolic link (shortcut) to another file.  
  Example: `ln -s /path/to/original /path/to/link`
- `less filename.txt` – Helps to easily move down a large file using the enter key.
- `tar` – Create/compress and extract archived files.  
  - `tar -cvf archive.tar file1 file2`  
  - `tar -xvf archive.tar`
- `diff file1.txt file2.txt` – Find the difference between two files.
- `cmp file1.txt file2.txt` – Check if two files are identical.
- `sort filename.txt` – Sort the content of a file.
- `zip archive.zip file1 file2` – Zip files.
- `unzip archive.zip` – Unzip files.
- `cal` – View a command-line calendar.
- `alias` – Create custom shortcuts for frequently used commands.

---

> 💡 Mastering these commands is essential for navigating and managing Linux systems effectively.
