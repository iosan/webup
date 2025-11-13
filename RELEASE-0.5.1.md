# WebUp v0.5.1 Release Notes

**Release Date:** November 13, 2025  
**Release Type:** Patch Release  
**Previous Version:** 0.5.0

---

## 🎉 What's New in v0.5.1

This patch release adds GitHub Actions workflows for automated deployment and continuous integration, fixing build and deployment issues.

### 🚀 GitHub Actions Integration

#### Automated Deployment Workflow
- **GitHub Pages**: Automatic deployment to gh-pages branch
- **peaceiris/actions-gh-pages**: Reliable deployment action
- **Simple Setup**: Deploy from branch configuration
- **Push to Deploy**: Automatic on master/main branch updates

#### Documentation Build Workflow
- **Ruby Setup**: Proper gem installation in user space
- **PlantUML & Graphviz**: Automated diagram generation
- **AsciiDoc PDFs**: Automatic PDF documentation build
- **Artifact Upload**: Generated files available for download

#### Bug Fixes
- ✅ Fixed `./configure` error by removing incorrect makefile.yml
- ✅ Fixed gem permissions error with --user-install flag
- ✅ Simplified deployment workflow for reliability
- ✅ Added proper Ruby environment setup

### 📚 Documentation Updates
- **README.md**: Added GitHub Actions & Deployment section
- **deployment.adoc**: Updated with new workflow instructions
- **.github/README.md**: Created workflow documentation
- **Project Structure**: Added .github/ directory to documentation

---

## 🎉 Features from v0.5.0

### 🧭 Navigation System Overhaul

#### Fixed Top Navigation Bar
- **Always Visible**: Navigation stays at the top while scrolling
- **Compact Logo**: 32px gear logo positioned on the left
- **Flexbox Layout**: Responsive alignment with centered menu items
- **Smart Positioning**: Fixed z-index: 1000 with proper shadow

#### Button-Style Menu
- **Modern Design**: Links styled as interactive buttons
- **Hover Effects**: Semi-transparent background on hover
- **Border Styling**: Subtle borders with rounded corners (4px)
- **Focus States**: Accessible keyboard navigation with visible outlines
- **Active Indicators**: Current page highlighted with background

#### Dropdown Menu
- **Project Navigation**: "Projects ▾" dropdown with all 5 project links
- **Smart Hiding**: Triple-layer (display, visibility, opacity)
- **Smooth Transitions**: Fade-in animation (0.3s)
- **Hover Activation**: Works with mouse and keyboard (focus-within)
- **Accessibility**: ARIA attributes (aria-haspopup, aria-expanded)
- **Mobile Optimization**: Right-aligned to prevent overflow

### 📱 Responsive Design System

#### Three Optimized Breakpoints
1. **Desktop (>768px)**: Full experience
2. **Tablet (≤768px)**: Optimized for medium screens
3. **Mobile (≤480px)**: Compact mobile layout

#### Desktop Layout (>768px)
- 32px navigation logo
- 48px header margin
- 250px gallery images with rotation effects
- Multi-column flexible grid
- 40px gallery gaps
- Full typography

#### Tablet Layout (≤768px)
- 28px navigation logo (reduced)
- 40px header margin (reduced)
- 180px gallery images
- 2-column auto-fit CSS Grid
- 30px gallery gaps
- 95% typography scale
- Wrapped footer badges

#### Mobile Layout (≤480px)
- 24px navigation logo (minimal)
- 32px header margin (minimal)
- 140px gallery images
- Single-column centered layout
- 20px gallery gaps
- 70-85% typography scale
- No rotation effects (cleaner)
- Right-aligned dropdown
- Stacked footer badges
- Simplified hover (scale only)

### 📊 Layout Improvements

#### Header Restructure
- **Before**: Logo + title + navigation in header
- **After**: Clean centered title only
- **Logo Moved**: To navigation bar (left side)
- **Navigation Moved**: To fixed top bar
- **Result**: Cleaner, more focused header

