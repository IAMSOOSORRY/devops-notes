# Day 1 - Linux & Git Command Notes

## 1. pwd

### Command

```bash
pwd
```

### Meaning

Print Working Directory

Shows the current location in the Linux filesystem.

### Example

```bash
pwd
```

Output:

```text
/home/ubuntu/DevOps/devops-notes
```

---

## 2. ls

### Command

```bash
ls
```

### Meaning

List files and folders in the current directory.

### Example

```bash
ls
```

Output:

```text
Day-01-Linux-Fundamentals
README.md
```

---

## 3. ls -la

### Command

```bash
ls -la
```

### Meaning

* `-l` = Long listing format
* `-a` = Show all files including hidden files

### Example

```bash
ls -la
```

Shows:

* Permissions
* Owner
* Size
* Hidden files

---

## 4. cd

### Command

```bash
cd foldername
```

### Meaning

Change Directory.

### Examples

```bash
cd Day-01-Linux-Fundamentals
```

Move into a folder.

```bash
cd ..
```

Move one level up.

```bash
cd ~
```

Go to home directory.

---

## 5. mkdir

### Command

```bash
mkdir Linux
```

### Meaning

Make Directory.

Creates a new folder.

### Example

```bash
mkdir Docker
```

Creates:

```text
Docker/
```

---

## 6. mkdir -p

### Command

```bash
mkdir -p DevOps/Linux
```

### Meaning

Creates parent directories automatically if they do not exist.

### Example

```bash
mkdir -p DevOps/Linux
```

Creates:

```text
DevOps/
└── Linux/
```

---

## 7. tree

### Command

```bash
tree
```

### Meaning

Displays folders and files in a tree structure.

### Example

```text
DevOps
├── Docker
├── Jenkins
├── Kubernetes
└── Linux
```

---

## 8. touch

### Command

```bash
touch notes.md
```

### Meaning

Creates an empty file.

### Example

```bash
touch notes.md
```

Creates:

```text
notes.md
```

---

## 9. nano

### Command

```bash
nano notes.md
```

### Meaning

Opens a file in the Nano text editor.

### Save

```text
Ctrl + O
Enter
```

### Exit

```text
Ctrl + X
```

---

# Git Commands

## 10. git status

### Command

```bash
git status
```

### Meaning

Shows the current status of the repository.

### Displays

* Modified files
* Untracked files
* Staged files

---

## 11. git add .

### Command

```bash
git add .
```

### Meaning

Adds all files to the staging area.

### Git Workflow

```text
Working Directory
       ↓
Staging Area
       ↓
Commit
```

---

## 12. git commit

### Command

```bash
git commit -m "Day 1 Linux Fundamentals"
```

### Meaning

Creates a snapshot of the current changes.

Think of it as saving your work permanently in Git history.

---

## 13. git branch -M main

### Command

```bash
git branch -M main
```

### Meaning

Renames the current branch to main.

Example:

```text
master → main
```

---

## 14. git remote add origin

### Command

```bash
git remote add origin git@github.com:IAMSOOSORRY/devops-notes.git
```

### Meaning

Connects the local repository to a GitHub repository.

### Breakdown

* `git remote` → Manage remote repositories
* `add` → Add a remote
* `origin` → Remote nickname
* Repository URL → GitHub repository address

---

## 15. git remote -v

### Command

```bash
git remote -v
```

### Meaning

Displays configured remote repositories.

### Example

```text
origin git@github.com:IAMSOOSORRY/devops-notes.git
```

---

## 16. ssh -T [git@github.com](mailto:git@github.com)

### Command

```bash
ssh -T git@github.com
```

### Meaning

Tests SSH authentication with GitHub.

### Success Message

```text
Hi IAMSOOSORRY!
You've successfully authenticated.
```

---

## 17. git push

### Command

```bash
git push
```

### Meaning

Uploads local commits to GitHub.

### Flow

```text
Local Repository
       ↓
GitHub Repository
```

---

## 18. git push -u origin main

### Command

```bash
git push -u origin main
```

### Meaning

Pushes code to the main branch and sets upstream tracking.

### Breakdown

* `push` → Upload commits
* `origin` → Remote repository
* `main` → Branch name
* `-u` → Set upstream branch

After this, you can simply use:

```bash
git push
```

---

## 19. .git Directory

### Meaning

Hidden directory created by Git.

Contains:

* Commit history
* Branch information
* Logs
* Repository configuration

Never delete it unless you want to remove Git tracking.

---

## 20. .gitkeep

### Command

```bash
touch .gitkeep
```

### Meaning

Allows Git to track an otherwise empty folder.

### Why?

Git tracks files, not empty directories.

Example:

```text
Linux/
└── .gitkeep
```

This ensures the folder appears in GitHub.

---

# Day 1 Summary

## Linux Commands Learned

* pwd
* ls
* ls -la
* cd
* mkdir
* mkdir -p
* tree
* touch
* nano

## Git Commands Learned

* git status
* git add .
* git commit
* git branch -M main
* git remote add origin
* git remote -v
* ssh -T [git@github.com](mailto:git@github.com)
* git push
* git push -u origin main

## Concepts Learned

* Linux File System
* Directories and Files
* Hidden Files
* Git Repository
* GitHub Integration
* SSH Authentication
* Empty Directory Handling with .gitkeep
