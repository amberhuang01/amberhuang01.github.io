# Quick Setup Guide

## 🚀 Get Your Website Live in 5 Minutes

### Step 1: Download Files
You have these files:
- `index.html` - Main website file
- `styles.css` - Styling
- `script.js` - Interactive features
- `README.md` - Full documentation
- `.gitignore` - Git configuration

### Step 2: Customize Content
1. Open `index.html` in a text editor
2. Replace ALL placeholder text:
   - Your name (appears multiple times)
   - Your title and institution
   - Your research description
   - Publications
   - Contact information
3. Update social media links in the sidebar
4. Add your profile photo as `profile.jpg` (recommended: 500x500px, square)

### Step 3: Deploy to GitHub

#### Option A: GitHub Web Interface (Easiest)
1. Create account at github.com
2. Create new repository named `yourusername.github.io`
3. Upload all files by drag-and-drop
4. Go to Settings → Pages
5. Select "main" branch as source
6. Done! Visit `yourusername.github.io`

#### Option B: Using Git (If you know Git)
```bash
# In your project folder
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/yourusername/yourusername.github.io.git
git push -u origin main
```

Then enable GitHub Pages in repository settings.

### Step 4: Test Locally (Optional)
Before deploying, you can test locally:

**Simple method:**
- Just double-click `index.html` to open in your browser

**Using Python:**
```bash
python3 -m http.server 8000
# Visit http://localhost:8000
```

**Using VS Code:**
- Install "Live Server" extension
- Right-click `index.html` → "Open with Live Server"

## 🎨 Quick Customizations

### Change Colors
Edit `styles.css`, lines 2-11:
```css
--primary-color: #2563eb;  /* Change this hex code */
```

Popular academic color schemes:
- Blue: `#2563eb` (default)
- Dark: `#1f2937`
- Green: `#059669`
- Purple: `#7c3aed`
- Red: `#dc2626`

### Add Your Photo
1. Name your photo `profile.jpg`
2. Put it in the same folder as `index.html`
3. Make sure it's square (same width and height)

### Update Publications
Find this section in `index.html` and duplicate the pattern:
```html
<div class="publication">
    <div class="pub-year">2024</div>
    <div class="pub-content">
        <p class="pub-title">Your Paper Title</p>
        <p class="pub-authors"><strong>Your Name</strong>, Others</p>
        <p class="pub-venue"><em>Journal Name</em></p>
        <div class="pub-links">
            <a href="#">PDF</a>
        </div>
    </div>
</div>
```

## 📱 What You Get

✅ Responsive design (works on phone, tablet, desktop)
✅ Smooth scrolling navigation
✅ Professional academic layout
✅ Easy to update and maintain
✅ Free hosting on GitHub Pages
✅ Custom domain support (optional)

## 🆘 Need Help?

**Website not loading?**
- Wait 2-3 minutes after first push to GitHub
- Check GitHub Pages is enabled in Settings
- Verify files are in root directory (not in a subfolder)

**Images not showing?**
- Check filename matches exactly (case-sensitive!)
- Make sure image is in same folder as `index.html`

**Want to change something else?**
- Check the full `README.md` for detailed instructions
- Most text is in `index.html`
- Colors and styling are in `styles.css`

## 🎯 Next Steps

After your site is live:
1. Add your CV as a PDF
2. Link your Google Scholar profile
3. Update regularly with new publications
4. Share your URL: `yourusername.github.io`

---

**Questions?** Read the full README.md for complete documentation!