#### Footer Changes
- **Before**: Fixed position at bottom
- **After**: Scrolls naturally with content
- **Badges**: Horizontal on desktop, vertical on mobile
- **Spacing**: Optimized per breakpoint

#### Gallery Enhancements
- **CSS Grid**: Auto-fit for flexible columns
- **Responsive Sizing**: 250px → 180px → 140px
- **Centered Layout**: Proper alignment on all screens
- **Mobile Optimization**: Single column, no rotation
- **Tablet Optimization**: 2 columns with justify-content

### 📚 Documentation Expansion

#### New Documents
- **responsive-design.adoc**: Complete 400+ line guide
  - Breakpoint specifications
  - Size comparison tables
  - CSS code examples
  - Testing checklist
  - Browser compatibility
  - Performance tips

#### Visual Documentation
- **desktop-layout.svg**: 1200×800px mockup
- **tablet-layout.svg**: 768×1024px mockup
- **mobile-layout.svg**: 375×667px mockup
- **screenshots/**: New directory for visuals

#### Updated Documents
- **README.md**: Responsive design section
- **docs/index.adoc**: Navigation system docs
- **docs/README.adoc**: Document index updated
- **docs/quick-reference.adoc**: Responsive tables
- **CHANGELOG.md**: Complete change history
- **humans.txt**: Feature list updated

### ♿ Accessibility Enhancements

- **ARIA Attributes**: Added for dropdown menu
- **Keyboard Navigation**: Full support with focus-within
- **Focus States**: Visible outlines on all interactive elements
- **Active Page**: aria-current="page" for current location
- **Screen Readers**: Proper semantic HTML (figure/figcaption)
- **Touch Targets**: Maintained adequate sizes (44×44px minimum)

### 🎨 CSS Improvements

#### Variables System
- Centralized theme configuration
- Easy color/spacing customization
- Responsive scaling built-in

#### Modern Techniques
- Flexbox for navigation
- CSS Grid for gallery
- Media queries (2 breakpoints)
- Hardware-accelerated transforms
- Smooth transitions

#### Mobile-Specific
```css
/* Disabled rotation for cleaner mobile look */
.rotate-* { transform: rotate(0deg) !important; }

/* Right-aligned dropdown */
.dropdown-menu { left: auto; right: 0; }

