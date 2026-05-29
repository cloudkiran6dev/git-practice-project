# Git & GitHub Beginner Practice Notes

# Project: Daily Notes App

This project is for practicing:

* Git basics
* GitHub workflow
* Commits
* Branches
* Merge
* Push/Pull
* Real-world DevOps workflow

---

# Step 1 — Create Project Folder

## Command

```bash
mkdir git-practice-project
```

## What it is

Creates a new folder.

## Why we do this

Git tracks files inside a project folder called a repository.

## Explanation

* `mkdir` = make directory/folder

---

# Step 2 — Move Into the Folder

## Command

```bash
cd git-practice-project
```

## What it is

Moves terminal into the project folder.

## Why we do this

All Git commands should run inside the project directory.

## Explanation

* `cd` = change directory

---

# Step 3 — Open VS Code

## Command

```bash
code .
```

## What it is

Opens current folder in VS Code.

## Why we do this

Makes it easy to create and edit files.

## Explanation

* `.` means current folder

---

# Step 4 — Initialize Git Repository

## Command

```bash
git init
```

## What it is

Initializes Git inside the project.

## What happens internally

Git creates a hidden `.git` folder.

This folder stores:

* commit history
* branch information
* tracking details
* configuration

## Why we do this

Without `.git`, Git cannot track files.

## Important Understanding

You are telling Git:

> “Start tracking this project.”

---

# Step 5 — Create Files

## Create Files

```text
README.md
notes.txt
```

---

## README.md Content

```md
# Daily Notes App

This is my Git practice project.
```

---

## notes.txt Content

```text
Day 1:
Learning Git basics.
```

---

## What is README.md?

A README file explains the project.

Almost every professional project contains a README file.

---

# Step 6 — Check Git Status

## Command

```bash
git status
```

## What it is

Shows current condition of repository.

## It displays

* new files
* modified files
* deleted files
* staged files
* branch information

## Why we do this

Git does not automatically save files.

We must tell Git what should be tracked.

---

## Example Output

```bash
Untracked files:
README.md
notes.txt
```

## Meaning

Git sees files but is not tracking them yet.

---

# Step 7 — Add Files to Staging Area

## Command

```bash
git add .
```

---

# Important Git Workflow

```text
Working Directory
       ↓
Staging Area
       ↓
Repository (Commit)
```

---

## What is `git add`?

Moves files into staging area.

## What is Staging Area?

Temporary preparation area before final save (commit).

## Why staging exists

Developers may want to:

* commit selected files only
* review changes before saving
* organize commits properly

---

## Meaning of `.`

```bash
.
```

Means:

> “Add everything from current folder.”

---

# Step 8 — Commit Changes

## Command

```bash
git commit -m "Initial commit"
```

## What is a commit?

A commit is:

* saved checkpoint
* project snapshot
* version history point

## Why commits are important

Commits help us:

* rollback changes
* recover deleted code
* track history
* understand what changed
* collaborate with teams

---

## Meaning of `-m`

```bash
-m
```

Means message.

Example:

```bash
"Initial commit"
```

Describes what changes were saved.

---

# Step 9 — Create GitHub Repository

## Go to

GitHub official website.

## Create Repository Name

```text
git-practice-project
```

## Important

Do NOT:

* add README
* add .gitignore

Reason:
Local project already contains files.

---

# Step 10 — Connect Local Repository to GitHub

## Command

```bash
git remote add origin https://github.com/USERNAME/git-practice-project.git
```

---

## What is happening?

Connecting:

* local repository

with

* remote GitHub repository

---

## Important Terms

| Term              | Meaning                       |
| ----------------- | ----------------------------- |
| Local Repository  | Project on your computer      |
| Remote Repository | Project stored on GitHub      |
| Origin            | Nickname of remote repository |

---

# Step 11 — Push Code to GitHub

## Command

```bash
git push -u origin master
```

OR

```bash
git push -u origin main
```

(depending on branch name)

---

## What is Push?

Uploads local commits to GitHub.

---

## Meaning of `-u`

Sets default upstream branch.

After this, future push becomes:

```bash
git push
```

---

# Step 12 — Modify Files

## Update notes.txt

```text
Day 2:
Learning branching.
```

---

# Step 13 — Check Repository Status Again

## Command

```bash
git status
```

---

## Example Output

```bash
modified: notes.txt
```

## Meaning

Git detected file changes.

---

# Step 14 — Commit Updated Changes

## Commands

```bash
git add .
git commit -m "Updated notes for day 2"
```

---

# Step 15 — Push Updated Code

## Command

```bash
git push
```

## What happens

Latest commits are uploaded to GitHub.

---

# Step 16 — Create Branch

## Command

```bash
git branch feature-header
```

## What is a Branch?

A separate workspace.

## Why branches are used

Developers can work independently without affecting main code.

---

# Step 17 — Switch Branch

## Commands

```bash
git checkout feature-header
```

OR

```bash
git switch feature-header
```

## What happens

You move from current branch to another branch.

---

# Step 18 — Make Changes in Branch

## Update README.md

```md
## Features
- Daily notes
- Git practice
```

---

# Step 19 — Commit Branch Changes

## Commands

```bash
git add .
git commit -m "Added features section"
```

---

# Step 20 — Merge Branch Into Main

## Switch Back to Main Branch

```bash
git checkout master
```

OR

```bash
git switch main
```

---

## Merge Command

```bash
git merge feature-header
```

---

## What is Merge?

Combines branch changes into main branch.

---

# Step 21 — Push Final Code

## Command

```bash
git push
```

## What happens

Merged code is uploaded to GitHub.

---

# Important Git Concepts

| Concept      | Meaning                    |
| ------------ | -------------------------- |
| Repository   | Project tracked by Git     |
| Commit       | Saved snapshot             |
| Branch       | Separate workspace         |
| Merge        | Combine changes            |
| Push         | Upload code to GitHub      |
| Pull         | Download latest code       |
| Staging Area | Temporary preparation area |

---

# Real Company Workflow

```text
Create Branch
    ↓
Develop Feature
    ↓
Commit Changes
    ↓
Push to GitHub
    ↓
Create Pull Request
    ↓
Code Review
    ↓
Merge
```

This is the standard workflow used in:

* DevOps
* Cloud Engineering
* Software Development
* Platform Engineering

---

# Bonus Practice Tasks

# Task 1 — Create Another Branch

## Command

```bash
git branch feature-login
```

## Create File

```text
login.txt
```

---

# Task 2 — Delete Branch

## Command

```bash
git branch -d feature-login
```

## What it does

Deletes branch locally.

---

# Task 3 — View Commit History

## Command

```bash
git log
```

## What it shows

* commit IDs
* author
* date
* commit messages

---

# Most Important Understanding

# Git vs GitHub

| Git                  | GitHub                     |
| -------------------- | -------------------------- |
| Version control tool | Cloud hosting platform     |
| Works locally        | Works online               |
| Tracks file history  | Stores remote repositories |

---

# Final Learning Outcome

After completing this project, you will understand:

* Git basics
* GitHub workflow
* Local repository
* Remote repository
* Commits
* Branches
* Merge
* Push/Pull
* Real-world developer workflow

This forms the foundation for:

* DevOps
* Terraform Projects
* Azure Projects
* CI/CD Pipelines
* Team Collaboration
