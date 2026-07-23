# Day 11 - Git Basics

## Objective

Learn the fundamentals of Git and understand how version control works in real-world DevOps projects.

---

# What is Git?

Git is a Distributed Version Control System (VCS) used to track changes in files and source code.

Git helps developers and DevOps engineers:

- Track changes
- Collaborate with teams
- Maintain code history
- Roll back changes when required

---

# Why Git is Important in DevOps?

Git is used to store:

- Application Source Code
- Terraform Code
- Kubernetes YAML Files
- Dockerfiles
- Jenkinsfiles
- Shell Scripts

Almost every DevOps project uses Git.

---

# What is a Repository?

A Repository (Repo) is a folder tracked by Git.

Example:

```text
project/
├── Dockerfile
├── Jenkinsfile
├── deployment.yaml
└── README.md
```

Git tracks all changes inside the repository.

---

# Git Workflow

```text
Working Directory
       ↓
git add
       ↓
Staging Area
       ↓
git commit
       ↓
Git Repository
```

---

# 1. git init

## Purpose

Initializes a new Git repository.

## Syntax

```bash
git init
```

## Example

```bash
mkdir project

cd project

git init
```

## Use Case

Start version control in a new project.

---

# 2. git status

## Purpose

Shows the current status of the repository.

## Syntax

```bash
git status
```

## Displays

- New files
- Modified files
- Staged files
- Untracked files

## Use Case

Check repository status before committing changes.

---

# 3. git add

## Purpose

Adds files to the staging area.

## Syntax

```bash
git add file.txt
```

Add all files:

```bash
git add .
```

## Use Case

Prepare changes before creating a commit.

---

# 4. git commit

## Purpose

Saves changes in Git history.

## Syntax

```bash
git commit -m "Initial commit"
```

## Example

```bash
git commit -m "Added Docker Notes"
```

## Use Case

Create a snapshot of the current state of the project.

---

# 5. git log

## Purpose

Displays commit history.

## Syntax

```bash
git log
```

## Information Displayed

- Commit ID
- Author
- Date
- Commit Message

## Use Case

Check previous commits and project history.

---

# 6. git diff

## Purpose

Shows changes before committing.

## Syntax

```bash
git diff
```

## Use Case

Verify modifications before adding or committing them.

---

# Real DevOps Scenarios

## Scenario 1: Review Changes Before Deployment

Check:

```bash
git diff
```

Verify what has changed.

---

## Scenario 2: Verify Repository Status

Check:

```bash
git status
```

Before creating a commit.

---

## Scenario 3: Check Commit History

Use:

```bash
git log
```

To identify who made changes and when.

---

## Scenario 4: Save Infrastructure Changes

After modifying Terraform files:

```bash
git add .

git commit -m "Updated EC2 configuration"
```

---

# Hands-On Practice

```bash
mkdir git-practice

cd git-practice

git init

touch notes.txt

git status

git add .

git commit -m "Initial commit"

git log

git diff
```

---

# Interview Questions and Answers

## What is Git?

Git is a distributed version control system used to track changes in files and source code.

---

## What is a Repository?

A repository is a folder tracked and managed by Git.

---

## What does git init do?

Creates a new Git repository.

---

## What does git status show?

Shows the current state of the repository and file changes.

---

## What does git add do?

Moves changes to the staging area before committing.

---

## What is a commit?

A commit is a snapshot of changes stored in Git history.

---

## What does git commit do?

Saves staged changes into the repository.

---

## What does git log do?

Displays commit history.

---

## What does git diff do?

Shows differences between current and previous versions of files.

---

## Difference between git add and git commit?

git add:
Moves files to staging area.

git commit:
Saves staged changes permanently in Git history.

---

# Day 11 Summary

Topics Covered:

✅ Git

✅ Repository

✅ git init

✅ git status

✅ git add

✅ git commit

✅ git log

✅ git diff

✅ Git Workflow

✅ Real DevOps Scenarios

Day 11 Status: Completed ✅
