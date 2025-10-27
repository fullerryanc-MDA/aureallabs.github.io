# Aureal Labs Website - Deployment Instructions (v2.0)

## 🎯 Mission-Focused Redesign Complete ✅

The Aureal Labs landing page has been completely rebuilt to reflect your true mission: **responsible discovery, ethical exploration, and heritage preservation** — not AI signal prediction.

## Files Created ✅

The following files have been created and are ready for deployment:

1. **index.html** - Complete mission-driven landing page with 8 sections
2. **styles.css** - Professional slate-gray & muted gold theme with CSS variables
3. **script.js** - Navigation functionality and smooth scroll animations
4. **CNAME** - Custom domain configuration file
5. **README.md** - Comprehensive documentation for future updates

## 🎨 What's New

### Design Features
- ✅ Sticky navigation bar with smooth scroll
- ✅ Full-screen hero with topographic texture overlay
- ✅ Mission section with core values
- ✅ Feature cards with hover animations (Smart Mapping, PermissionLink™, RFN, Eco Impact)
- ✅ Ethos manifesto section
- ✅ Call-to-action banner for early access
- ✅ Fully responsive mobile menu
- ✅ Smooth scroll animations on page load

### Content Focus
- ✅ Emphasizes responsible discovery and ethical exploration
- ✅ Highlights heritage preservation and property rights respect
- ✅ Features PermissionLink™ for secure land access
- ✅ Promotes Responsible Finder Network (RFN) for museum partnerships
- ✅ NO references to AI signal prediction or inference
- ✅ Privacy-first, transparency-focused messaging

## 📋 Deployment Steps

### Step 1: Clone or Access Your GitHub Repository

```bash
# Clone the repository (if not already cloned)
git clone https://github.com/fullerryanc-MDA/aureallabs.github.io.git
cd aureallabs.github.io
```

### Step 2: Add the Website Files

Copy all five files to the root of your repository:

```bash
# Copy files to repository root
cp index.html styles.css script.js CNAME README.md /path/to/aureallabs.github.io/
```

### Step 3: Commit and Push to GitHub

```bash
# Navigate to repository
cd aureallabs.github.io

# Add all files
git add index.html styles.css script.js CNAME README.md

# Commit with descriptive message
git commit -m "v2.0: Mission-focused redesign - responsible discovery companion"

# Push to main branch
git push origin main
```

### Step 4: Enable GitHub Pages

1. Go to: https://github.com/fullerryanc-MDA/aureallabs.github.io
2. Click **Settings** (top menu)
3. Click **Pages** in the left sidebar
4. Under "Build and deployment":
   - **Source**: Deploy from a branch
   - **Branch**: `main`
   - **Folder**: `/ (root)`
5. Click **Save**
6. GitHub will show: "Your site is live at https://www.aureallabs.com"

### Step 5: Configure DNS Records

#### In Zoho Mail (or your domain registrar):

**Required DNS Records:**

1. **CNAME Record** (for www subdomain):
   ```
   Type: CNAME
   Host: www
   Value: fullerryanc-mda.github.io
   TTL: 3600
   ```

2. **A Records** (for root domain - add all 4):
   ```
   Type: A
   Host: @ (or blank/root)
   
   Values (create 4 separate A records):
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   
   TTL: 3600
   ```

#### Zoho-Specific Steps:

1. Log into Zoho Mail Control Panel
2. Navigate to **Domain Settings** → **DNS Management**
3. Click **Add Record**
4. Add the CNAME record first
5. Add all four A records one by one
6. Click **Save** after each record
7. Verify all records appear in your DNS table

### Step 6: Wait for DNS Propagation

- **Typical time**: 10-30 minutes
- **Maximum time**: Up to 48 hours (rare)
- **Check status**: https://dnschecker.org/
  - Enter `www.aureallabs.com`
  - Select "CNAME" type
  - Should show: `fullerryanc-mda.github.io`

### Step 7: Verify SSL Certificate

