# Mission 4 — How programs run

## 1. Task / objective
Create and run a Python program (`hello.py`) from the Terminal and compare how compilers and interpreters execute programs.

## 2. Work completed

### Task 4.1 — Create and run a Python program
- Created `hello.py` inside `mission-04-programs/` containing `print("Hello from Python")`.
- Executed the file using `python3 mission-04-programs/hello.py` in Terminal and confirmed `Hello from Python` printed on screen.

---

### Task 4.2 — Compare compiler and interpreter

| Point | Compiler | Interpreter |
| :--- | :--- | :--- |
| When translation / execution happens | Translates the entire source code file into machine code before the program runs. | Translates and executes code line by line while the program is running. |
| Typical output | Produces a standalone executable binary file (such as `.exe` or a macOS binary). | Does not produce a separate executable file; runs instructions directly. |
| One example | C or C++ (using `gcc` / `clang`) | Python (`python3`) |
| One advantage | Runs very fast once compiled because translation is already finished. | Easier to test and debug quickly because code runs immediately without a separate build step. |

**Comparison in my own words:**
A compiler translates the whole program into machine code ahead of time and saves an executable file that runs directly on the CPU. An interpreter reads and executes the source code step by step at runtime without creating a separate binary file. Because of this, compiled programs usually run faster, while interpreted languages like Python are faster to write, test, and debug.

## 3. Commands / tools used
- `echo 'print("Hello from Python")' > mission-04-programs/hello.py`: Created the Python program file.
- `python3 mission-04-programs/hello.py`: Ran the Python script using the Python 3 interpreter.
- Git (`git add`, `git commit`, `git push`): Committed and pushed Mission 4 to GitHub.

## 4. My understanding
Computers only execute low-level machine instructions, so human-readable programming languages need either a compiler or an interpreter to translate them. Python uses an interpreter (`python3`) to read and execute `hello.py` immediately at runtime.

## 5. Difficulties faced
No major difficulties.

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
- `mission-04-programs/hello.py`
- `mission-04-programs/README.md`

## 8. Commit details
Committed with message: "Compare compilers and interpreters" and pushed to GitHub.
