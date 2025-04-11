# DevOps Version-Controlled Project

## 🏁 Objective
Manage a DevOps project using Git best practices like branching, pull requests, tagging, and documentation.

## 🛠️ Tools Used
- Git
- GitHub

## 📁 Branch Structure
- `main`: Production-ready code
- `dev`: Development integration
- `feature`: Feature development

## 📌 Git Workflow Followed
- Created and initialized Git repo
- Created `dev` and `feature` branches
- Made changes in `feature`, merged into `dev`, then into `main` via Pull Requests
- Added `.gitignore` for ignoring unwanted files
- Created tag `v1.0` to mark project version

## 📄 Files
- `README.md` – Documentation
- `index.js` – Sample Node.js file
- `.gitignore` – Ignore list

## ✅ Outcome
Learned version control workflows using Git and GitHub like:
- Branching
- Commit history
- Pull requests
- Tags
- Markdown documentation

---

## 🔁 Git Branching Strategy

- **main** – Stable production branch  
- **dev** – Active development branch  
- **feature** – For new features or changes

---

## 📸 Screenshots

> Please refer to the screenshots folder or markdown for all Git commands and operations done during this task.

---

## 🧾 Commands Used

```bash
# Step 1: Initialize the repository
git init

# Step 2: Add GitHub remote
git remote add origin https://github.com/shireesha-banothu/git-devops-project.git

# Step 3: Create sample files
echo "# DevOps Project" > README.md
echo "console.log('Hello from Node.js');" > index.js

# Step 4: Stage and commit files
git add .
git commit -m "Initial commit with README and index.js"
git branch -M main
git push -u origin main

# Step 5: Create dev and feature branches
git checkout -b dev
git push origin dev
git checkout -b feature
git push origin feature

# Step 6: Add changes and push from feature
git add .
git commit -m "Added sample feature code"
git push origin feature

# Step 7: Create Pull Requests (on GitHub)
# - feature ➡️ dev (merge)
# - dev ➡️ main (merge)

# Step 8: Pull updates if needed
git checkout main
git pull origin main

# Step 9: Add .gitignore
echo "node_modules/" >> .gitignore
echo "*.log" >> .gitignore
git add .gitignore
git commit -m "Add .gitignore"
git push origin main

# Step 10: Create a version tag
git tag v1.0 -m "First release"
git push origin v1.0


