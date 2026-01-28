# GitHub Setup Guide

Follow these steps to upload your File Validator app to GitHub and create a shareable link.

## Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in to your account
2. Click the **"+"** button in the top right corner and select **"New repository"**
3. Fill in the repository details:
   - **Repository name**: `file-validator-demo` (or any name you prefer)
   - **Description**: "Web app for validating PDF, JPG, and TIFF files"
   - **Visibility**: Choose **Public** (so GitHub Pages can work)
   - **DO NOT** initialize with README, .gitignore, or license (we already have files)
4. Click **"Create repository"**

## Step 2: Push Your Code to GitHub

After creating the repository, GitHub will show you commands. Open your terminal in the `file-validator-demo` folder and run:

```bash
cd /path/to/file-validator-demo
git remote add origin https://github.com/YOUR-USERNAME/file-validator-demo.git
git push -u origin main
```

**Note**: Replace `YOUR-USERNAME` with your actual GitHub username.

If prompted for credentials:
- **Username**: Your GitHub username
- **Password**: Use a [Personal Access Token](https://github.com/settings/tokens) (not your GitHub password)

### Creating a Personal Access Token (if needed):
1. Go to GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
2. Click "Generate new token (classic)"
3. Give it a name like "file-validator-upload"
4. Select scope: **repo** (full control of private repositories)
5. Click "Generate token"
6. Copy the token and use it as your password when pushing

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **"Settings"** tab
3. Scroll down to **"Pages"** section in the left sidebar
4. Under **"Source"**, select:
   - Branch: **main**
   - Folder: **/ (root)**
5. Click **"Save"**
6. Wait 1-2 minutes for deployment

## Step 4: Get Your Shareable Link

After GitHub Pages is enabled, you'll see a message like:

**"Your site is published at https://YOUR-USERNAME.github.io/file-validator-demo/"**

This is the link you can share with your boss! 🎉

## Testing the App

Before sharing, test that:
1. The page loads correctly
2. You can search for a recurso code
3. You can upload a file
4. The validation works

## Troubleshooting

**Problem**: Page shows 404 error
- **Solution**: Wait a few more minutes, GitHub Pages can take up to 10 minutes to deploy

**Problem**: recursos_db.json fails to load
- **Solution**: Check that the file was pushed to GitHub (should be visible in your repository)

**Problem**: Git push asks for username/password repeatedly
- **Solution**: Use SSH instead or set up credential helper

## Alternative: Quick Upload via GitHub Web Interface

If you prefer not to use the command line:

1. Create a new repository on GitHub (as above)
2. Click **"uploading an existing file"**
3. Drag and drop all three files: `index.html`, `recursos_db.json`, and `README.md`
4. Click **"Commit changes"**
5. Then follow Step 3 to enable GitHub Pages

---

**Need Help?** The git repository is already initialized and committed. You just need to push it to GitHub!