1. Wait 10-15 minutes after DNS propagates
2. Visit https://www.aureallabs.com
3. GitHub automatically issues Let's Encrypt SSL
4. Look for padlock icon in browser address bar
5. If SSL isn't active, wait up to 24 hours

### Step 8: Configure Custom Domain in GitHub

1. Return to repository **Settings** → **Pages**
2. Under "Custom domain":
   - Should automatically show: `www.aureallabs.com`
   - If not, enter it manually and click **Save**
3. Wait for DNS check to complete (green checkmark)
4. Check **Enforce HTTPS** (may need to wait for SSL cert)
5. Status should show: "Your site is published at https://www.aureallabs.com"

## ✅ Verification Checklist

Complete these steps to verify deployment:

- [ ] All files pushed to GitHub main branch
- [ ] GitHub Pages enabled (Settings → Pages)
- [ ] DNS CNAME record added and verified
- [ ] DNS A records added (all 4)
- [ ] Wait 15-30 minutes for DNS propagation
- [ ] Visit https://www.aureallabs.com - site loads
- [ ] Check hero section displays properly
- [ ] Test navigation - smooth scroll works
- [ ] Test mobile menu (hamburger icon)
- [ ] Verify all sections present (Mission, Features, Ethos, Contact)
- [ ] SSL certificate active (padlock icon)
- [ ] Root domain redirects: aureallabs.com → www.aureallabs.com
- [ ] "Enforce HTTPS" enabled in GitHub Pages

## 🧪 Testing Your Site

Once deployed, test these scenarios:

### URL Redirects
- ✅ https://www.aureallabs.com (primary URL - should load)
- ✅ http://www.aureallabs.com (should redirect to HTTPS)
- ✅ https://aureallabs.com (should redirect to www)
- ✅ http://aureallabs.com (should redirect to www + HTTPS)

### Navigation
- ✅ Click "Mission" - smooth scroll to mission section
- ✅ Click "Features" - smooth scroll to features
- ✅ Click "Ethos" - smooth scroll to ethos
- ✅ Click "Contact" - smooth scroll to contact
- ✅ Click "Join Beta Waitlist" - opens email client

### Mobile Testing
- ✅ Visit on phone - responsive layout works
- ✅ Hamburger menu appears on mobile
- ✅ Click hamburger - menu slides in
- ✅ Click nav link - menu closes, page scrolls
- ✅ All text readable on small screens

### Interactive Elements
- ✅ Feature cards have hover effects
- ✅ Buttons have hover states
- ✅ Navbar becomes slightly opaque on scroll
- ✅ Sections fade in as you scroll down

## 🍎 Apple Developer Program Verification

Once your site is live at https://www.aureallabs.com:

### Pre-Enrollment Checklist
1. ✅ Site loads without errors
2. ✅ Company name "Aureal Labs LLC" is prominently displayed
3. ✅ Contact email "hello@aureallabs.com" is visible in Contact section
4. ✅ Location "Gainesville, Florida, USA" is shown
5. ✅ Professional appearance matches company mission
6. ✅ SSL certificate active (HTTPS)

### During Enrollment
Use these exact details:
- **Organization Name**: Aureal Labs LLC
- **Website**: https://www.aureallabs.com
- **Email**: hello@aureallabs.com
- **Location**: Gainesville, Florida, USA

Apple will verify your website matches your company information.

## 🐛 Troubleshooting

### Issue: Site Shows 404 Error
**Solutions:**
- Verify GitHub Pages is enabled
- Check CNAME file contains exactly: `www.aureallabs.com`
- Ensure files are in repository root, not a subdirectory
- Wait 2-3 minutes after pushing changes

### Issue: DNS Not Resolving
**Solutions:**
- Double-check DNS records in Zoho
- Wait full 30 minutes for propagation
- Use https://dnschecker.org/ to verify
- Flush your local DNS cache:
  - Mac: `sudo dscacheutil -flushcache`
  - Windows: `ipconfig /flushdns`

