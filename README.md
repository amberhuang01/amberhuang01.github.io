# Academic Website

A clean, modern personal academic website template built from scratch with HTML, CSS, and JavaScript.

## Features

- ✨ Clean, professional design
- 📱 Fully responsive (mobile, tablet, desktop)
- 🎯 Smooth scrolling navigation
- 📚 Sections for About, Research, Publications, Teaching, and Contact
- 🎨 Easy to customize colors and content
- 🚀 Ready to deploy on GitHub Pages
- ♿ Accessible and SEO-friendly

## Quick Start

### 1. Customize Your Content

Edit `index.html` and replace the placeholder content:

- **Personal Information**: Update name, title, institution
- **Profile Image**: Replace `profile.jpg` with your photo
- **About Section**: Write your bio, research interests
- **Publications**: Add your papers with links
- **Teaching**: List your courses
- **Contact**: Update your contact information
- **Social Links**: Update URLs for Google Scholar, GitHub, LinkedIn

### 2. Customize Colors (Optional)

Edit the CSS variables in `styles.css` (lines 2-11):

```css
:root {
    --primary-color: #2563eb;  /* Main accent color */
    --text-primary: #1f2937;   /* Main text color */
    --text-secondary: #6b7280; /* Secondary text color */
    /* ... other colors ... */
}
```

### 3. Add Your Profile Photo

Add your profile photo as `profile.jpg` in the same directory, or update the image path in `index.html`:

```html
<img src="your-image-name.jpg" alt="Your Name" class="profile-img">
```

Recommended image specifications:
- Square aspect ratio (e.g., 500x500px)
- Professional quality
- File size: < 500KB

## Deploy to GitHub Pages

### Method 1: Simple GitHub Pages (Recommended)

1. **Create a GitHub repository**
   - Go to [GitHub](https://github.com) and create a new repository
   - Name it `username.github.io` (replace `username` with your GitHub username)
   - Make it public

2. **Upload your files**
   - Upload `index.html`, `styles.css`, `script.js`, and your profile image
   - You can drag and drop files directly on GitHub, or use Git:

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/username/username.github.io.git
git push -u origin main
```

3. **Enable GitHub Pages**
   - Go to repository Settings → Pages
   - Under "Source", select "main" branch
   - Click "Save"
   - Your site will be live at `https://username.github.io`

### Method 2: Custom Domain

If you want to use a custom domain (e.g., `yourname.com`):

1. Follow steps above to deploy to GitHub Pages
2. Buy a domain from a domain registrar
3. Add a `CNAME` file to your repository with your domain name
4. Configure DNS settings with your domain registrar:
   - Add A records pointing to GitHub's IPs:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - Or add a CNAME record pointing to `username.github.io`
5. In GitHub repository settings, add your custom domain

## File Structure

```
your-website/
├── index.html          # Main HTML file
├── styles.css          # All styling
├── script.js           # JavaScript for interactivity
├── profile.jpg         # Your profile photo
├── cv.pdf             # Your CV (optional)
├── README.md          # This file
└── CNAME              # Custom domain (optional)
```

## Customization Tips

### Adding Publications

Each publication follows this structure in `index.html`:

```html
<div class="publication">
    <div class="pub-year">2024</div>
    <div class="pub-content">
        <p class="pub-title">Your Paper Title</p>
        <p class="pub-authors"><strong>Your Name</strong>, Co-Authors</p>
        <p class="pub-venue"><em>Journal/Conference Name</em></p>
        <div class="pub-links">
            <a href="paper.pdf">PDF</a>
            <a href="https://doi.org/...">DOI</a>
            <a href="https://github.com/...">Code</a>
        </div>
    </div>
</div>
```

### Adding Courses

```html
<div class="course">
    <div class="course-header">
        <h4>COURSE 101: Course Name</h4>
        <span class="course-term">Fall 2024</span>
    </div>
    <p>Course description...</p>
    <a href="course-url" class="course-link">Course Website →</a>
</div>
```

### Changing Fonts

The site uses Inter font from Google Fonts. To change:

1. Visit [Google Fonts](https://fonts.google.com)
2. Select your preferred font
3. Replace the font link in `index.html` (line 8)
4. Update `font-family` in `styles.css` (line 16)

### Adding New Sections

To add a new section:

1. Add navigation link in sidebar:
```html
<li><a href="#newsection">New Section</a></li>
```

2. Add section content:
```html
<section id="newsection" class="section">
    <h2>New Section</h2>
    <p>Your content here...</p>
</section>
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## Tips for Academic Websites

1. **Keep it updated**: Regularly update your publications and teaching
2. **Add your CV**: Include a downloadable PDF version
3. **Use Google Scholar**: Link to your profile for citation metrics
4. **SEO**: Use descriptive titles and meta tags
5. **Analytics**: Consider adding Google Analytics to track visitors
6. **Accessibility**: Ensure all images have alt text
7. **Performance**: Optimize images (compress before uploading)

## Adding Google Analytics (Optional)

To track website visits, add before `</head>` in `index.html`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

Replace `G-XXXXXXXXXX` with your Google Analytics tracking ID.

## Maintenance

### Regular Updates
- Update publications as they're published
- Keep teaching information current
- Update your CV annually
- Check that all links work

### Git Workflow
```bash
# Make changes to your files
git add .
git commit -m "Update publications"
git push
```

Changes typically go live within 1-2 minutes.

## Troubleshooting

**Site not loading?**
- Check that files are in the root directory
- Verify GitHub Pages is enabled in Settings
- Wait a few minutes after pushing changes

**Images not showing?**
- Check file names match exactly (case-sensitive)
- Ensure images are in the same directory
- Use relative paths (e.g., `profile.jpg` not `/profile.jpg`)

**Styling looks wrong?**
- Clear browser cache (Ctrl+Shift+R or Cmd+Shift+R)
- Check that `styles.css` is in the same directory
- Verify the CSS link in HTML is correct

## License

Feel free to use this template for your own academic website. No attribution required, but appreciated!

## Credits

Inspired by clean, modern academic websites with a focus on readability and simplicity.

---

For questions or issues, please open an issue on GitHub or contact [your.email@university.edu]