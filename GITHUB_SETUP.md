# 🚀 Push to GitHub - Step by Step Guide

## Step 1: Create a GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in
2. Click the **+** icon in the top right corner
3. Select **New repository**
4. Fill in the details:
   - **Repository name**: `parkease` (or any name you prefer)
   - **Description**: "Smart Parking Management System"
   - **Visibility**: Choose Public or Private
   - **DO NOT** check "Initialize with README" (we already have files)
5. Click **Create repository**

## Step 2: Copy Your Repository URL

After creating the repository, GitHub will show you a URL like:
```
https://github.com/your-username/parkease.git
```
**Copy this URL** - you'll need it in the next step.

## Step 3: Push Your Code

Open terminal in your project directory and run these commands:

```bash
# Navigate to your project (if not already there)
cd /Users/tusharchopra/Downloads/parkease-main

# Add all files to git
git add .

# Commit the files
git commit -m "Initial commit: ParkEase project"

# Add your GitHub repository as remote (replace with your actual URL)
git remote add origin https://github.com/your-username/parkease.git

# Push to GitHub
git branch -M main
git push -u origin main
```

## Step 4: Authenticate

If prompted for authentication:
- **Username**: Your GitHub username
- **Password**: Use a **Personal Access Token** (not your GitHub password)
  - To create one: GitHub → Settings → Developer settings → Personal access tokens → Generate new token
  - Give it `repo` permissions
  - Copy and use it as the password

## ✅ Done!

Your code is now on GitHub! Visit your repository URL to see it.

---

## 🔄 For Future Updates

When you make changes and want to push updates:

```bash
git add .
git commit -m "Description of your changes"
git push
```

---

## 🆘 Troubleshooting

**"Repository not found"**
- Check that the repository URL is correct
- Make sure you have access to the repository

**"Authentication failed"**
- Use a Personal Access Token instead of password
- Make sure the token has `repo` permissions

**"Remote origin already exists"**
- Run: `git remote set-url origin https://github.com/your-username/parkease.git`

