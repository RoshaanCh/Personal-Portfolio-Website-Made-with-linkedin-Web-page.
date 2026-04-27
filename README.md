# Professional Portfolio Website

## Overview
A modern, responsive, and professional portfolio website built with HTML5, CSS3, and vanilla JavaScript. Designed specifically for Computer Science students, developers, and professionals to showcase education, certificates, achievements, and skills.

## Features

### Core Features
- **Responsive Design** - Mobile, tablet, and desktop optimized
- **Dark/Light Mode** - Theme toggle with persistent storage
- **Smooth Animations** - Fade-in, slide, and hover effects
- **Modern UI/UX** - Professional gradient design with smooth transitions
- **Mobile Menu** - Hamburger navigation for small screens
- **Sticky Navbar** - Always accessible navigation with active section highlighting

### Sections
1. **Hero Section** - Eye-catching landing section with call-to-action buttons
2. **About Section** - Personal introduction with skills and statistics
3. **Education Timeline** - Educational background displayed in timeline format
4. **Certificates Gallery** - Professional certificates with lightbox functionality
5. **Achievements Section** - Clubs, societies, and hackathon participation
6. **Contact Section** - Contact form and social media links
7. **Footer** - Copyright and attribution

## Project Structure

```
website/
├── index.html                 # Main HTML file
├── assets/
│   ├── css/
│   │   └── styles.css        # All styling and responsive design
│   ├── js/
│   │   └── script.js         # Interactive functionality
│   └── images/
│       └── cert-placeholder.jpg  # Placeholder certificate image
└── README.md                  # This file
```

## Customization Guide

### 1. **Personal Information**
Edit `index.html` to add your personal details:

```html
<!-- Hero Section -->
<h1 class="hero-title">Your Name</h1>
<p class="hero-subtitle">Your Title | Interests | Skills</p>
<p class="hero-tagline">Your tagline here</p>
```

### 2. **Education Details**
Update the education timeline with your institutions:

```html
<div class="timeline-item">
    <div class="timeline-marker"></div>
    <div class="timeline-content">
        <h3 class="timeline-title">Your Degree/Program</h3>
        <p class="timeline-subtitle">Institution Name</p>
        <p class="timeline-duration">Start - End</p>
        <p class="timeline-description">Your description here</p>
    </div>
</div>
```

### 3. **Adding Certificate Images**
1. Place your certificate images in `assets/images/` folder
2. Update the image paths in the HTML:

```html
<img src="assets/images/your-certificate.jpg" alt="Certificate Name">
```

3. Update the certificate information:

```html
<div class="certificate-card">
    <div class="certificate-image-wrapper">
        <img src="assets/images/your-cert.jpg" alt="Your Certificate">
        <div class="certificate-overlay">
            <button class="btn-view" data-image="assets/images/your-cert.jpg">
                <i class="fas fa-expand"></i> View Full
            </button>
        </div>
    </div>
    <div class="certificate-info">
        <h3>Certificate Name</h3>
        <p class="certificate-issuer">Issuing Authority</p>
        <p class="certificate-date">Issued: 2024</p>
    </div>
</div>
```

### 4. **Update Achievement Cards**
Customize the achievements section with your memberships:

```html
<div class="achievement-card">
    <div class="achievement-icon">
        <i class="fas fa-your-icon"></i>  <!-- Change icon -->
    </div>
    <h3>Your Achievement Title</h3>
    <p class="achievement-role">Your Role</p>
    <p class="achievement-description">
        Your description here
    </p>
    <div class="achievement-tags">
        <span class="tag">Tag1</span>
        <span class="tag">Tag2</span>
    </div>
</div>
```

### 5. **Update Contact Information**
Change contact details in the HTML:

```html
<!-- Email -->
<p><strong>Email:</strong> your-email@example.com</p>

<!-- Social Links -->
<a href="https://linkedin.com/in/your-profile" target="_blank">
    <i class="fab fa-linkedin"></i> LinkedIn
</a>
```

### 6. **Color Customization**
Edit the CSS variables in `assets/css/styles.css`:

