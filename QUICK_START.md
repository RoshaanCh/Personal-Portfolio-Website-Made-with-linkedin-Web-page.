# Quick Start Guide - Portfolio Website

Get your professional portfolio online in 5 minutes!

## 🚀 Quick Start (5 Minutes)

### Step 1: Open Your Portfolio (1 minute)
1. Double-click `index.html` file
2. Your portfolio opens in your default browser
3. Explore the website!

### Step 2: Test the Features (2 minutes)
- ✅ Click navigation links (smooth scrolling)
- ✅ Try the theme toggle (dark/light mode)
- ✅ Scroll through all sections
- ✅ Click "View Full" on certificates
- ✅ Test on mobile (open DevTools: F12)

### Step 3: Customize with Your Info (2 minutes)
1. Open `index.html` with a text editor
2. Find and replace:
   - "Muhammad Roshaan" → Your Name
   - "Computer Science Student | Hackathon Enthusiast | Vibe Coder" → Your Title
   - Email addresses and social links

### Step 4: Deploy (Optional, 5 minutes)
See "Deployment" section below

---

## 📝 Essential Customizations

### Edit Personal Info
Open `index.html` and find these sections:

**Hero Section (Line ~70)**
```html
<h1 class="hero-title">Your Name Here</h1>
<p class="hero-subtitle">Your Title | Your Interest | Your Vibe</p>
<p class="hero-tagline">Your motivational tagline</p>
```

**Education (Line ~150)**
Replace example education with yours

**Achievements (Line ~250)**
Update your clubs and societies

**Contact (Line ~350)**
Update your email and social links

### Easiest Way to Edit
1. Right-click `index.html`
2. Select "Open with" → Notepad or VSCode
3. Find text you want to change (Ctrl+F)
4. Replace it
5. Save (Ctrl+S)
6. Refresh browser to see changes

---

## 🎨 Customization Options

### Change Colors (Advanced)
Edit `assets/css/styles.css`, find `:root` section (top of file):

```css
:root {
    --primary-color: #0a84ff;      /* Main blue - change this */
    --secondary-color: #00d98e;    /* Green accent */
    --accent-color: #ff6b6b;       /* Red accent */
}
```

**Color Ideas**:
- Tech: `#0066ff`, `#00d98e`, `#ff6b6b`
- Professional: `#1a1a1a`, `#0066cc`, `#cccccc`
- Creative: `#ff006e`, `#00f5ff`, `#ffd700`

### Add Your Images
See `IMAGES_GUIDE.md` for detailed instructions

### Change Social Links
Find the contact section, update these:

```html
<a href="https://linkedin.com/in/YOUR-USERNAME/" target="_blank">
    <i class="fab fa-linkedin"></i>
    <span>LinkedIn</span>
</a>
```

---

## 🌐 Deployment (Get It Online)

### Option 1: GitHub Pages (Recommended - Free)

**Step 1**: Create GitHub Account
- Go to github.com
- Sign up (free)

**Step 2**: Create Repository
- Click "+" → New repository
- Name it: `portfolio`
- Click "Create"

**Step 3**: Upload Files
- Click "Add file" → "Upload files"
- Drag and drop entire `website` folder
- Commit changes

**Step 4**: Enable GitHub Pages
- Go to repository Settings
- Find "Pages" section
- Select "main" branch
- Save

**Step 5**: Your Site is Live!
- URL: `https://yourusername.github.io/portfolio`
- Share with recruiters!

### Option 2: Netlify (Easiest - Free)

**Step 1**: Go to netlify.com
**Step 2**: Click "Deploy manually"
**Step 3**: Drag and drop `website` folder
**Step 4**: Your site goes live instantly!

### Option 3: Vercel (Fast - Free)

1. Go to vercel.com
2. Click "Add New Project"
3. Upload folder
4. Done! 🎉

### Option 4: Traditional Hosting

If you have a web host:
1. Upload `website` folder contents via FTP
2. Set index.html as default page
3. Visit your domain

---

## 📱 Test on Different Devices

### Browser Testing
1. Open index.html in browser
2. Press F12 (Developer Tools)
3. Click mobile icon (top-left)
4. Test at different widths:
   - Mobile: 375px
   - Tablet: 768px
   - Desktop: 1200px+

