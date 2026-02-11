# GitHub Deployment Guide

## Quick Start - Deploy to GitHub Pages

### Step 1: Initialize Git Repository
```bash
cd d:\harsh_portfolio
git init
```

### Step 2: Add All Files
```bash
git add .
```

### Step 3: Commit Changes
```bash
git commit -m "Initial commit: Portfolio website"
```

### Step 4: Create GitHub Repository
1. Go to [GitHub](https://github.com)
2. Click the **+** icon → **New repository**
3. Name it: `harsh-portfolio` (or any name you prefer)
4. **DO NOT** initialize with README (we already have one)
5. Click **Create repository**

### Step 5: Connect and Push
Replace `[your-username]` with your GitHub username:
```bash
git remote add origin https://github.com/[your-username]/harsh-portfolio.git
git branch -M main
git push -u origin main
```

### Step 6: Enable GitHub Pages
1. Go to your repository on GitHub
2. Click **Settings**
3. Scroll to **Pages** (left sidebar)
4. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**
6. Wait 1-2 minutes for deployment

### Step 7: Access Your Live Site
Your portfolio will be live at:
```
https://[your-username].github.io/harsh-portfolio/
```

## Update README with Live URL

After deployment, update line 14 in README.md:
```markdown
Visit the live website: [https://[your-username].github.io/harsh-portfolio/](https://[your-username].github.io/harsh-portfolio/)
```

## Making Updates

After making changes to your portfolio:
```bash
git add .
git commit -m "Description of changes"
git push
```

GitHub Pages will automatically update in 1-2 minutes.

## Troubleshooting

### Profile Picture Not Showing
- Ensure `profile.jpg` is in the root directory
- Check that `index.html` references `src="profile.jpg"`
- Clear browser cache (Ctrl+Shift+R)

### Page Not Loading
- Wait 2-3 minutes after enabling Pages
- Check GitHub Actions tab for build status
- Ensure `index.html` is in the root directory

### Custom Domain (Optional)
1. Buy a domain (e.g., from Namecheap, GoDaddy)
2. In repository Settings → Pages → Custom domain
3. Enter your domain and save
4. Update DNS settings with your domain provider

## Files in Your Repository

- `index.html` - Main website file
- `profile.jpg` - Your profile picture
- `README.md` - Project documentation
- `.gitignore` - Files to exclude from Git

## Next Steps

1. ✅ Deploy to GitHub Pages
2. ✅ Share your portfolio URL
3. ✅ Add to LinkedIn profile
4. ✅ Include in resume
5. ✅ Share with recruiters

---

**Need Help?** Check [GitHub Pages Documentation](https://docs.github.com/en/pages)
