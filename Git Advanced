# Additional Important Git Commands (Beginner to Intermediate)

These are commonly used Git commands after learning:

* init
* add
* commit
* push
* branch
* merge

These commands are heavily used in real projects and DevOps environments.

---

# 1. Clone Repository

## Command

```bash
git clone <repository-url>
```

## Example

```bash
git clone https://github.com/USERNAME/project.git
```

## What it is

Downloads a GitHub repository to local machine.

## Why we use it

Used when:

* joining a company project
* downloading existing code
* collaborating with teams

## What happens internally

Git:

* downloads files
* creates `.git` folder
* connects remote automatically

---

# 2. View Branches

## Command

```bash
git branch
```

## What it is

Shows all local branches.

## Example Output

```bash
* main
  feature-login
```

## Meaning

* `*` = current branch
* other branches are available locally

---

# 3. Create and Switch Branch Together

## Old Method

```bash
git checkout -b feature-api
```

## New Recommended Method

```bash
git switch -c feature-api
```

## What it does

* creates branch
* switches to branch immediately

## Why useful

Saves time.

---

# 4. View Remote Repository Details

## Command

```bash
git remote -v
```

## What it shows

Connected GitHub repository URLs.

## Example Output

```bash
origin  https://github.com/user/project.git (fetch)
origin  https://github.com/user/project.git (push)
```

## Meaning

* fetch = download operations
* push = upload operations

---

# 5. Pull Latest Code from GitHub

## Command

```bash
git pull
```

## What it is

Downloads latest changes from GitHub.

## Why important

In teams:

* other developers push code
* your local repo becomes outdated

`git pull` syncs latest changes.

---

# 6. Fetch Latest Changes

## Command

```bash
git fetch
```

## Difference Between Pull and Fetch

| Command   | Action                     |
| --------- | -------------------------- |
| git fetch | Downloads changes only     |
| git pull  | Downloads + merges changes |

## Why fetch is useful

Lets developers review changes before merging.

---

# 7. Check Commit History

## Command

```bash
git log
```

## What it shows

* commit IDs
* author
* date
* messages

---

# Better Readable Log

## Command

```bash
git log --oneline
```

## Example Output

```bash
a5d44c1 Added login feature
b3c7721 Initial commit
```

## Why useful

Compact commit history.

---

# 8. View File Differences

## Command

```bash
git diff
```

## What it does

Shows exact changes made in files.

## Why useful

Developers verify changes before commit.

---

# 9. Remove File from Git Tracking

## Command

```bash
git rm filename.txt
```

## Example

```bash
git rm notes.txt
```

## What it does

* deletes file
* stages deletion

---

# 10. Rename File

## Command

```bash
git mv oldname.txt newname.txt
```

## Example

```bash
git mv notes.txt daily-notes.txt
```

## What it does

Renames file while preserving Git history.

---

# 11. Ignore Files

# Create `.gitignore`

## Example

```text
node_modules/
*.log
.env
```

## What it is

Tells Git:

> “Do not track these files.”

## Why important

Sensitive or unnecessary files should not go to GitHub.

Examples:

* passwords
* logs
* temporary files
* binaries

---

# 12. Remove Staged Changes

## Command

```bash
git reset
```

## What it does

Removes files from staging area.

## Important

Does NOT delete file changes.

---

# 13. Undo Last Commit

## Command

```bash
git reset --soft HEAD~1
```

## What it does

Removes last commit but keeps code changes.

---

# 14. Completely Remove Last Commit

## Command

```bash
git reset --hard HEAD~1
```

## WARNING

Deletes:

* commit
* code changes

Use carefully.

---

# 15. Check Current Branch

## Command

```bash
git branch --show-current
```

## What it does

Displays current branch name.

---

# 16. Delete Local Branch

## Command

```bash
git branch -d branch-name
```

## Example

```bash
git branch -d feature-login
```

## What it does

Deletes branch locally.

---

# 17. Force Delete Branch

## Command

```bash
git branch -D branch-name
```

## Why needed

Deletes branch even if not merged.

---

# 18. Push New Branch to GitHub

## Command

```bash
git push -u origin feature-login
```

## What it does

Uploads branch to GitHub.

---

# 19. View All Branches

## Command

```bash
git branch -a
```

## What it shows

* local branches
* remote branches

---

# 20. Stash Temporary Changes

## Command

```bash
git stash
```

## What it does

Temporarily saves unfinished changes.

## Why useful

Developer can:

* switch branch quickly
* work on urgent issue
* return later

---

# View Stash List

## Command

```bash
git stash list
```

---

# Restore Stash

## Command

```bash
git stash pop
```

---

# 21. Check Repository History Graph

## Command

```bash
git log --oneline --graph --all
```

## What it shows

Visual branch history.

---

# 22. View Configurations

## Command

```bash
git config --list
```

## What it shows

Git username, email, settings.

---

# 23. Set Username

## Command

```bash
git config --global user.name "Kiran Kumar"
```

---

# 24. Set Email

## Command

```bash
git config --global user.email "yourmail@gmail.com"
```

## Why important

Commits are linked to your identity.

---

# 25. View Connected Remote

## Command

```bash
git remote
```

## Example Output

```bash
origin
```

---

# 26. Remove Remote Repository

## Command

```bash
git remote remove origin
```

## What it does

Disconnects GitHub repository.

---

# 27. Change Remote Repository URL

## Command

```bash
git remote set-url origin NEW_URL
```

---

# 28. Tagging Releases

## Create Tag

```bash
git tag v1.0
```

## Push Tag

```bash
git push origin v1.0
```

## Why used

Marks release versions.

Examples:

* v1.0
* v2.0
* production release

---

# 29. See Tags

## Command

```bash
git tag
```

---

# 30. Cherry Pick Commit

## Command

```bash
git cherry-pick COMMIT_ID
```

## What it does

Copies specific commit from another branch.

---

# Important Real-World Workflow

```text
Clone Repository
       ↓
Create Branch
       ↓
Make Changes
       ↓
git add .
       ↓
git commit
       ↓
git push
       ↓
Create Pull Request
       ↓
Code Review
       ↓
Merge
       ↓
git pull
```

---

# Most Important Git Commands Summary

| Command       | Purpose                  |
| ------------- | ------------------------ |
| git init      | Initialize repository    |
| git clone     | Download repository      |
| git status    | Check repository status  |
| git add .     | Stage changes            |
| git commit    | Save snapshot            |
| git push      | Upload changes           |
| git pull      | Download latest changes  |
| git fetch     | Download without merge   |
| git branch    | View branches            |
| git switch    | Change branch            |
| git merge     | Combine branches         |
| git log       | View history             |
| git diff      | View changes             |
| git stash     | Temporary save           |
| git reset     | Undo staging/commits     |
| git remote -v | View remote repositories |
| git tag       | Create releases          |

---

# Final Understanding

After learning these commands, you will understand:

* Local Git workflow
* GitHub workflow
* Team collaboration
* Branching strategy
* Real-world DevOps practices
* Production development workflow
