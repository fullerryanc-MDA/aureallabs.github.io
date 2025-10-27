# Aureal Labs LLC - Official Website

This repository hosts the official landing page for Aureal Labs LLC at [www.aureallabs.com](https://www.aureallabs.com).

## Overview

A professional, mission-driven landing page showcasing Aureal Labs' commitment to responsible metal detecting, ethical discovery, and heritage preservation through intelligent mapping and permission management tools.

## Brand Identity

**Mission:** Empowering detectorists to explore responsibly — protecting heritage, respecting property rights, and preserving stories.

**Core Values:** 
- Responsible discovery
- Ethical exploration
- Heritage preservation
- Privacy-first technology
- Transparent community building

## Technology Stack

- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Hosting**: GitHub Pages
- **Custom Domain**: www.aureallabs.com
- **Font**: Inter (via Google Fonts)
- **Design**: Responsive, accessible (WCAG AA compliant)

## File Structure

```
.
├── index.html          # Main HTML file with semantic structure
├── styles.css          # Complete stylesheet with CSS variables
├── script.js           # Navigation and smooth scroll functionality
├── CNAME              # Custom domain configuration
└── README.md          # This file
```

## Design Specifications

### Color Palette
- **Background**: `#2E3A46` (Slate Gray)
- **Accent**: `#C9A66B` (Muted Gold)
- **Text Primary**: `#ECECEC` (Off-white)
- **Text Secondary**: `#B8B8B8` (Light Gray)
- **Dark Accent**: `#1F2933` (Deep Slate)

### Typography
- **Font Family**: Inter
- **Weights**: 300 (Light), 400 (Regular), 500 (Medium), 600 (Semi-bold), 700 (Bold)
- **Scale**: Responsive font sizing for all screen sizes

### Layout Features
- Sticky navigation with smooth scroll
- Full-height hero section with topographic texture
- Feature cards with hover effects
- Mobile-responsive hamburger menu
- Smooth scroll-triggered animations

## Page Sections

1. **Navigation Bar** - Sticky header with smooth scroll links
2. **Hero Section** - Full-screen introduction with dual CTAs
3. **Mission Section** - Company values and philosophy
4. **Features Section** - Four core product features
5. **Ethos Section** - Brand manifesto and values
6. **CTA Banner** - Call-to-action for early access
7. **Contact Section** - Email and location information
8. **Footer** - Copyright and legal links

## Updating Content

### Changing Text Content

All content is in `index.html`. Key sections to update:

**Hero Section:**
```html
<h1 class="hero-headline">Your Digital Companion for Responsible Discovery</h1>
```

**Mission Text:**
```html
<p class="mission-text">
    Aureal Labs builds tools that empower detectorists...
</p>
```

**Feature Cards:**
Each feature is in a `.feature-card` div with icon, title, and description.

**Contact Information:**
```html
<a href="mailto:hello@aureallabs.com">hello@aureallabs.com</a>
```

### Changing Colors

Update CSS variables in `styles.css`:

```css
:root {
    --color-bg: #2E3A46;
    --color-accent: #C9A66B;
    --color-text: #ECECEC;
    /* etc. */
}
```

### Adding/Modifying Features

Features are in a grid layout. Add a new feature card:

```html
<div class="feature-card">
    <div class="feature-icon">
        <!-- SVG icon here -->
    </div>
    <h3 class="feature-title">Feature Name</h3>
    <p class="feature-description">Feature description</p>
</div>
```

### Updating Navigation Links

Modify the nav links in the `<nav class="navbar">` section:

```html
<ul class="nav-links">
    <li><a href="#home">Home</a></li>
    <li><a href="#mission">Mission</a></li>
    <!-- Add more links -->
</ul>
```

Ensure each link points to a section with a matching `id` attribute.

## Deploying Changes

All changes pushed to the `main` branch are automatically deployed to GitHub Pages within 1-2 minutes.

```bash
# Standard workflow
git add .
git commit -m "Update: [describe your changes]"
git push origin main
```

## GitHub Pages Configuration

The site is configured to deploy from:
- **Branch**: `main`
- **Folder**: `/` (root)
- **Custom Domain**: www.aureallabs.com (configured via CNAME file)

To verify settings:
1. Go to repository **Settings** → **Pages**
2. Source: "Deploy from a branch"
3. Branch: `main` / Folder: `/ (root)`
4. Custom domain: `www.aureallabs.com`
5. Enforce HTTPS: ✓ (enabled)

## DNS Configuration

For the custom domain, configure these DNS records in your domain registrar:

### Required Records

**CNAME Record (www subdomain):**
```
Host: www
Value: fullerryanc-mda.github.io
TTL: 3600
```

**A Records (root domain):**
```
Host: @
Values:
  185.199.108.153
  185.199.109.153
  185.199.110.153
  185.199.111.153
TTL: 3600
```

### Verification Steps

1. Configure DNS records as above
2. Wait 10-30 minutes for propagation
3. Verify at https://dnschecker.org/
4. Test these URLs:
   - ✅ https://www.aureallabs.com
   - ✅ http://www.aureallabs.com (redirects to HTTPS)
   - ✅ https://aureallabs.com (redirects to www)
   - ✅ http://aureallabs.com (redirects to www/HTTPS)

## Mobile Responsiveness

The site is fully responsive with breakpoints at:
- **Desktop**: 1200px+ (full layout)
- **Tablet**: 768px-1199px (adjusted spacing)
- **Mobile**: <768px (hamburger menu, stacked layout)
- **Small Mobile**: <480px (optimized for small screens)

## Accessibility

- Semantic HTML5 structure
- ARIA labels on interactive elements
- Keyboard navigation support
- Sufficient color contrast (WCAG AA)
- Focus indicators on all interactive elements
- Alt text for images (when added)

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Performance

- Minimal dependencies (Google Fonts only)
- Optimized CSS with CSS variables
- Lazy-loaded animations with Intersection Observer
- No heavy frameworks or libraries

## Apple Developer Program Verification

This website serves as official verification for Apple Developer Program enrollment:

- **Company Name**: Aureal Labs LLC
- **Website**: https://www.aureallabs.com
- **Contact Email**: hello@aureallabs.com
- **Location**: Gainesville, Florida, USA

Ensure the site is live and displays matching company information before submitting Apple Developer enrollment.

## Future Enhancements

Potential additions for future updates:
- Blog section for company news
- Team/About page
- FAQ section
- Press kit/media resources
- Newsletter signup integration
- Analytics integration (privacy-focused)

## Troubleshooting

### Site Not Loading
- Verify DNS records are correctly configured
- Check GitHub Pages is enabled in repo settings
- Wait 30 minutes after DNS changes
- Clear browser cache

### SSL Certificate Issues
- GitHub automatically issues certificates
- Wait up to 24 hours after DNS configuration
- Ensure "Enforce HTTPS" is checked in GitHub Pages settings

### Mobile Menu Not Working
- Verify `script.js` is loading correctly
- Check browser console for JavaScript errors
- Test on multiple devices/browsers

### Styling Issues
- Clear browser cache
- Verify `styles.css` is linked correctly in `index.html`
- Check for CSS syntax errors

## Support

For questions, issues, or feature requests:
- **Email**: hello@aureallabs.com
- **Repository**: https://github.com/fullerryanc-MDA/aureallabs.github.io

## License

© 2025 Aureal Labs LLC · All Rights Reserved

---

**Last Updated**: October 27, 2025  
**Version**: 2.0 (Mission-focused redesign)  
**Repository**: https://github.com/fullerryanc-MDA/aureallabs.github.io  
**Live Site**: https://www.aureallabs.com
