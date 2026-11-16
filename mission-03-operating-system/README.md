# Mission 3 — Understand the operating system

## 1. Task / objective
Explore the operating system environment, active processes, storage usage, file paths, and permissions, and explain core OS responsibilities.

## 2. Work completed

### Task 3.1 — Explore your operating system

| Information explored | What it tells you | Your observation (privacy-safe) |
| :--- | :--- | :--- |
| Operating system / system details (`sw_vers`) | Shows the OS name, version number, and build identifier. | `ProductName: macOS`, `ProductVersion: 27.2.1`, `BuildVersion: 26B131`. |
| Current account identity (`whoami`) | Displays the username of the currently logged-in account. | Returned `[redacted]`. |
| Available and used storage (`df -h /`) | Shows total disk capacity, used space, free space, and mount point. | Total `926Gi`, Used `13Gi`, Available `677Gi` (`2%` capacity) mounted on `/`. |
| System activity snapshot (`ps`) | Lists active processes running in the current Terminal session along with their `PID`. | Showed active shell processes (`zsh`) with their unique `PID` numbers. |

---

### Task 3.2 — Understand processes
- **What is a process?** A process is a running instance of a program currently loaded in memory.
- **What does the PID column represent?** `PID` stands for Process Identifier—a unique number assigned by the OS to identify and manage each running process.
- **Two examples of processes running on my computer:**
  1. `zsh` — the active Terminal shell process running my commands.
  2. `WindowServer` / browser or editor process — the application process running my graphical interface.

---

### Task 3.3 — Understand paths and permissions
- **Difference between an absolute path and a relative path:**
  - An **absolute path** starts from the root directory (`/`) and gives the full location of a file or folder (Example: `/Users/[redacted]/digital-detective-8071/mission-03-operating-system`).
  - A **relative path** gives a location starting from the current working directory without a leading `/` (Example: `mission-03-operating-system/README.md`).
- **File permissions inspection (`ls -l mission-02-terminal/terminal-practice/note.txt`):**
  - Permission string observed: `-rw-r--r--@`
  - The first `-` shows it is a regular file. The next three letters `rw-` are for the **owner**: the owner **can read (`r`)** and **can write (`w`)** to the file, and **cannot execute (`-`)** it.

| Permission | Meaning | Example |
| :--- | :--- | :--- |
| `r` — Read | Allows a file's contents to be viewed or a folder's contents to be listed. | Opening `note.txt` with `cat` |
| `w` — Write | Allows a file to be modified, overwritten, or deleted. | Adding text to `note.txt` |
| `x` — Execute | Allows a file to be run as a program/script, or allows entering a directory (`cd`). | Running a script |

---

### Task 3.4 — Explain operating-system responsibilities

| OS responsibility | Your explanation | Example |
| :--- | :--- | :--- |
| Process management | Starts, schedules, and stops running programs so multiple tasks share the CPU. | Running Terminal and a web browser at the same time. |
| Memory management | Gives RAM to active programs and frees it when they close. | Allocating memory to the shell and text editor. |
| Device management | Controls hardware devices through drivers so software can use them. | Reading keystrokes from the keyboard. |
| File management | Organizes data into files and folders on storage drives. | Saving `README.md` inside `mission-03-operating-system`. |
| User interface / shell | Provides a command line (CLI) or graphical screen (GUI) for user interaction. | Typing basic commands in `zsh`. |
| Security and permissions | Controls who can read, write, or execute files and system resources. | Owner permissions `-rw-r--r--` on `note.txt`. |

## 3. Commands / tools used
- `sw_vers`: Checked macOS name and version.
- `whoami`: Checked active user account (redacted in notes).
- `df -h /`: Checked disk space used and available.
- `ps`: Listed active processes and their `PID` numbers.
- `ls -l`: Checked file permissions (`-rw-r--r--@`).

## 4. My understanding
The operating system manages hardware, memory, running processes, storage files, and permissions so programs run safely. Every active program gets a unique `PID`, and `rwx` permissions control what the owner and other users can do with a file.

## 5. Difficulties faced
No major difficulties.

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
- `mission-03-operating-system/README.md`

## 8. Commit details
Committed with message: "Document operating system and file management" and pushed to GitHub.
