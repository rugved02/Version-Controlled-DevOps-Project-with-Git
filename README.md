# 🚀 DevOps Project with Git – Complete Guide

## 📌 Objective
This project demonstrates **Version Control Best Practices** using Git and GitHub.  

You will:  
- Initialize a repo locally and push to GitHub  
- Use `main`, `dev`, and `feature/*` branches  
- Follow PR-based workflow  
- Add `.gitignore`, tags, and documentation  
- Practice professional commit messages  

---

## 🛠 Required Software
- [Git](https://git-scm.com/downloads) – Version control  
- [GitHub account](https://github.com/join) – Remote repository  
- [VS Code](https://code.visualstudio.com/) or any editor  
- *(Optional)* [GitHub CLI](https://cli.github.com/) – Manage PRs from terminal  

---

## 📂 Step 1 – Create GitHub Repository
1. Log in to GitHub → `+` → **New repository**  
2. Name: `DevOps-Project-with-Git`  
3. Visibility: Public or Private  
4. **Do not** add README or `.gitignore` (we’ll do this locally)  
5. Click **Create repository**  

---

## 📂 Step 2 – Local Setup
```bash
# Create local folder
mkdir DevOps-Project-with-Git && cd DevOps-Project-with-Git

# Initialize Git
git init
````

---

## 📂 Step 3 – Create `README.md`

```bash
echo "# DevOps Project with Git" > README.md
```

---

## 📂 Step 4 – Create `.gitignore`

```bash
touch .gitignore
# Add patterns to ignore (e.g., node_modules, .env)
```

---

## 📂 Step 5 – First Commit & Push

```bash
git add .
git commit -m "Initial commit: Added README and .gitignore"
git branch -M main
git remote add origin <repo-url>
git push -u origin main
```

---

## 📂 Step 6 – Create Branches

```bash
# Create dev branch
git checkout -b dev
git push -u origin dev

# Create a feature branch
git checkout -b feature/add-ci-docs
```

---

## 📂 Step 7 – Commit Changes

```bash
git add .
git commit -m "Add CI/CD documentation"
git push -u origin feature/add-ci-docs
```

---

## 📂 Step 8 – Open Pull Request

1. Go to GitHub repo
2. Click **Compare & pull request**
3. **Base:** `dev` | **Compare:** `feature/add-ci-docs`
4. Add title and description
5. Request review
6. Merge into `dev`

---

## 📂 Step 9 – Merge `dev` → `main`

1. Open PR from `dev` → `main`
2. Merge after testing

**Tag release:**

```bash
git tag -a v1.0 -m "First stable release"
git push origin v1.0
```

---

## 📂 Step 10 – Commit Message Guidelines

---

## ✅ Outcome

* Repo with clean commit history
* Proper branching workflow
* Documentation in Markdown
* Safe and maintainable Git project

```

This will render with nice icons, code blocks, and spacing — perfect for GitHub.  

If you want, I can also **add color-coded badges** (build, version, license) at the top for extra visual appeal. That would make your README stand out even more.
```
