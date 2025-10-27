# Aureal Labs Website - Quick Reference v2.0

## 🎯 Mission Statement

**"Your Digital Companion for Responsible Discovery"**

Map your hunts, manage permissions, and share history — ethically and privately.

## 🎨 Design Specifications

### Color Palette
| Element | Hex Code | Usage |
|---------|----------|-------|
| Background | `#2E3A46` | Main slate gray background |
| Accent | `#C9A66B` | Muted gold for CTAs, icons, links |
| Accent Hover | `#D4B67C` | Lighter gold for hover states |
| Text Primary | `#ECECEC` | Main body text |
| Text Secondary | `#B8B8B8` | Subtext, less emphasis |
| Dark Accent | `#1F2933` | Deep slate for contrast |

### Typography
- **Font**: Inter (Google Fonts)
- **Weights**: 300, 400, 500, 600, 700
- **Hero Title**: 3.5rem / 700 weight
- **Section Title**: 2.5rem / 700 weight
- **Body Text**: 1.125rem / 400 weight
- **Feature Cards**: 1.375rem title / 600 weight

### Visual Elements
- Topographic texture overlay on hero
- Smooth scroll animations
- Hover lift effects on feature cards
- Sticky navigation with blur backdrop
- Responsive mobile hamburger menu

## 📐 Page Layout

### Navigation (Sticky)
```
Logo (AU icon) + "Aureal Labs" | Home · Mission · Features · Ethos · Contact
```

### 8 Main Sections
1. **Hero** - Full-screen introduction with dual CTAs
2. **Mission** - Company values and philosophy  
3. **Features** - 4 core tools in grid layout
4. **Ethos** - Brand manifesto quote
5. **CTA Banner** - Early access call-to-action
6. **Contact** - Email and location
7. **Footer** - Copyright and legal links

## 🔧 Core Features Highlighted

1. **🗺️ Smart Hunt Mapping**
   - Track paths, finds, grid coverage
   - Works offline

2. **🤝 PermissionLink™ Access**
   - Secure land permission requests
   - Respectful property rights management

3. **🏛️ Responsible Finder Network (RFN)**
   - Museum partnerships
   - Heritage discovery sharing

4. **🌿 Eco Impact Insights**
   - Cleanup tracking
   - Restoration visualization

## 📁 File Structure

```
aureallabs.github.io/
├── index.html          # Main HTML (11 KB)
├── styles.css          # Complete stylesheet (9.2 KB)
├── script.js           # Navigation & animations (1.8 KB)
├── CNAME              # Domain config (20 bytes)
└── README.md          # Full documentation (8.4 KB)
```

## 🚀 Quick Deploy Commands

```bash
# Clone repo
git clone https://github.com/fullerryanc-MDA/aureallabs.github.io.git
cd aureallabs.github.io

# Copy your files
cp /path/to/files/* .

# Deploy
git add .
git commit -m "v2.0: Mission-focused redesign"
git push origin main

# Site live in 2-3 minutes at:
# https://www.aureallabs.com
```

## 🌐 DNS Configuration

### CNAME Record
```
Host: www
Value: fullerryanc-mda.github.io
TTL: 3600
```

### A Records (Root Domain)
```
Host: @
Values:
  185.199.108.153
  185.199.109.153
  185.199.110.153
  185.199.111.153
TTL: 3600
```

## 📱 Responsive Breakpoints

| Device | Width | Layout Changes |
|--------|-------|----------------|
| Desktop | 1200px+ | Full layout, side-by-side nav |
| Tablet | 768-1199px | Adjusted spacing, nav collapses |
| Mobile | <768px | Hamburger menu, stacked sections |
| Small Mobile | <480px | Optimized for smallest screens |

## 🎭 Key Messaging

### What We Are:
- ✅ Responsible discovery companion
- ✅ Ethical exploration platform
- ✅ Heritage preservation tool
- ✅ Privacy-first technology
- ✅ Community-driven network

