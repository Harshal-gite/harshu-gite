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

