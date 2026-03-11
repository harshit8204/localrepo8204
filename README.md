# 🗂️ localrepo8204 — Git Practice & Version Control Reference

<div align="center">

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Commits](https://img.shields.io/badge/Commits-8-brightgreen?style=for-the-badge)

**A hands-on Git practice repository — documenting real workflows for initialising repos, staging, committing, branching, and pushing to GitHub.**

[📖 View Commits](https://github.com/harshit8204/localrepo8204/commits/main) &nbsp;·&nbsp; [🌿 View Branches](https://github.com/harshit8204/localrepo8204/branches)

</div>

---

## 📌 Table of Contents

- [About](#-about)
- [Repository Structure](#-repository-structure)
- [Git Concepts Practised](#-git-concepts-practised)
- [Core Git Commands Reference](#-core-git-commands-reference)
- [Typical Workflow](#-typical-workflow)
- [Key Lessons Learned](#-key-lessons-learned)
- [Roadmap](#-roadmap)
- [Author](#-author)

---

## 💡 About

**localrepo8204** is a dedicated Git practice and learning repository. It was created to get hands-on experience with real Git workflows — from initialising a local repository and making commits, to pushing code to GitHub and managing branches.

Rather than just reading about Git, this repo documents the actual process of **doing it** — with real files, real commits, and real version history.

> Every developer starts somewhere. This repo is proof that the fundamentals were taken seriously.

The project contains:
- 📁 `localrepo/` — local repository practice files and exercises
- 📄 `my-demo` — a demo file used to practice staging, committing, and pushing

---

## 📁 Repository Structure

```
localrepo8204/
│
├── localrepo/          # Local Git workflow practice files
│   └── ...             # HTML/CSS files used for commit exercises
│
├── my-demo             # Demo file — used to practise git add, commit, push
└── README.md           # Project documentation
```

---

## 🧰 Git Concepts Practised

This repository was used to get hands-on with the following Git fundamentals:

| Concept | Description |
|---------|-------------|
| 🏗️ **`git init`** | Initialising a brand-new local repository |
| 📋 **`git status`** | Checking which files are staged, unstaged, or untracked |
| ➕ **`git add`** | Staging files — adding changes to the index |
| 💾 **`git commit`** | Saving snapshots of the codebase with meaningful messages |
| 🔗 **`git remote add`** | Linking a local repo to a GitHub remote |
| 🚀 **`git push`** | Uploading commits to the remote GitHub repository |
| 📥 **`git pull`** | Fetching and merging remote changes locally |
| 🌿 **`git branch`** | Creating and listing branches |
| 🔀 **`git checkout`** | Switching between branches |
| 🔁 **`git merge`** | Merging branch changes into main |
| 📜 **`git log`** | Viewing full commit history |

---

## 📖 Core Git Commands Reference

A personal cheatsheet built from this repo's practice sessions:

### 🏁 Setting Up

```bash
# Configure your identity (one-time setup)
git config --global user.name "Your Name"
git config --global user.email "you@example.com"

# Initialise a new local repository
git init

# Clone an existing GitHub repository
git clone https://github.com/username/repo-name.git
```

### 📸 Staging & Committing

```bash
# Check current status of working directory
git status

# Stage a specific file
git add filename.html

# Stage ALL changed files
git add .

# Commit staged changes with a message
git commit -m "feat: add navigation bar to index.html"

# Stage and commit in one step (tracked files only)
git commit -am "fix: update button styles"
```

### 🌍 Working with GitHub (Remote)

```bash
# Link local repo to GitHub remote
git remote add origin https://github.com/username/repo-name.git

# Verify remote connection
git remote -v

# Push commits to GitHub (first time)
git push -u origin main

# Push subsequent commits
git push

# Pull latest changes from GitHub
git pull origin main
```

### 🌿 Branching & Merging

```bash
# List all branches
git branch

# Create a new branch
git branch feature/new-feature

# Switch to a branch
git checkout feature/new-feature

# Create AND switch to a new branch (shorthand)
git checkout -b feature/new-feature

# Merge a branch into main
git checkout main
git merge feature/new-feature

# Delete a branch after merging
git branch -d feature/new-feature
```

### 🔍 History & Inspection

```bash
# View full commit history
git log

# View compact one-line history
git log --oneline

# View changes not yet staged
git diff

# View changes already staged
git diff --staged

# Undo last commit (keep changes staged)
git reset --soft HEAD~1

# Discard all local changes (CAUTION: irreversible)
git checkout -- .
```

---

## 🔄 Typical Workflow

The standard day-to-day Git workflow practised in this repo:

```
1. Make changes to files
         │
         ▼
2. git status          ← See what changed
         │
         ▼
3. git add .           ← Stage all changes
         │
         ▼
4. git commit -m "..."  ← Save a snapshot
         │
         ▼
5. git push            ← Upload to GitHub
         │
         ▼
6. Repeat ✅
```

---

## 💡 Key Lessons Learned

- ✅ Always write **clear, descriptive commit messages** — future-you will thank you
- ✅ **Commit often, commit small** — small commits are easier to review and revert
- ✅ Use **branches** for every new feature or fix — never work directly on `main`
- ✅ Always `git pull` before starting new work to avoid merge conflicts
- ✅ `.gitignore` is essential — never commit `node_modules/`, `.env`, or OS files
- ✅ `git status` and `git log --oneline` are your best friends

---

## 🗺️ Roadmap

- [x] Initialise local repo and push to GitHub
- [x] Practice `add`, `commit`, `push` workflow
- [x] Explore branching and merging
- [x] Build 8+ meaningful commits with real file changes
- [ ] 🔜 Practice rebasing (`git rebase`)
- [ ] 🔜 Resolve merge conflicts intentionally
- [ ] 🔜 Explore `git stash` for temporary work storage
- [ ] 🔜 Set up a `.gitignore` template
- [ ] 🔜 Practice pull requests & code review on GitHub

---

## 🤝 Contributing

This is a personal learning repository, but suggestions and improvements are always welcome!

1. Fork the repository
2. Create a branch: `git checkout -b improve/git-notes`
3. Commit: `git commit -m "docs: add git stash examples"`
4. Push: `git push origin improve/git-notes`
5. Open a Pull Request

---

## 👤 Author

**Harshit**

[![GitHub](https://img.shields.io/badge/GitHub-harshit8204-181717?style=flat-square&logo=github)](https://github.com/harshit8204)

---

## 📄 License

This project is open source under the **MIT License**.

---

<div align="center">

*Every expert was once a beginner. Every pro was once an amateur.*
*The commits don't lie — this is where the Git journey started.* 🚀

⭐ **Found this Git reference helpful? Give it a star!**

</div>