/* No-wrap menus */
.top-nav ul { flex-wrap: nowrap; }
.nav-button { white-space: nowrap; }
```

### 🐛 Bug Fixes

- ✅ Dropdown properly hidden when not hovered
- ✅ No gap between nav and header on small screens
- ✅ Menu items don't wrap or overflow
- ✅ Dropdown stays within viewport
- ✅ Gallery properly centered
- ✅ Semantic HTML validation (article → figure)

### 📈 Performance

- **CSS-Only**: No JavaScript for responsiveness
- **Single Stylesheet**: All breakpoints in one file
- **GPU Acceleration**: Transform properties optimized
- **Minimal Reflows**: Targeted CSS changes
- **Optimized Images**: Proper sizing per breakpoint

---

## 📦 What's Included

### Core Files
- ✅ 9 HTML pages (all updated)
- ✅ Enhanced CSS with responsive queries
- ✅ SVG validator badges
- ✅ Architecture diagrams (7 PlantUML)

### Documentation
- ✅ 8 AsciiDoc guides (all updated to v0.5.1)
- ✅ 3 SVG layout screenshots
- ✅ Makefile for automation
- ✅ Complete API/reference docs
- ✅ GitHub Actions workflows documentation

### Assets
- ✅ 32px responsive logo
- ✅ Favicon (gear.ico)
- ✅ Placeholder images (metal1-5.jpg)
- ✅ Validator badges (SVG)

---

## 🚀 Upgrade Guide

### From v0.5.0 to v0.5.1

#### Automatic (Full Update)
```bash
git pull origin v0.5.1
```

#### What Changed
1. **Added .github/workflows/**: New GitHub Actions workflows
2. **Updated README.md**: Added deployment instructions
3. **Updated deployment.adoc**: New workflow documentation
4. **Fixed build issues**: Ruby gem permissions resolved

### From v0.1.0 to v0.5.1

#### Automatic (Full Update)
```bash
git pull origin v0.5.1
```

#### Manual (Review Changes First)
1. **Backup current version**
2. **Update HTML files**: Navigation structure changed
3. **Update CSS**: New responsive media queries
4. **Update docs**: All version numbers changed
5. **Test responsive layouts**: Desktop, tablet, mobile

#### Breaking Changes
⚠️ **Navigation HTML Structure**: If you customized navigation, update to new structure with dropdown menu

⚠️ **CSS Classes**: New classes added (.nav-button, .dropdown, .dropdown-menu)

⚠️ **Footer Position**: Changed from fixed to scrolling (adjust custom CSS if needed)

---

## 🧪 Testing

### Browser Compatibility
- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+
- ✅ Mobile Safari iOS 12+
- ✅ Chrome Mobile Android 8+

### Device Testing
- ✅ Desktop (1920×1080, 1366×768)
- ✅ Tablet (768×1024, 1024×1366)
- ✅ Mobile (375×667, 390×844)

### Validation
- ✅ W3C HTML5 Validator: No errors
- ✅ W3C CSS3 Validator: Valid (warnings for CSS variables only)
- ✅ WCAG Accessibility: Compliant

---

## 📖 Documentation

All documentation updated to v0.5.1:

1. **[Main Documentation](docs/index.adoc)** - Complete guide
2. **[Responsive Design Guide](docs/responsive-design.adoc)** - NEW!
3. **[Theming Guide](docs/theming.adoc)** - CSS customization
4. **[Deployment Guide](docs/deployment.adoc)** - Hosting instructions
5. **[Quick Reference](docs/quick-reference.adoc)** - Fast lookup
6. **[Learning Guide](docs/learning.adoc)** - HTML5/CSS resources
7. **[Architecture Diagrams](docs/diagrams.adoc)** - Visual gallery
8. **[Build Instructions](docs/BUILD.adoc)** - Automation guide

---

## 🎯 Migration Checklist

- [ ] Backup current version
- [ ] Update to v0.5.0
- [ ] Test desktop layout (>768px)
- [ ] Test tablet layout (≤768px)
- [ ] Test mobile layout (≤480px)
- [ ] Verify navigation dropdown works
- [ ] Check active page indicators
- [ ] Test keyboard navigation
- [ ] Validate HTML/CSS
- [ ] Review documentation
- [ ] Update custom modifications

---

## 🔜 Future Roadmap

Potential enhancements for future versions:

1. **Container Queries**: Component-level responsiveness
2. **Responsive Images**: srcset/picture elements
3. **Dark Mode**: prefers-color-scheme support
4. **Print Styles**: Optimized @media print
5. **Reduced Motion**: prefers-reduced-motion support
6. **Landscape Modes**: Specific mobile landscape styles
7. **High DPI**: Retina/HiDPI alternatives

---

## 🙏 Acknowledgments

Thanks to:
- W3C for standards and validators
- PlantUML for diagram generation
- AsciiDoc for documentation
- Open source community for inspiration

---

## 📝 License

MIT License - See [LICENSE](LICENSE) file for details

⚠️ **Image Licensing**: Placeholder images must be replaced with properly licensed images before commercial use.

---

## 🤝 Contributing

Contributions welcome! See [CONTRIBUTING.md](CONTRIBUTING.md)

---

## 📧 Support

- **Issues**: https://github.com/iosan/webup/issues
- **Repository**: https://github.com/iosan/webup
- **Branch**: v0.5.1

---

<div align="center">

**WebUp v0.5.1** - Responsive. Modern. Accessible. Automated.

Made with ❤️ and ⚙️ by [iosan](https://github.com/iosan)

⭐ Star this repo if you like it!

</div>
