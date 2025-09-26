# 🚀 DevOps Git Project – Task 4

This repository demonstrates **Git & GitHub best practices** for managing a DevOps project.  
It contains all steps performed, from initializing the repo to tagging a release.  

---

## 📌 Objective
- Manage a DevOps project using Git version control.  
- Practice branching, commits, pull requests, tags, and documentation.  

---

## 🛠️ Tools Used
- **Git** – Version control system  
- **GitHub** – Remote repository hosting  

---

# 📝 Step-by-Step Execution  

## 1️⃣ Repository Initialization
1. Created project folder:  
   ```bash
   mkdir devops-git-project && cd devops-git-project
````

2. Initialized Git:

   ```bash
   git init
   ```
3. Created initial files:

   ```bash
   echo "# DevOps Git Project" > README.md
   echo "*.log" > .gitignore
   mkdir docs
   echo "## Task Documentation" > docs/TASKS.md
   ```
4. Added files to staging:

   ```bash
   git add .
   ```
5. Committed changes:

   ```bash
   git commit -m "Initial commit: project setup with README, .gitignore, docs"
   ```
6. Added remote GitHub repo:

   ```bash
   git remote add origin https://github.com/<your-username>/devops-git-project.git
   ```
7. Pushed code to **main** branch:

   ```bash
   git branch -M main
   git push -u origin main
   ```

---

## 2️⃣ Branching

1. Created **dev** branch for integration:

   ```bash
   git checkout -b dev
   git push -u origin dev
   ```
2. Created **feature branch** for development:

   ```bash
   git checkout -b feature-setup
   git push -u origin feature-setup
   ```

---

## 3️⃣ Making Changes

1. Edited `README.md` to add project details.
2. Staged & committed changes:

   ```bash
   git add README.md
   git commit -m "Updated README with project overview and objectives"
   git push origin feature-setup
   ```

---

## 4️⃣ Pull Requests & Merging

1. Opened Pull Request (PR) from `feature-setup` → `dev`.
2. Reviewed & merged changes into `dev`.
3. Later, merged `dev` → `main` for production-ready code.

---

## 5️⃣ Git Tags

1. After stable release, created version tag:

   ```bash
   git checkout main
   git tag -a v1.0 -m "First stable release"
   git push origin v1.0
   ```

---

## 6️⃣ Documentation

* **README.md** → Detailed project steps (this file).
* **docs/TASKS.md** → Summary of tasks in Markdown format.
* **.gitignore** → Prevents unnecessary files (like `.log`) from being committed.

---

# 📂 Repository Structure

```
devops-git-project/
│── docs/
│   └── TASKS.md      # Task documentation in markdown
│── .gitignore        # Git ignore rules
│── README.md         # Step-by-step execution log
```

---

# ✅ Deliverables

* GitHub repo with **main, dev, and feature** branches.
* Proper commit history with meaningful messages.
* Pull Requests used for merging.
* `.gitignore` file.
* **README.md** with full step-by-step execution.
* **docs/TASKS.md** with task documentation.
* Git tag `v1.0` for stable release.

---

# 📌 Outcome

This project successfully simulates a **real-world DevOps Git workflow** with:

* Clean branching strategy
* Proper version control practices
* Documentation for every action taken

```

