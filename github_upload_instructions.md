# How to Push This Repository to GitHub

## Step 1 — Create a new GitHub repository

1. Go to https://github.com/new
2. Name your repository (e.g., `solidworks-assembly`)
3. Set visibility (Public or Private)
4. **Do NOT** initialize with README, .gitignore, or license — we already have those
5. Click **Create repository**

---

## Step 2 — Initialize and push from your local machine

After downloading the files from Claude, open a terminal in the repository folder and run:

```bash
git init
git add .
git commit -m "Initial commit — SolidWorks assembly and parts"
git branch -M main
git remote add origin https://github.com/<your-username>/mechanical-drone-design.git
git push -u origin main
```

Replace `<your-username>` and `<repo-name>` with your actual GitHub username and repo name.

---

## Step 3 — Verify

Visit your GitHub repo page — you should see all folders and files:
```
assemblies/
parts/
docs/
.gitignore
CHANGELOG.md
README.md
```

---

## Notes on Large Files

SolidWorks files can be large. If any file exceeds **100 MB**, GitHub will reject the push.
In that case, use **Git Large File Storage (LFS)**:

```bash
# Install Git LFS
git lfs install

# Track SolidWorks binary formats
git lfs track "*.SLDPRT"
git lfs track "*.SLDASM"
git lfs track "*.SLDDRW"

# Stage the .gitattributes file LFS creates
git add .gitattributes
git add .
git commit -m "Add Git LFS tracking for SolidWorks files"
git push -u origin main
```

> Git LFS requires a GitHub account with LFS storage (free tier includes 1 GB).
