# Aureal Labs LLC - Official Website

This repository hosts the official landing page for Aureal Labs LLC at [www.aureallabs.com](https://www.aureallabs.com).

## Overview

A minimal, professional landing page showcasing Aureal Labs' AI-powered metal-detecting companion app.

## Technology Stack

- **Static Site**: HTML5 & CSS3
- **Hosting**: GitHub Pages
- **Custom Domain**: www.aureallabs.com
- **Font**: Inter (via Google Fonts)

## File Structure

```
.
├── index.html          # Main HTML file
├── styles.css          # Stylesheet
├── CNAME              # Custom domain configuration
└── README.md          # This file
```

## Updating Content

### Changing Text Content

1. Open `index.html` in your editor
2. Locate the section you want to update:
   - **Company Name**: Find `<h1>Aureal Labs LLC</h1>` in the header
   - **Hero Title**: Find `<h2 class="hero-title">` in the hero section
   - **About Text**: Find `<p class="about-text">` in the about section
   - **Contact Email**: Find `<a href="mailto:hello@aureallabs.com">` in the contact section
   - **Location**: Find the location text in the contact section
   - **Footer Year**: Find the copyright text in the footer
3. Save your changes
4. Commit and push to the `main` branch

### Changing Colors

1. Open `styles.css` in your editor
2. Update the color variables:
   - **Background**: Currently `#2E3A46` (slate-gray)
   - **Accent Color**: Currently `#C9A66B` (muted gold)
   - Look for these hex codes throughout the CSS file
3. Save, commit, and push your changes

### Adding a Logo

1. Add your logo image file to the repository (e.g., `logo.png`)
2. In `index.html`, replace the logo placeholder:
   ```html
   <!-- Replace this: -->
   <div class="logo-placeholder">AL</div>
   
   <!-- With this: -->
   <img src="logo.png" alt="Aureal Labs Logo" class="logo-image">
   ```
3. In `styles.css`, add styles for the logo image:
   ```css
   .logo-image {
       height: 50px;
       width: auto;
   }
   ```

### Deploying Changes

All changes pushed to the `main` branch are automatically deployed to GitHub Pages within a few minutes.

```bash
git add .
git commit -m "Update website content"
git push origin main
```

## GitHub Pages Setup

The site is configured to deploy from:
- **Branch**: `main`
- **Folder**: `/` (root)
- **Custom Domain**: www.aureallabs.com (configured via CNAME file)

To verify or update GitHub Pages settings:
1. Go to repository Settings → Pages
2. Ensure source is set to "Deploy from a branch"
3. Branch should be `main` with folder `/ (root)`
4. Custom domain should show `www.aureallabs.com`

## DNS Configuration

For the custom domain to work, the following DNS records should be configured in your domain registrar (e.g., Zoho):

### Required Records

1. **CNAME Record for www subdomain**:
   - Host: `www`
   - Value: `fullerryanc-mda.github.io`
   - TTL: 3600 (or auto)

2. **Root Domain Redirect** (choose one method):
   - **Option A**: A Records pointing to GitHub Pages IPs:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```
   - **Option B**: Domain forwarding from `aureallabs.com` to `www.aureallabs.com`

### Verification

After DNS changes, allow 10-30 minutes for propagation. Then verify:
- `https://www.aureallabs.com` loads the site
- SSL certificate is active (HTTPS)
- `http://aureallabs.com` redirects to `https://www.aureallabs.com`

## Apple Developer Program Enrollment

This website serves as verification for Apple Developer Program enrollment:
- **Company Name**: Aureal Labs LLC
- **Contact Email**: hello@aureallabs.com
- **Website**: https://www.aureallabs.com

Ensure the site is live and displays matching company information before submitting your Apple Developer enrollment.

## Support

For questions or issues with the website, contact: hello@aureallabs.com

---

© 2025 Aureal Labs LLC · All Rights Reserved
