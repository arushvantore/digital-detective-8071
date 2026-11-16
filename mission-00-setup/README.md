# Mission 0 — Create your GitHub workspace

## 1. Task / objective
Create a public GitHub repository named `digital-detective-8071`, build the required mission folder structure, prepare the root README, and verify Python 3 and Git tools.

## 2. Work completed
- Created the local workspace folder `digital-detective-8071`.
- Created all 9 mission folders (`mission-00-setup` through `mission-08-final-report`) and the `evidence/` folder.
- Created placeholder `README.md` files inside all mission folders and `number_converter.py` inside `mission-05-numbers-data/`.
- Prepared the root `README.md` with the project title, short description, mission index links, and sequential commit rule.

## 3. Commands / tools used
- `pwd`: Checked the current working directory path.
- `git init`: Initialized a local Git repository.
- `git mv`: Renamed `mission-0` to `mission-00-setup` while keeping Git history.
- `mkdir -p` and `touch`: Created all required mission folders and placeholder files.
- `python3 --version`: Checked Python installation (`Python 3.15.2`).
- `git --version`: Checked Git installation (`git version 2.55.0`).

## 4. My understanding
A repository is a project folder tracked by Git that saves snapshots of file changes over time and connects to GitHub for online backup. Organizing the workspace by mission folders keeps each topic, script, and output clean and easy to review.

## 5. Difficulties faced
Initially created `mission-0` instead of `mission-00-setup` and ran `mkdir` while inside that subfolder.

## 6. How I resolved them
Moved back to the root folder with `cd ~/digital-detective-8071`, cleaned the misplaced folders, renamed the directory using `git mv`, and recreated the folders in the root directory.

## 7. Evidence / files
- `README.md`
- `mission-00-setup/README.md`

## 8. Commit details
Committed the complete Mission 0 setup with message `"Set up Digital Detective mission structure"` and pushed to GitHub.
