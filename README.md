# 🚀 Day 02 - SSH Key Authentication & Git Essentials

## 📌 Overview

On Day 02 of my DevOps Journey, I learned how to establish a secure connection between a Linux server and GitHub using SSH Keys. I also revised essential Git commands used in daily DevOps workflows.

Secure authentication is a critical skill for DevOps Engineers because it enables safe communication between local systems, cloud servers, and source code repositories.

---

## 🎯 Learning Objectives

* Understand SSH (Secure Shell)
* Learn Public Key & Private Key Authentication
* Generate SSH Keys using Linux
* Configure GitHub Authentication
* Practice essential Git commands
* Follow an industry-standard Git workflow

---

# 🔐 What is SSH?

SSH (Secure Shell) is a cryptographic network protocol used for secure communication between systems over an unsecured network.

### Key Benefits

✅ Secure Authentication

✅ Encrypted Communication

✅ Remote Server Access

✅ Secure GitHub Integration

✅ Industry Standard Security Practice

---

# 🔑 Understanding SSH Key Authentication

SSH Authentication works using a pair of cryptographic keys.

## Private Key

* Stored securely on the local machine
* Never shared with anyone
* Used to prove identity

Example:

```bash
~/.ssh/id_ed25519
```

## Public Key

* Shared with GitHub
* Used for verification

Example:

```bash
~/.ssh/id_ed25519.pub
```

---

# ⚙️ SSH Key Generation

Generate a new SSH Key:

```bash
ssh-keygen -t ed25519 -C "your-email@example.com"
```

### Parameters

| Option     | Description                 |
| ---------- | --------------------------- |
| ssh-keygen | Generates SSH Keys          |
| -t ed25519 | Secure encryption algorithm |
| -C         | Adds a comment/email        |

---

# 🚀 SSH Configuration Process

### Start SSH Agent

```bash
eval "$(ssh-agent -s)"
```

### Add SSH Key

```bash
ssh-add ~/.ssh/id_ed25519
```

### Display Public Key

```bash
cat ~/.ssh/id_ed25519.pub
```

### Test GitHub Authentication

```bash
ssh -T git@github.com
```

Expected Result:

```text
Hi username! You've successfully authenticated.
```

---

# 📚 Essential Git Commands

## Initialize Repository

```bash
git init
```

Creates a new Git repository.

---

## Check Repository Status

```bash
git status
```

Displays current repository state.

---

## Stage Files

```bash
git add .
```

Adds all modified files to the staging area.

---

## Commit Changes

```bash
git commit -m "Added Day 02 Documentation"
```

Creates a snapshot of the staged changes.

---

## View Commit History

```bash
git log
```

Displays repository commit history.

---

## Connect Remote Repository

```bash
git remote add origin <repository-url>
```

Links the local repository with GitHub.

---

## Push Changes

```bash
git push origin main
```

Uploads local commits to GitHub.

---

## Pull Latest Changes

```bash
git pull origin main
```

Downloads the latest updates from GitHub.

---

## Clone Repository

```bash
git clone <repository-url>
```

Creates a local copy of a GitHub repository.

---

# 🔄 Standard Git Workflow

```bash
git status

git add .

git commit -m "Updated Project Documentation"

git push origin main
```

---

# 💼 Real-World DevOps Use Cases

### Infrastructure as Code

Store Terraform and CloudFormation templates securely in GitHub.

### CI/CD Pipelines

Maintain Jenkins, GitHub Actions, and deployment configurations.

### Team Collaboration

Enable multiple engineers to work on the same project efficiently.

### Version Control

Track every change and maintain project history.

---

# 🎤 Interview Questions

### What is SSH?

SSH is a secure protocol used for encrypted communication between systems.

### Why is SSH preferred over password authentication?

SSH provides stronger security through cryptographic key-based authentication.

### What is the difference between a Public Key and a Private Key?

The Public Key is shared for verification, while the Private Key remains secret and is used for authentication.

### What is the purpose of git add?

It moves modified files to the staging area before committing.

### What is the purpose of git commit?

It creates a permanent snapshot of staged changes.

### What is the purpose of git push?

It uploads local commits to a remote GitHub repository.

---

# 🏆 Skills Practiced Today

* Linux Administration
* SSH Authentication
* GitHub Integration
* Git Commands
* Repository Management
* Version Control
* DevOps Fundamentals

---

## 📅 DevOps Journey Progress

✅ Day 01 - Git & GitHub Basics

✅ Day 02 - SSH Authentication & Git Essentials

🚀 Continuous Learning Every Day
# harshu-gite
hii my name is harshu
