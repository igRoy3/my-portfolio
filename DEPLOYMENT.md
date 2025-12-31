# 🚀 Deployment Guide - GitHub Pages

This guide will help you deploy your portfolio website to GitHub Pages.

## Prerequisites
- Git installed on your computer
- A GitHub account

## Step-by-Step Deployment

### 1. Initialize Git Repository (if not already done)
```bash
cd /Users/priyangshuroy/Documents/GitHub/my-portfolio
git init
```

### 2. Add all files to Git
```bash
git add .
```

### 3. Commit your changes
```bash
git commit -m "Initial commit: Portfolio website"
```

### 4. Create a GitHub Repository
1. Go to [GitHub](https://github.com)
2. Click the "+" icon in the top right
3. Select "New repository"
4. Name it: `my-portfolio` (or any name you prefer)
5. **Do NOT initialize with README** (since you already have files)
6. Click "Create repository"

### 5. Link your local repository to GitHub
Replace `yourusername` with your actual GitHub username:
```bash
git remote add origin https://github.com/yourusername/my-portfolio.git
git branch -M main
git push -u origin main
```

### 6. Enable GitHub Pages
1. Go to your repository on GitHub
2. Click on **Settings** (tab at the top)
3. Scroll down to **Pages** section (in the left sidebar)
4. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**

### 7. Access Your Live Website
After a few minutes, your site will be live at:
```
https://yourusername.github.io/my-portfolio/
```

Replace `yourusername` with your GitHub username.

---

## Making Updates

When you want to update your portfolio:

1. **Make your changes** to the files
2. **Save** all files
3. **Commit and push**:
```bash
git add .
git commit -m "Update portfolio content"
git push origin main
```

GitHub Pages will automatically rebuild and deploy your site within a few minutes.

---

## Updating Your Content

### Update Personal Information
Open `index.html` and update:
- Your name (already set to "Priyangshu Roy")
- Contact email, GitHub, LinkedIn links (search for `yourname@email.com`, `yourusername`)

### Add Your Projects
In `index.html`, find the Projects section and:
1. Update project titles and descriptions
2. Change placeholder links to your actual GitHub repos and live demos
3. Add more project cards by copying the existing structure

### Update Skills
Modify the skills section to add/remove technologies you work with.

---

## Custom Domain (Optional)

If you want to use a custom domain (e.g., `www.yourname.com`):

1. Buy a domain from a provider (Namecheap, GoDaddy, etc.)
2. Create a file named `CNAME` in your repository root
3. Add your custom domain to the file:
   ```
   www.yourname.com
   ```
4. Configure DNS settings with your domain provider:
   - Type: `CNAME`
   - Name: `www`
   - Value: `yourusername.github.io`

---

## Troubleshooting

### Site not showing up?
- Wait 5-10 minutes after enabling GitHub Pages
- Check that you selected the correct branch (`main`)
- Make sure `index.html` is in the root directory

### Styles not loading?
- Check that file paths are correct (they should be relative: `css/styles.css`, not `/css/styles.css`)
- Clear your browser cache (Cmd+Shift+R on Mac, Ctrl+Shift+R on Windows)

### Need help?
- Check GitHub Pages documentation: https://docs.github.com/en/pages
- Verify all files are committed and pushed: `git status`

---

## 🎉 Congratulations!

Your portfolio is now live on the internet! Share it with potential employers, clients, and your network.

**Next Steps:**
1. Update placeholder content with your actual information
2. Add real project descriptions and links
3. Test on mobile devices
4. Share your portfolio URL on LinkedIn and your resume
