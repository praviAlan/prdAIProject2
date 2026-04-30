# GitHub Setup & Deployment Guide

## Step 1: Initialize Git Repository

```bash
cd c:\Users\USER\Downloads\prdAI2
git init
git add .
git commit -m "Initial commit: p5.js Interactive Portfolio"
```

## Step 2: Create GitHub Repository

1. Go to [GitHub.com](https://github.com)
2. Click the "+" icon → "New repository"
3. Name it: `p5js-interactive-portfolio`
4. Add description: "Interactive portfolio showcasing p5.js creative coding projects"
5. Choose "Public" for visibility
6. Click "Create repository"

## Step 3: Push to GitHub

```bash
git remote add origin https://github.com/yourusername/p5js-interactive-portfolio.git
git branch -M main
git push -u origin main
```

Replace `yourusername` with your actual GitHub username.

## Step 4: Deploy to Vercel

### Option A: Via GitHub (Recommended)

1. Go to [Vercel.com](https://vercel.com)
2. Click "Sign up" or "Log in"
3. Choose "Continue with GitHub"
4. Authorize Vercel to access your repositories
5. Click "Add New" → "Project"
6. Select `p5js-interactive-portfolio`
7. Click "Import"
8. Framework: Next.js (auto-detected)
9. Click "Deploy"
10. Wait ~2 minutes for deployment
11. Get your live URL (e.g., `https://p5js-portfolio.vercel.app`)

### Option B: Via Vercel CLI

```bash
npm i -g vercel
vercel
```

Follow the prompts to deploy.

## Step 5: Custom Domain (Optional)

In Vercel dashboard:
1. Go to your project settings
2. Click "Domains"
3. Add your custom domain
4. Update DNS records as shown

## Step 6: Update Project Files

Before deploying, personalize these files:

### In `app/page.js` - Update social links:
```javascript
<a href="https://github.com/yourusername" target="_blank">GitHub</a>
```

### In `app/about/page.js` - Update email:
```javascript
<a href="mailto:your.email@example.com">Email</a>
```

### In `README.md` - Update contact info:
- Your email
- GitHub URL
- LinkedIn URL

## Step 7: Update Project Info

Edit project data in `app/projects/[id]/page.js`:
```javascript
{
  id: 1,
  title: 'Your Project Title',
  description: '...',
  concept: '...',
  controls: '...',
  tools: ['p5.js', 'JavaScript'],
  github: 'https://github.com/yourusername/project-repo',
}
```

## Continuous Deployment

Every time you push to GitHub, Vercel will:
1. Automatically build your project
2. Run tests (if configured)
3. Deploy to production
4. Send you a deployment notification

## Environment Setup

1. **Local Development**
   ```bash
   npm run dev
   # Visit http://localhost:3000
   ```

2. **Build & Test**
   ```bash
   npm run build
   npm start
   ```

3. **Deploy**
   ```bash
   git push origin main  # Vercel auto-deploys
   ```

## Troubleshooting

### Build fails on Vercel?
- Check `.vercelignore` and `.gitignore`
- Ensure `package.json` has all dependencies
- Check logs in Vercel dashboard

### Preview URL not showing?
- Wait a few moments for build to complete
- Refresh Vercel dashboard
- Check build logs for errors

### Changes not live?
- Push to `main` branch (not other branches)
- Check that deployment completed successfully
- Clear browser cache (Ctrl+Shift+Delete)

## Repository Commands

```bash
# Check git status
git status

# Add specific files
git add app/page.js

# Add all changes
git add .

# Commit
git commit -m "Describe your changes"

# Push to GitHub
git push origin main

# Pull latest changes
git pull origin main

# View commit history
git log --oneline
```

## Success Checklist

- [ ] Git repository created locally
- [ ] Remote GitHub repository created
- [ ] Pushed code to GitHub
- [ ] Connected GitHub to Vercel
- [ ] Deployed successfully to Vercel
- [ ] Portfolio accessible at live URL
- [ ] All projects load and interact correctly
- [ ] Responsive on mobile devices
- [ ] Social links point to your accounts
- [ ] Email link is your real email

## Next Steps

1. Customize the 11 sketches with your actual p5.js code
2. Add project screenshots/thumbnails
3. Update About section with your bio
4. Add GitHub links to actual project repositories
5. Test on mobile and different browsers
6. Share with recruiters!

---

**Your portfolio is now ready to showcase your creative coding!** 🚀
