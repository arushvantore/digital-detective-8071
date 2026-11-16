# Mission 2 — Become comfortable with the Terminal

## 1. Task / objective
Use the command-line interface (CLI) to navigate folders, inspect directory contents, create and manage practice files safely, explain flags and pipes, and describe package managers.

## 2. Work completed

### Task 2.1 — Explore basic Terminal operations

| Operation / command name | What it does | What I observed |
| :--- | :--- | :--- |
| Current-directory display (`pwd`) | Prints the full path of the folder I am currently working in. | Showed `/Users/[redacted]/digital-detective-8071/mission-02-terminal`. |
| Directory listing (`ls`) | Lists visible files and folders in the current location. | Listed `README.md` and the practice directory. |
| Detailed listing (`ls -la`) | Lists all files (including hidden ones) with permissions, owner, size, and date. | Showed `.`, `..`, and `README.md` with owner `[redacted]` and size `0`. |
| Change directory (`cd ..`) | Moves up one level to the parent folder. | Prompt path changed back to `~/digital-detective-8071`. |
| Create directory (`mkdir`) | Creates a new folder with the specified name. | Created `terminal-practice` without error output. |
| Create empty file (`touch`) | Creates a new blank file if it does not already exist. | Created `note.txt` inside `terminal-practice`. |
| Copy file (`cp`) | Duplicates a file to a new file name or path. | Created `note_copy.txt` while keeping the original `note.txt`. |
| Move / rename file (`mv`) | Moves a file or renames it in place. | Renamed `note_copy.txt` to `note_renamed.txt`. |
| Display file contents (`cat`) | Prints the text contents of a file in the Terminal. | Displayed both `Line 1: Initial note` and `Line 2: Appended note`. |

---

### Task 2.2 — Practise file changes safely
- Created `terminal-practice`, created `note.txt`, wrote `Line 1: Initial note` using `>`, appended `Line 2: Appended note` using `>>`, verified both lines with `cat`, made a backup copy with `cp`, and renamed it to `note_renamed.txt` with `mv`.

**Answers to Task 2.2 questions:**
- **Difference between replacing a file's contents (`>`) and adding text to the end (`>>`):** `>` overwrites the entire file and erases previous text, whereas `>>` appends new text to the end without deleting existing lines.
- **Difference between copying a file (`cp`) and moving a file (`mv`):** `cp` creates a second independent copy so both files remain, whereas `mv` relocates or renames the original file so only one exists.
- **What information the current-directory display (`pwd`) provides:** It prints my exact full folder path from the root directory (`/`), confirming where my commands will run.
- **Why a directory-listing operation (`ls`) is useful:** It shows which files and subfolders exist in a directory and, with flags like `-la`, reveals file sizes, permissions, and timestamps.

---

### Task 2.3 — Flags and pipes
- **Command run:** `ls -lh terminal-practice | head -n 5`
- **What it does:** `ls -lh` lists files in long format (`-l`) with human-readable sizes (`-h`, showing `43B`). The pipe (`|`) passes that output directly into `head -n 5`, which displays only the first 5 lines.

---

### Task 2.4 — Package managers
- **Package manager checked:** Homebrew (`brew --version` returned `Homebrew 7.0.12`).
- **Why package managers are useful:** They automate installing, updating, and removing software tools and dependencies from one command instead of manual web downloads.

## 3. Commands / tools used
- `pwd`, `ls`, `ls -la`, `cd ..`: Checked current location, listed files, and navigated directories.
- `mkdir`, `touch`, `echo`, `cat`, `cp`, `mv`: Created `terminal-practice` and safely created, edited, copied, and renamed files.
- `ls -lh terminal-practice | head -n 5`: Used flags and a pipe (`|`) to format and limit output.
- `brew --version`: Verified Homebrew (`7.0.12`) is installed.

## 4. My understanding
The Terminal provides fast, direct control over files and directories using short commands. Flags modify command behavior, redirection operators (`>` and `>>`) control how output is saved, and pipes (`|`) connect commands together.

## 5. Difficulties faced
Initially created the practice folder as `practice` instead of `terminal-practice`.

## 6. How I resolved them
Renamed the directory to `terminal-practice` using `mv`.

## 7. Evidence / files
- `mission-02-terminal/README.md`
- `mission-02-terminal/terminal-practice/note.txt`
- `mission-02-terminal/terminal-practice/note_renamed.txt`

## 8. Commit details
Committed with message: "Complete Terminal commands and file operations mission" and pushed to GitHub.
