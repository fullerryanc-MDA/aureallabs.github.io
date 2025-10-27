# Aureal Labs Website - Deployment Instructions

## Files Created ✅

The following files have been created and are ready for deployment:

1. **index.html** - Main landing page
2. **styles.css** - Stylesheet with slate-gray and muted gold theme
3. **CNAME** - Custom domain configuration file
4. **README.md** - Documentation for future updates

## Deployment Steps

### Step 1: Clone or Access Your GitHub Repository

```bash
# Clone the repository (if not already cloned)
git clone https://github.com/fullerryanc-MDA/aureallabs.github.io.git
cd aureallabs.github.io
```

### Step 2: Add the Website Files

Copy the four files (index.html, styles.css, CNAME, README.md) to the root of your repository:

```bash
# Copy files to repository root
cp index.html styles.css CNAME README.md /path/to/aureallabs.github.io/
```

### Step 3: Commit and Push to GitHub

```bash
# Navigate to repository
cd aureallabs.github.io

# Add all files
git add index.html styles.css CNAME README.md

# Commit with message
git commit -m "Initial deployment: Aureal Labs landing page"

# Push to main branch
git push origin main
```

### Step 4: Enable GitHub Pages

1. Go to your repository on GitHub: https://github.com/fullerryanc-MDA/aureallabs.github.io
2. Click **Settings** (top right)
3. Click **Pages** in the left sidebar
4. Under "Source", select:
   - **Branch**: `main`
   - **Folder**: `/ (root)`
5. Click **Save**
6. GitHub will display: "Your site is ready to be published at https://fullerryanc-mda.github.io/aureallabs.github.io/"

### Step 5: Configure DNS (Zoho or Your Domain Registrar)

#### Required DNS Records:

1. **CNAME Record** (for www subdomain):
   - **Host/Name**: `www`
   - **Value/Target**: `fullerryanc-mda.github.io`
   - **TTL**: 3600 (or automatic)

2. **A Records** (for root domain - choose this option):
   Add four A records pointing to GitHub Pages servers:
   - **Host/Name**: `@` (or leave blank for root)
   - **Values** (create 4 separate A records):
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```
   - **TTL**: 3600 (or automatic)

   **OR**

3. **Domain Forwarding** (alternative for root domain):
   - Configure `aureallabs.com` to forward to `www.aureallabs.com`
   - Enable "301 Permanent Redirect"

#### Zoho-Specific Instructions:

1. Log into Zoho Mail Control Panel
2. Go to **Domain Settings** → **DNS**
3. Add the records listed above
4. Save changes

### Step 6: Wait for DNS Propagation

- DNS changes typically take 10-30 minutes
- Can take up to 48 hours in rare cases
- Check propagation: https://dnschecker.org/

### Step 7: Verify SSL Certificate

1. Wait 5-10 minutes after DNS propagation
2. Visit https://www.aureallabs.com
3. GitHub automatically issues a Let's Encrypt SSL certificate
4. If SSL isn't working immediately, wait up to 24 hours

### Step 8: Verify Custom Domain in GitHub

1. Return to repository Settings → Pages
2. Under "Custom domain", you should see: `www.aureallabs.com`
3. Check "Enforce HTTPS" once certificate is active
4. If you see errors, click "Remove" then re-add the domain

## Verification Checklist

- [ ] Files pushed to GitHub repository
- [ ] GitHub Pages enabled (Settings → Pages)
- [ ] DNS CNAME record added (www → fullerryanc-mda.github.io)
- [ ] DNS A records or forwarding configured
- [ ] Wait 10-30 minutes for DNS propagation
- [ ] Visit https://www.aureallabs.com - site loads
- [ ] Visit http://aureallabs.com - redirects to www subdomain
- [ ] SSL certificate active (padlock icon in browser)
- [ ] "Enforce HTTPS" enabled in GitHub Pages settings

## Testing Your Site

Once deployed, test these URLs:
- ✅ https://www.aureallabs.com (primary URL)
- ✅ http://www.aureallabs.com (should redirect to HTTPS)
- ✅ http://aureallabs.com (should redirect to www subdomain)
- ✅ https://aureallabs.com (should redirect to www subdomain)

## For Apple Developer Enrollment

Once your site is live:
1. Verify https://www.aureallabs.com displays correctly
2. Confirm company name "Aureal Labs LLC" is visible
3. Confirm email "hello@aureallabs.com" is displayed
4. Use this information when enrolling:
   - **Company Name**: Aureal Labs LLC
   - **Website**: https://www.aureallabs.com
   - **Email**: hello@aureallabs.com

## Troubleshooting

### Site Not Loading
- Verify DNS records are correct
- Check DNS propagation status
- Ensure GitHub Pages is enabled
- Wait 30 minutes after DNS changes

### SSL Certificate Not Working
- Wait 24 hours for automatic certificate generation
- Ensure "Enforce HTTPS" is checked in GitHub Pages settings
- Try removing and re-adding the custom domain

### Domain Shows 404 Error
- Verify CNAME file contains exactly: `www.aureallabs.com`
- Check that files are in the root directory
- Ensure GitHub Pages is set to deploy from `main` branch, `/` folder

## Need Help?

Contact hello@aureallabs.com for support with the website.

---

**Created**: October 27, 2025  
**Repository**: https://github.com/fullerryanc-MDA/aureallabs.github.io  
**Live Site**: https://www.aureallabs.com (once deployed)
