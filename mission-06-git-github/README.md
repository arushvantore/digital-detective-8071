# Mission 6 — Git and GitHub in practice

## 1. Task / objective
Practice the core Git workflow (`status`, `add`, `commit`, `log`), create and push a feature branch (`update-about`), open a Pull Request on GitHub, and build a personal Git command glossary.

## 2. Work completed

### Task 6.1 — Understand the basic Git workflow

| Git operation | What it does in your own words |
| :--- | :--- |
| Check repository status (`git status`) | Shows which branch I am on, which files were modified or created, and whether changes are staged for the next commit. |
| Stage selected changes (`git add <file>`) | Adds specific modified or new files into the staging area so Git prepares them for the next commit snapshot. |
| Create a commit (`git commit -m "..."`) | Saves a permanent snapshot of all staged changes into the local repository history along with a descriptive message. |
| View commit history (`git log`) | Displays the chronological list of past commits, including their commit IDs, author, dates, and messages. |

**Difference between staging a change and committing it:**
Staging (`git add`) is like putting chosen items into a box before sealing it—you can add or remove files before saving. Committing (`git commit`) permanently seals that box and records it as a numbered checkpoint in Git history.

---

### Task 6.2 — Create and use a branch
- Created and switched to a new branch named `update-about` using `git checkout -b update-about`.
- Added a `## My Learning` section to the root `README.md` summarizing key takeaways so far.
- Checked `git status`, staged `README.md`, committed with message `"Add My Learning section to root README"`, and pushed the branch to GitHub (`git push -u origin update-about`).

---

### Task 6.3 — Create a Pull Request
- Opened a Pull Request on GitHub from `update-about` into `main` with a summary of the `README.md` update.
- **PR Status:** The Pull Request is currently **open (unmerged)** on GitHub as instructed (merging is left pending instructor approval), and I switched back to my local `main` branch (`git checkout main`) to continue Mission 6 documentation.

**What a branch and a Pull Request are, and why they are useful:**
- A **branch** is an independent copy of the codebase where you can safely build or test changes without breaking the main working version.
- A **Pull Request (PR)** is a formal request on GitHub asking to review and merge changes from one branch into another. Together, they allow multiple people to work on features simultaneously, review code for bugs, and keep the `main` branch stable.

---

### Task 6.4 — Build your Git command glossary

| Git operation | One-line explanation in your own words |
| :--- | :--- |
| Initialise a repository (`git init`) | Creates a new hidden `.git` database inside a folder so Git starts tracking file changes there. |
| Check status (`git status`) | Lists modified, untracked, and staged files on the current branch. |
| Stage changes (`git add`) | Moves selected file changes into the staging area to prepare them for a commit. |
| Commit changes (`git commit`) | Records a permanent snapshot of staged changes in local Git history with a message. |
| View history (`git log`) | Shows the list of previous commits with their IDs, timestamps, and messages. |
| Create or list branches (`git branch`) | Lists all local branches or creates a new branch without switching to it. |
| Switch branches (`git checkout` / `git switch`) | Moves your working directory from one branch to another. |
| Publish changes (`git push`) | Uploads local commits from your computer up to a remote repository like GitHub. |
| Retrieve remote changes (`git pull` / `git fetch`) | Downloads new commits from a remote repository like GitHub onto your local computer. |

## 3. Commands / tools used
- `git status`, `git add`, `git commit`, `git log`: Inspected changes, staged files, recorded commits, and verified history.
- `git checkout -b update-about` and `git push -u origin update-about`: Created and published the feature branch.
- `git checkout main`: Switched back to the `main` branch after opening the Pull Request on GitHub.

## 4. My understanding
Git tracks project history locally using staging (`git add`) and snapshots (`git commit`), while GitHub hosts repositories online and enables safe collaboration through branches and Pull Requests.

## 5. Difficulties faced
No major difficulties.

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
- `mission-06-git-github/README.md`
- Branch `update-about` and open Pull Request on GitHub (`arushvantore/digital-detective-8071`)

## 8. Commit details
Committed with message: "Complete Git and GitHub collaboration mission" and pushed to GitHub.