### Real Device Testing
1. Note your computer's IP address
2. On phone, visit: `http://YOUR-IP:5000`
3. (You may need to use a local server)

---

## 🔧 Common Edits

### Change Hero Background
Edit `styles.css`, find `.hero` section:
```css
.hero {
    background: linear-gradient(135deg, rgba(10, 132, 255, 0.1) 0%, rgba(0, 217, 142, 0.05) 100%);
}
```

### Change Fonts
At top of `styles.css`:
```css
--font-primary: 'Your Font Name', sans-serif;
```

### Add More Certificate Cards
Copy this block and paste 4 times:
```html
<div class="certificate-card">
    <!-- Copy entire card here -->
</div>
```

### Adjust Spacing
Modify these in styles.css:
```css
--spacing-lg: 2rem;    /* Larger = more space */
--spacing-md: 1.5rem;
```

---

## ✨ Professional Tips

### Make It Stand Out
1. **Use High-Quality Images** - Professional looking certificates
2. **Clear Writing** - Concise descriptions
3. **Real Information** - Actual achievements (recruiters can tell)
4. **Keep Updated** - Add new certificates as you earn them
5. **Mobile First** - Test on phone first!

### For Recruiters
1. Link from LinkedIn profile
2. Include in job applications
3. Share in email signature
4. Point to in cover letters
5. Update frequently

---

## 🐛 Troubleshooting

### Website looks broken
- Clear browser cache: Ctrl+Shift+Delete
- Hard refresh: Ctrl+F5
- Try different browser

### Images not showing
- Check file path is correct
- Verify file exists in folder
- Check file name spelling (case-sensitive)

### Contact form not working
- It's for demo only (see README.md for integration)
- Success message still shows locally
- Need backend service for real emails

### Theme toggle not working
- Check browser has JavaScript enabled
- Clear localStorage: Open DevTools → Application → Storage → Clear All
- Hard refresh page

### Mobile menu not opening
- Refresh page
- Clear cache
- Try different mobile browser

---

## 📚 File Reference

### Main Files You'll Edit
- `index.html` - Your content (text, links, sections)
- `assets/css/styles.css` - Colors, fonts, spacing (advanced)
- `assets/images/` - Your certificate images

### Don't Edit (Unless Advanced)
- `assets/js/script.js` - Interactive features
- Files in `_files` folder

---

## 🎯 Checklist Before Sharing

- [ ] Updated your name everywhere
- [ ] Changed social media links
- [ ] Added real education info
- [ ] Changed color scheme (optional)
- [ ] Tested on mobile
- [ ] Tested contact form
- [ ] Tested theme toggle
- [ ] Tested all navigation links
- [ ] Images display correctly
- [ ] No broken links
- [ ] Deploy to free hosting (GitHub Pages/Netlify)

---

## 🎓 Next Steps

### After Basic Setup
1. **Add Your Images** - See `IMAGES_GUIDE.md`
2. **Advanced Styling** - Edit `styles.css` for custom colors
3. **Integration** - Set up real contact form (see README.md)
4. **SEO** - Add meta tags for search engines
5. **Analytics** - Track visitors (Google Analytics)

### Learning Resources
- HTML/CSS: w3schools.com
- JavaScript: javascript.info
- Web Design: dribbble.com
- Color Schemes: coolors.co

---

## 💡 Pro Tips

### Keyboard Shortcuts
- Alt+H: Jump to Home section
- Alt+C: Jump to Contact section
- Esc: Close lightbox

### Performance
- Compress images before uploading
- Minify CSS/JS (advanced)
- Use CDN for libraries

### SEO
- Update page title in HTML head
- Add meta descriptions
- Use descriptive alt text for images
- Create sitemap.xml

---

## 🆘 Get Help

1. Check README.md (comprehensive guide)
2. Check IMAGES_GUIDE.md (for image help)
3. Review code comments in files
4. Search error messages online
5. Test in different browsers

---

## 🎉 Congratulations!

Your professional portfolio is ready! 

**Next**: Customize it, deploy it, and share it with the world! 🚀

---

**Questions?** See the detailed guides:
- `README.md` - Full documentation
- `IMAGES_GUIDE.md` - Image customization

**Have fun building your online presence!** 💻✨