### Issue: SSL Certificate Not Working
**Solutions:**
- Wait 24 hours for automatic certificate generation
- Remove and re-add custom domain in GitHub Pages
- Ensure "Enforce HTTPS" is checked
- Verify DNS is fully propagated first

### Issue: Mobile Menu Not Working
**Solutions:**
- Verify `script.js` is in repository root
- Check browser console for JavaScript errors
- Ensure `<script src="script.js"></script>` is in `index.html`
- Clear browser cache and reload

### Issue: Smooth Scroll Not Working
**Solutions:**
- Check that section IDs match navigation hrefs
- Verify JavaScript is loading (check console)
- Try different browser (some older browsers don't support)

### Issue: Images or Styles Not Loading
**Solutions:**
- Verify file paths are correct (use relative paths)
- Check that `styles.css` is in same directory as `index.html`
- Clear browser cache
- Wait 2-3 minutes after deployment

## 📱 Page Structure Reference

Your site now contains these sections in order:

1. **Navigation Bar** (sticky)
   - Logo: "AU" icon + "Aureal Labs"
   - Links: Home, Mission, Features, Ethos, Contact

2. **Hero Section** (#home)
   - Headline: "Your Digital Companion for Responsible Discovery"
   - Subtext: "Map your hunts, manage permissions..."
   - Two CTAs: "Explore the Mission" + "Join Beta Waitlist"

3. **Mission Section** (#mission)
   - Core mission statement
   - Values: Compass, Handshake, Map Pin icons

4. **Features Section** (#features)
   - Smart Hunt Mapping 🗺️
   - PermissionLink™ Access 🤝
   - Responsible Finder Network 🏛️
   - Eco Impact Insights 🌿

5. **Ethos Section** (#ethos)
   - Brand manifesto quote
   - AU emblem

6. **CTA Banner**
   - "Launching 2025" message
   - "Request Early Access" button

7. **Contact Section** (#contact)
   - Email: hello@aureallabs.com
   - Location: Gainesville, Florida, USA

8. **Footer**
   - Copyright © 2025 Aureal Labs LLC
   - Privacy Policy · Terms of Use links

## 🎨 Customization Tips

### Change Colors
Edit `styles.css` root variables:
```css
:root {
    --color-bg: #2E3A46;        /* Main background */
    --color-accent: #C9A66B;    /* Gold accent */
    --color-text: #ECECEC;      /* Main text */
}
```

### Add New Features
Copy a `.feature-card` block in `index.html`:
```html
<div class="feature-card">
    <div class="feature-icon"><!-- SVG icon --></div>
    <h3 class="feature-title">New Feature</h3>
    <p class="feature-description">Description here</p>
</div>
```

### Update Mission Text
Find the `.mission-text` paragraphs in `index.html` and edit as needed.

## 📞 Need Help?

- **Email**: hello@aureallabs.com
- **Repository Issues**: https://github.com/fullerryanc-MDA/aureallabs.github.io/issues
- **DNS Help**: Check your domain registrar's documentation

## 📊 Success Metrics

Your site will be successfully deployed when:
- ✅ https://www.aureallabs.com loads instantly
- ✅ All 8 sections visible and styled correctly
- ✅ Navigation smooth scrolls to each section
- ✅ Mobile menu works on phones
- ✅ SSL certificate shows padlock icon
- ✅ Site passes Apple Developer verification
- ✅ Professional, mission-driven appearance
- ✅ No references to "AI signal" anywhere

---

## 🚀 Ready to Launch!

You now have a professional, mission-focused landing page that:
- Positions Aureal Labs as a responsible discovery platform
- Emphasizes ethical exploration and heritage preservation
- Showcases core features (mapping, permissions, RFN)
- Passes Apple Developer Program verification
- Reflects your true company values and mission

**Estimated deployment time**: 30-45 minutes (including DNS propagation)

**Live site**: https://www.aureallabs.com (after deployment)

---

**Created**: October 27, 2025  
**Version**: 2.0 (Mission-focused redesign)  
**Repository**: https://github.com/fullerryanc-MDA/aureallabs.github.io
