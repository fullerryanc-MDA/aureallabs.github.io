# Aureal Labs Website - Quick Reference

## 🎨 Design Specifications

### Colors
- **Background**: `#2E3A46` (Slate Gray)
- **Accent**: `#C9A66B` (Muted Gold)
- **Text Primary**: `#FFFFFF` (White)
- **Text Secondary**: `#D0D0D0` (Light Gray)

### Typography
- **Font Family**: Inter (via Google Fonts)
- **Hero Title**: 3rem / 700 weight
- **Body Text**: 1.125rem / 400 weight

### Logo Placeholder
- 50x50px square with rounded corners
- Gold gradient background
- "AL" text in center

## 📋 Content Structure

### Header
- Logo placeholder + "Aureal Labs LLC"

### Hero Section
- Main title: "AI-Powered Metal-Detecting Companion App"
- Subtitle: "Discover. Identify. Preserve."

### About Section
Three-sentence description about Aureal's mission and technology

### Contact Section
- Email: hello@aureallabs.com (clickable link)
- Location: Gainesville, Florida, USA (with icons)

### Footer
- Copyright: © 2025 Aureal Labs LLC · All Rights Reserved

## 📁 File Structure

```
aureallabs.github.io/
├── index.html          # Main HTML (3.3 KB)
├── styles.css          # Stylesheet (3.2 KB)
├── CNAME              # Domain config (19 bytes)
└── README.md          # Documentation (3.9 KB)
```

## 🚀 Quick Deploy Commands

```bash
# 1. Navigate to repo
cd aureallabs.github.io

# 2. Add files
git add .

# 3. Commit
git commit -m "Deploy Aureal Labs landing page"

# 4. Push
git push origin main
```

## 🌐 DNS Records

### CNAME Record
```
Host: www
Value: fullerryanc-mda.github.io
TTL: 3600
```

### A Records (4 records needed)
```
Host: @
Values:
  185.199.108.153
  185.199.109.153
  185.199.110.153
  185.199.111.153
```

## ✅ Launch Checklist

1. ✅ Files created
2. ⏳ Push to GitHub
3. ⏳ Enable GitHub Pages
4. ⏳ Configure DNS
5. ⏳ Wait for propagation (10-30 min)
6. ⏳ Verify SSL certificate
7. ⏳ Test live site

## 📱 Responsive Design

- Desktop: Full layout (1200px max width)
- Tablet: Adjusted font sizes
- Mobile: Stacked layout, optimized spacing

## 🔗 Important Links

- Repository: https://github.com/fullerryanc-MDA/aureallabs.github.io
- Live Site: https://www.aureallabs.com (post-deployment)
- DNS Checker: https://dnschecker.org/

---

**Ready to deploy!** Follow the DEPLOYMENT_GUIDE.md for step-by-step instructions.
