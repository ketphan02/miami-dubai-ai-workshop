# Deploy to GitHub Pages

This guide will help you deploy the Miami Dubai AI Workshop landing page to GitHub Pages for free hosting.

## Prerequisites

- GitHub account
- Git installed on your computer

## Step-by-Step Deployment

### 1. Initialize Git Repository (if not already done)

```bash
cd ai-landing-page
git init
git add .
git commit -m "Initial commit: Miami Dubai AI Workshop landing page"
```

### 2. Create GitHub Repository

1. Go to [GitHub](https://github.com)
2. Click the "+" icon in the top right
3. Select "New repository"
4. Name it: `ai-landing-page` (or any name you prefer)
5. **Do NOT** initialize with README, .gitignore, or license (we already have these)
6. Click "Create repository"

### 3. Link and Push to GitHub

Replace `YOUR_USERNAME` with your GitHub username:

```bash
git remote add origin https://github.com/YOUR_USERNAME/ai-landing-page.git
git branch -M main
git push -u origin main
```

### 4. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" tab
3. Scroll down to "Pages" section (left sidebar)
4. Under "Source", select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click "Save"

### 5. Wait for Deployment

- GitHub will take 1-2 minutes to deploy
- Your site will be available at: `https://YOUR_USERNAME.github.io/ai-landing-page/`
- You'll see a green checkmark when it's live

## Project Structure for GitHub Pages

```
ai-landing-page/
├── index.html          # Main landing page (root)
├── script.js           # JavaScript file (root)
├── public/             # Original source files (backup)
│   ├── index.html
│   └── script.js
├── server.js           # Local development server (not used on GitHub Pages)
├── package.json        # Node.js config (not used on GitHub Pages)
├── .gitignore          # Git ignore rules
└── README.md           # Project documentation
```

## Updating the Site

After making changes:

```bash
# Edit index.html or script.js
git add .
git commit -m "Update landing page content"
git push origin main
```

GitHub Pages will automatically rebuild and deploy in 1-2 minutes.

## Custom Domain (Optional)

To use a custom domain like `workshop.yourdomain.com`:

1. Add a file named `CNAME` in the root:
   ```bash
   echo "workshop.yourdomain.com" > CNAME
   git add CNAME
   git commit -m "Add custom domain"
   git push origin main
   ```

2. In your domain registrar (Namecheap, GoDaddy, etc.):
   - Add a CNAME record: `workshop` → `YOUR_USERNAME.github.io`

3. Wait 10-30 minutes for DNS propagation

## Local Testing

Before deploying changes, test locally:

```bash
# Option 1: Use Node.js server
npm start

# Option 2: Use Python server
python3 -m http.server 3000

# Option 3: Use any static file server
```

Open `http://localhost:3000` in your browser.

## Troubleshooting

**Site not loading?**
- Check GitHub Pages settings are correct
- Wait 2-3 minutes for first deployment
- Clear browser cache
- Check repository is public (or enable Pages for private repos)

**Changes not showing?**
- Wait 1-2 minutes after push
- Hard refresh browser (Ctrl/Cmd + Shift + R)
- Check commit was successful: `git log`

**404 Error?**
- Ensure `index.html` is in the root directory
- Verify branch name is `main` (not `master`)
- Check Pages settings show the correct branch

## Cost

- **Free** for public repositories
- **Free** for private repositories (with GitHub Pro, Team, or Enterprise)
- Includes free SSL certificate (HTTPS)
- Unlimited bandwidth for reasonable use

## Support

For GitHub Pages issues:
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [GitHub Pages Status](https://www.githubstatus.com/)