### What We're NOT:
- ❌ AI signal predictor
- ❌ Treasure hunting exploit
- ❌ Data harvesting app
- ❌ Generic metal detector app

## ✅ Pre-Launch Checklist

### Technical
- [ ] All files in repo root
- [ ] GitHub Pages enabled
- [ ] DNS CNAME configured
- [ ] DNS A records added
- [ ] Custom domain verified
- [ ] SSL certificate active
- [ ] Mobile menu functional
- [ ] Smooth scroll working

### Content
- [ ] Company name prominent
- [ ] Contact email visible
- [ ] Location displayed
- [ ] Mission statement clear
- [ ] No AI signal references
- [ ] Professional tone throughout

### Apple Verification
- [ ] Site live at www.aureallabs.com
- [ ] Matches company name
- [ ] Shows contact email
- [ ] Professional appearance
- [ ] SSL enabled (HTTPS)

## 🔗 Important URLs

| Purpose | URL |
|---------|-----|
| Live Site | https://www.aureallabs.com |
| Repository | https://github.com/fullerryanc-MDA/aureallabs.github.io |
| DNS Check | https://dnschecker.org/ |
| SSL Check | https://www.ssllabs.com/ssltest/ |
| Email | hello@aureallabs.com |

## 🎯 Success Criteria

Your site is successfully deployed when:

✅ **Loads instantly** at https://www.aureallabs.com  
✅ **Sticky nav** works with smooth scroll  
✅ **8 sections** all visible and styled  
✅ **Mobile menu** toggles properly  
✅ **Feature cards** have hover effects  
✅ **SSL active** (padlock icon visible)  
✅ **Responsive** on all device sizes  
✅ **Mission-focused** messaging throughout  
✅ **Professional** appearance for Apple verification  

## 📊 Performance Metrics

- **Page Load**: <2 seconds
- **Total Size**: ~30 KB (HTML + CSS + JS)
- **Dependencies**: 1 (Google Fonts)
- **Lighthouse Score**: 95+ (target)
- **Mobile Friendly**: ✅ Yes
- **SEO Optimized**: ✅ Yes

## 🎨 CSS Architecture

### CSS Variables (Root)
```css
:root {
    --color-bg: #2E3A46;
    --color-accent: #C9A66B;
    --color-text: #ECECEC;
    --transition: all 0.3s ease;
}
```

### Key Classes
- `.navbar` - Sticky navigation
- `.hero` - Full-screen hero section
- `.section` - Standard section spacing
- `.feature-card` - Feature grid items
- `.btn` - Button base styles
- `.btn-primary` - Gold CTA button
- `.btn-secondary` - Outlined button

## 💡 Quick Updates

### Change Hero Text
```html
<!-- Line 35 in index.html -->
<h1 class="hero-headline">Your New Headline</h1>
```

### Add Feature
```html
<!-- Copy this block in features section -->
<div class="feature-card">
    <div class="feature-icon"><!-- SVG --></div>
    <h3 class="feature-title">Title</h3>
    <p class="feature-description">Description</p>
</div>
```

### Update Colors
```css
/* In styles.css :root section */
--color-accent: #YOUR_NEW_COLOR;
```

## 🎭 Brand Voice

**Tone**: Professional, trustworthy, mission-driven, ethical

**Key Phrases**:
- "Responsible discovery"
- "Ethical exploration"
- "Heritage preservation"
- "Privacy-first"
- "Community-driven"

**Avoid**:
- "AI-powered signal detection"
- "Treasure hunting"
- "Get rich quick"
- Technical jargon without context

## 📞 Support

**Email**: hello@aureallabs.com  
**Location**: Gainesville, Florida, USA  
**Company**: Aureal Labs LLC

---

**Version**: 2.0 (Mission-focused redesign)  
**Last Updated**: October 27, 2025  
**Status**: Ready for deployment  
**Estimated Deploy Time**: 30-45 minutes including DNS

🚀 **Ready to launch!** Follow DEPLOYMENT_GUIDE.md for step-by-step instructions.
