# 🚀 GitHub Pages Setup Guide

Follow these steps to deploy your Polymarket Trader Tracker to GitHub Pages.

## Step 1: Create GitHub Account
1. Go to [github.com](https://github.com)
2. Click "Sign up"
3. Choose a username (this will be in your URL)
4. Verify email

## Step 2: Create Repository
1. Click the **"+"** icon (top right) → "New repository"
2. Repository name: `polymarket-tracker`
3. Description: "Real-time Polymarket trader alerts"
4. Make it **Public**
5. ✅ Check "Add a README file" (optional - we have our own)
6. Click **"Create repository"**

## Step 3: Upload Files

### Option A: Web Upload (Easiest)
1. Click **"uploading an existing file"** or **"Add file" → "Upload files"**
2. Drag and drop ALL these files:
   - `index.html`
   - `notifications.html`
   - `README.md`
   - `GUIDE.md`
   - `LICENSE`
   - `.gitignore`
3. Scroll down, click **"Commit changes"**

### Option B: Git Command Line
```bash
cd /path/to/polymarket-github
git init
git add .
git commit -m "Initial commit: Polymarket Trader Tracker"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/polymarket-tracker.git
git push -u origin main
```

## Step 4: Enable GitHub Pages
1. In your repository, click **"Settings"** tab
2. Scroll down to **"Pages"** in left sidebar
3. Under "Source":
   - Select **"main"** branch
   - Folder: **"/ (root)"**
4. Click **"Save"**
5. Wait 1-2 minutes for deployment

## Step 5: Access Your Live App
Your app will be live at:
```
https://YOUR_USERNAME.github.io/polymarket-tracker/
```

For example:
- Username: `cryptotrader123`
- URL: `https://cryptotrader123.github.io/polymarket-tracker/`

The `index.html` will auto-redirect to `notifications.html`

## Step 6: Update README
1. Edit `README.md` in GitHub
2. Replace `yourusername` with your actual GitHub username in the demo links
3. Commit changes

## 🎉 You're Done!

Your app is now:
- ✅ Live on the internet
- ✅ Accessible from any device
- ✅ No CORS issues
- ✅ Free hosting forever
- ✅ Shareable with anyone

## 📱 Accessing on Mobile
1. Open Safari/Chrome on your phone
2. Go to your GitHub Pages URL
3. Tap "Share" → "Add to Home Screen"
4. Now it's an app icon on your phone!

## 🔄 Making Updates
Whenever you want to update the app:
1. Edit files in GitHub (click file → pencil icon)
2. Or upload new versions
3. Changes go live in ~1 minute

## 🌟 Next Steps
- Add to browser bookmarks
- Share link with trading community
- Star your own repo
- Customize the code however you want!

## ⚠️ Important Notes
- Don't share your Discord webhook URL publicly (keep it in app settings only)
- Your app will always be at the same URL
- Free tier has no usage limits for static sites
- Can handle thousands of users

## 🆘 Troubleshooting

**"404 - Page not found"?**
- Wait 2-3 minutes after enabling Pages
- Check Settings → Pages shows green checkmark
- Verify URL is correct format

**Changes not showing?**
- Hard refresh: Ctrl+Shift+R (Windows) or Cmd+Shift+R (Mac)
- Clear browser cache
- Wait 1-2 minutes after commit

**Still having issues?**
- Check repository is Public (not Private)
- Verify branch is named "main" not "master"
- Make sure Pages is set to "main" branch

---

**That's it! You now have a professional, live web app on GitHub Pages for free! 🚀**
