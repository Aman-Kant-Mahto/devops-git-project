# 📘 Task Documentation

## 🔹 Task 4: Build a Version-Controlled DevOps Project with Git

This document captures the step-by-step execution of the Git & GitHub workflow.  

---

### 1️⃣ Repository Initialization
- Created a local directory `devops-git-project`.  
- Initialized Git: `git init`.  
- Added `.gitignore`, `README.md`, and `docs/TASKS.md`.  
- Connected remote GitHub repository.  
- First commit pushed to **main** branch.  

---

### 2️⃣ Branching
- Created `dev` branch for integration.  
- Created `feature-setup` branch for development.  
- Strategy followed:  
  - `main` → stable code.  
  - `dev` → collects all features.  
  - `feature/*` → temporary branches for specific tasks.  

---

### 3️⃣ Pull Requests
- Raised PR from `feature-setup` → `dev`.  
- Reviewed & merged changes.  
- Later merged `dev` → `main`.  

---

### 4️⃣ Commits
- Used meaningful commit messages (e.g., `Added README with project overview`).  
- Avoided large unstructured commits.  

---

### 5️⃣ Tags
- Tagged the first release as `v1.0`:  
  ```bash
  git tag -a v1.0 -m "First stable release"
  git push origin v1.0
