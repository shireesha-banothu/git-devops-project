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
# Step 1: Initialize repo and connect to GitHub
git init
git remote add origin https://github.com/shireesha-banothu/git-devops-project.git

# Step 2: Add sample files
echo "# DevOps Project" > README.md
echo "console.log('Hello from Node.js');" > index.js
git add .
git commit -m "Initial commit with README and index.js"
git branch -M main
git push -u origin main

# Step 3: Create & switch to dev branch
git checkout -b dev
git push origin dev

# Step 4: Create & switch to feature branch
git checkout -b feature
git push origin feature

# Step 5: Make changes in feature branch
# (e.g., edit README or index.js)
git add .
git commit -m "Added sample feature code"
git push origin feature

# Step 6: Create PR: feature ➡️ dev (on GitHub) and merge
# Step 7: Create PR: dev ➡️ main (on GitHub) and merge

# Step 8: Pull latest changes if needed
git checkout main
git pull origin main

# Step 9: Add .gitignore
echo "node_modules/" >> .gitignore
echo "*.log" >> .gitignore
git add .gitignore
git commit -m "Add .gitignore"
git push origin main

# Step 10: Add a tag
git tag v1.0 -m "First release"
git push origin v1.0

