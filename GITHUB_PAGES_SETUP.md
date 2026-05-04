# GitHub Pages Deployment Guide

Follow these steps to deploy your Southeast Asia Travel Tracker to GitHub Pages.

## Prerequisites

- GitHub account ([create one here](https://github.com/join) if needed)
- Git installed on your computer (already detected on your system)

---

## Step 1: Create a New GitHub Repository

1. Go to [github.com](https://github.com) and sign in
2. Click the **"+"** icon in the top-right corner
3. Select **"New repository"**
4. Fill in the details:
   - **Repository name**: `southeast-asia-travel-tracker` (or your preferred name)
   - **Description**: "Interactive travel tracker for Singapore & Thailand 2026"
   - **Public** or **Private**: Choose based on your preference
   - ❌ **DO NOT** check "Add a README file" (we already have one)
5. Click **"Create repository"**

---

## Step 2: Initialize Git in Your Project

Open Command Prompt or PowerShell and run these commands:

```bash
# Navigate to your project directory
cd "C:\Users\maxjwang\Documents\Projects\2026 Southeast Asia Travel Tracker"

# Initialize git repository
git init

# Add all files to git
git add .

# Commit the files
git commit -m "Initial commit: Southeast Asia Travel Tracker with mobile optimizations"
```

---

## Step 3: Connect to GitHub and Push

**Replace `YOUR-USERNAME` and `YOUR-REPO-NAME` with your actual GitHub username and repository name:**

```bash
# Add GitHub as remote origin
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git

# Rename default branch to main (if needed)
git branch -M main

# Push to GitHub
git push -u origin main
```

**Example:**
```bash
git remote add origin https://github.com/maxjwang/southeast-asia-travel-tracker.git
git branch -M main
git push -u origin main
```

You'll be prompted to sign in to GitHub. Use your GitHub credentials.

---

## Step 4: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **"Settings"** tab (top right of repository page)
3. Scroll down to **"Pages"** in the left sidebar
4. Under **"Source"**, select:
   - **Branch**: `main`
   - **Folder**: `/ (root)`
5. Click **"Save"**

GitHub will now build and deploy your site. This takes 1-2 minutes.

---

## Step 5: Access Your Live Site

Once deployed, your site will be available at:

```
https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/
```

**Example:**
```
https://maxjwang.github.io/southeast-asia-travel-tracker/
```

Since your main file is `index.html`, it will automatically load at the root URL!

---

## Making Future Updates

Whenever you update your website:

```bash
# Navigate to project directory
cd "C:\Users\maxjwang\Documents\Projects\2026 Southeast Asia Travel Tracker"

# Add changed files
git add .

# Commit with a descriptive message
git commit -m "Updated flight times" # or whatever you changed

# Push to GitHub
git push
```

GitHub Pages will automatically rebuild and deploy your site (takes 1-2 minutes).

---

## Troubleshooting

### Authentication Issues

If you have trouble pushing, you may need to use a Personal Access Token:

1. Go to GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
2. Click "Generate new token (classic)"
3. Give it a name: "Travel Tracker Deployment"
4. Check the `repo` scope
5. Click "Generate token"
6. Copy the token (you won't see it again!)
7. Use this token as your password when pushing

### Site Not Updating

- Wait 2-3 minutes for GitHub Pages to rebuild
- Hard refresh your browser (Ctrl + Shift + R or Cmd + Shift + R)
- Check the "Actions" tab in your repository to see deployment status

### Wrong URL or 404 Error

- Make sure your file is named `index.html` (not `travel-tracker.html`)
- Check that GitHub Pages is enabled in repository Settings → Pages
- Verify the branch is set to `main` and folder is `/ (root)`

---

## Custom Domain (Optional)

If you want to use your own domain (e.g., `travel.maxwang.com`):

1. Buy a domain from a registrar (Namecheap, Google Domains, etc.)
2. In your repository Settings → Pages → Custom domain
3. Enter your domain name
4. Add DNS records from your domain registrar pointing to GitHub Pages
5. See [GitHub's custom domain guide](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)

---

## Sharing Your Site

Once deployed, share your URL with family and friends:

```
https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/
```

They can:
- View all your flight details
- Track live clocks from different time zones
- See the interactive map with flight paths
- Access it perfectly on mobile devices!

---

## Security Note

Since this site will be publicly accessible:
- Don't include sensitive personal information (passport numbers, full addresses, etc.)
- The information currently included (hotel names, flight numbers) is generally safe to share
- You can make the repository private, but the GitHub Pages site will still be publicly accessible (unless you have GitHub Pro for private Pages)

---

## Need Help?

- GitHub Pages documentation: https://pages.github.com/
- Git documentation: https://git-scm.com/doc
- GitHub support: https://support.github.com/