```css
:root {
    --primary-color: #0a84ff;      /* Main accent color */
    --secondary-color: #00d98e;    /* Secondary accent */
    --accent-color: #ff6b6b;       /* Tertiary accent */
    --dark-bg: #0f1419;            /* Dark theme background */
    --card-bg: #1a1f26;            /* Card background */
}
```

## Icons
This portfolio uses Font Awesome 6.4.0 icons. Common icon classes:

- `fa-linkedin` - LinkedIn
- `fa-github` - GitHub
- `fa-twitter` - Twitter
- `fa-envelope` - Email
- `fa-trophy` - Trophy/Award
- `fa-star` - Star/Rating
- `fa-code` - Code
- `fa-lightbulb` - Idea/Innovation
- `fa-microphone` - Speaking/Debate
- `fa-network-wired` - Networking

Full icon list: https://fontawesome.com/icons

## Browser Support

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+
- Mobile browsers (iOS Safari, Chrome Mobile)

## Performance Tips

1. **Optimize Images**: Compress certificate images before uploading
   - Recommended size: 400x300px
   - Format: JPG or PNG
   - Max file size: 200KB per image

2. **Use WebP Format**: For better performance
   - Convert images to WebP format
   - Update image paths accordingly

3. **Lazy Loading**: Images load on demand for better performance

## JavaScript Features

### Smooth Scrolling
- Click navigation links for smooth scroll to section
- Automatic scroll-to-top button appears after scrolling

### Mobile Menu
- Hamburger menu for screens under 768px
- Auto-closes when a link is clicked
- Smooth animation

### Dark/Light Mode
- Toggle between dark and light themes
- Preference stored in localStorage
- Persists across page reloads

### Certificate Lightbox
- Click "View Full" button on certificate cards
- Full-size image modal display
- Close with X button or Escape key
- Click outside image to close

### Contact Form
- Email validation
- Form submission handling
- Success/error notifications
- Form reset after submission

### Scroll Animations
- Elements fade in as you scroll
- Parallax effect on hero section
- Active navigation highlighting

## SEO Optimization

The portfolio includes:
- Semantic HTML5 elements
- Meta tags for responsiveness
- Proper heading hierarchy
- Alt text for images
- Schema.org structured data ready

## Hosting

You can host this portfolio on:
1. **GitHub Pages** - Free hosting for static sites
2. **Netlify** - Easy deployment from Git
3. **Vercel** - Optimized for web apps
4. **Traditional Hosting** - Any web host that serves HTML

## Deployment Steps (GitHub Pages)

1. Create a GitHub repository named `portfolio`
2. Push the website files to the repository
3. Enable GitHub Pages in repository settings
4. Your site will be live at: `https://yourusername.github.io/portfolio`

## Contact Form Integration

To make the contact form functional:

1. **Option 1**: Use Formspree (Recommended)
   - Go to https://formspree.io
   - Create a new form
   - Replace the form action in HTML:
   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```

2. **Option 2**: Use EmailJS
   - Sign up at https://www.emailjs.com
   - Follow their integration guide
   - Update the JavaScript in `assets/js/script.js`

3. **Option 3**: Backend API
   - Create your own backend endpoint
   - Update the form submission in `script.js`

## Maintenance

Regular updates recommended:
- Update Font Awesome icon library (CDN link)
- Update personal information and achievements
- Add new certificates as you earn them
- Update project links and descriptions
- Check for broken links quarterly

## License

This portfolio template is free to use and modify for personal and commercial purposes.

## Credits

- **Icons**: Font Awesome (https://fontawesome.com)
- **Typography**: Segoe UI System Font
- **Design Inspiration**: Modern portfolio trends

## Support

For issues or questions:
1. Check the code comments
2. Review the customization guide above
3. Test in different browsers
4. Clear browser cache if styles don't update

## Quick Customization Checklist

- [ ] Update personal name and title in hero section
- [ ] Add your education details
- [ ] Add your certificate images
- [ ] Update achievements/memberships
- [ ] Change social media links
- [ ] Update email address
- [ ] Customize color scheme
- [ ] Test on mobile devices
- [ ] Test contact form
- [ ] Deploy to hosting platform

---

**Version**: 1.0
**Last Updated**: April 2025
**Built with**: HTML5, CSS3, JavaScript (Vanilla)
