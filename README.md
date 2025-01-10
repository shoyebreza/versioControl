# Git and GitHub Version Control System

## Table of Contents

1. [Initializing a Git Repository](#initializing-a-git-repository)
2. [Working Directory](#working-directory)
3. [Viewing the Status](#viewing-the-status)
4. [Staging Files](#staging-files)
5. [Committing Changes](#committing-changes)
6. [Viewing Commit Logs](#viewing-commit-logs)
7. [Branch Management](#branch-management)
8. [Connecting to a GitHub Repository](#connecting-to-a-github-repository)
9. [Pushing Code to GitHub](#pushing-code-to-github)
10. [Ignoring Files and Folders](#ignoring-files-and-folders)
11. [Unstaging Files and Folders](#unstaging-files-and-folders)
12. [Reverting Changes and Restoring Code](#reverting-changes-and-restoring-code)

---

## 1. Initializing a Git Repository
To initialize a Git repository, run:
```bash
git init
```

---

## 2. Working Directory
To add a file to the staging area:
```bash
git add filename
```
To add all files to the staging area:
```bash
git add .
```

---

## 3. Viewing the Status
To check the status of your working directory and staging area:
```bash
git status
```

---

## 4. Staging Files
To stage specific or all files:
```bash
# Add a specific file
git add filename

# Add all files
git add .
```

---

## 5. Committing Changes
To commit the staged changes with a message:
```bash
git commit -m "project setup"
```

---

## 6. Viewing Commit Logs
To view the commit history:
```bash
git log
```
To view a concise commit log:
```bash
git log --oneline
```
Exit the log view by pressing `Q`.

---

## 7. Branch Management
- To create a new branch:
  ```bash
  git branch branch_name
  ```
- To switch to a branch:
  ```bash
  git checkout branch_name
  ```
- To rename the current branch to `main`:
  ```bash
  git branch -M main
  ```
- To check the current branch:
  ```bash
  git branch
  ```
- To merge a branch into `main`:
  ```bash
  git merge branch_name
  ```

---

## 8. Connecting to a GitHub Repository
To connect your local repository to a remote GitHub repository:
```bash
git remote add origin https://github.com/shoyebreza/versionControl.git
```

---

## 9. Pushing Code to GitHub
To push code to the `main` branch:
```bash
git push -u origin main
```
To push changes to a specific branch:
```bash
git push origin branch_name
```

---

## 10. Ignoring Files and Folders
Create a `.gitignore` file and add the names of files or folders to exclude them from tracking:
```bash
# Ignore specific files
file_name

# Ignore a folder
folder_name/
```

---

## 11. Unstaging Files and Folders
- To unstage a specific file:
  ```bash
  git rm --cached filename
  ```
- To unstage a folder:
  ```bash
  git rm -r --cached folder_name/
  ```

---

## 12. Reverting Changes and Restoring Code
- To revert back to a specific commit:
  ```bash
  git checkout commit_hash
  ```
- To restore files to their last committed state:
  ```bash
  git restore filename
  
