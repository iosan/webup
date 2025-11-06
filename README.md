# 🌐 WebUp Industrial Engineering

> A modern, responsive HTML5 website showcasing industrial metal engineering, fabrication, and CNC machining projects with elegant design and accessibility features.

![Version](https://img.shields.io/badge/version-0.1.0-blue.svg)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![SEO Optimized](https://img.shields.io/badge/SEO-Optimized-green.svg)
![Accessibility](https://img.shields.io/badge/A11y-WCAG-blue.svg)

---

## ✨ Features

- 🎨 **Modern Design** - Clean HTML5 structure with semantic elements and ARIA labels
- 📱 **Responsive Layout** - Works seamlessly across different screen sizes
- 🖼️ **Interactive Gallery** - 5 metal engineering projects with paper shadow effects and rotation
- 🔗 **Multi-Page Navigation** - Home, About, Contact, Impressum, and individual project detail pages
- ⚙️ **Custom Branding** - Gear logo with favicon support
- 🎭 **Watermarked Backgrounds** - Beautiful project images as backgrounds on detail pages
- 🎨 **Dark Sepia Theme** - Warm, earthy color scheme for professional industrial look
- ♿ **Accessibility** - ARIA labels, semantic HTML, and keyboard navigation support
- 🔍 **SEO Optimized** - Meta descriptions, keywords, and proper heading structure
- 🔒 **Privacy Compliant** - About, Contact, and Impressum pages excluded from search engines
- 🤖 **Crawler Control** - robots.txt for search engine management

---

## 📂 Project Structure

```
webup/
├── 📄 README.md
└── 📁 html/
    ├── 🏠 index.html           # Homepage with project gallery
    ├── 📖 about.html            # About page (excluded from search)
    ├── 📧 contact.html          # Contact page (excluded from search)
    ├── ⚖️ impressum.html        # Legal notice (excluded from search)
    ├── 🖼️ image1.html           # Project detail page 1
    ├── 🖼️ image2.html           # Project detail page 2
    ├── 🖼️ image3.html           # Project detail page 3
    ├── 🖼️ image4.html           # Project detail page 4
    ├── 🖼️ image5.html           # Project detail page 5
    ├── 🤖 robots.txt            # Web crawler control file
    ├── 📁 css/
    │   └── 🎨 style.css         # Main stylesheet (beautified & organized)
    └── 📁 images/
        ├── ⚙️ gear.ico          # Browser favicon
        ├── ⚙️ gear.png          # Site logo (80x80px)
        ├── 🖼️ metal1.jpg        # Gallery image 1
        ├── 🖼️ metal2.jpg        # Gallery image 2
        ├── 🖼️ metal3.jpg        # Gallery image 3
        ├── 🖼️ metal4.jpg        # Gallery image 4
        └── 🖼️ metal5.jpg        # Gallery image 5
```

---

## 🚀 Getting Started

### ⚠️ Important: Image Licensing

**The current images in the `html/images/` folder are placeholders and must be replaced before commercial use.**

- Replace `metal1.jpg` through `metal5.jpg` with your own photos or properly licensed images
- Ensure you have the rights to use all images on your website
- Consider using:
  - Your own photography of projects/machinery
  - Licensed stock photos (Shutterstock, Adobe Stock, Getty Images)
  - Free stock photos with proper attribution (Unsplash, Pexels, Pixabay)
- Document image sources and keep license receipts
- Add attribution if required by the license

**Failure to use properly licensed images may result in copyright infringement issues.**

---

### Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/iosan/webup.git
   cd webup
   ```

2. **Open in browser**
   ```bash
   # Simply open the index.html file
   open html/index.html
   # or on Linux
   xdg-open html/index.html
   # or on Windows
   start html/index.html
   ```

3. **That's it!** No build process or dependencies required. 🎉

### Development

For local development with live reload, you can use any simple HTTP server:

```bash
# Python 3
cd html && python -m http.server 8000

# Node.js (with http-server installed)
cd html && npx http-server -p 8000

# PHP
cd html && php -S localhost:8000
```

Then open `http://localhost:8000` in your browser.

---

## 🎨 Customization

### Change Colors

Edit `html/css/style.css` to modify the color scheme:

```css
/* Header and Footer - Dark Sepia Theme */
header, footer {
    background-color: #3d2f21;  /* Change to your preferred color */
}

/* Content Background */
.content {
    background-color: #f4f4f4;  /* Light background - customize as needed */
}
```

### Replace Images

**⚠️ IMPORTANT: Replace placeholder images before publishing**

1. Add your own images or properly licensed images to `html/images/`
2. Use the same filenames (`metal1.jpg` through `metal5.jpg`) or update references
3. Update the image references in `html/index.html` if needed
4. Ensure image names match in the corresponding `imageX.html` pages
5. Recommended size: 250x250px or larger (maintains aspect ratio with `object-fit: cover`)
6. Keep documentation of image sources and licenses

**Image Sources:**
- Take your own photos (you own the copyright)
- Purchase from stock sites (Shutterstock, Adobe Stock, Getty Images)
- Use free stock photos (Unsplash, Pexels, Pixabay)
- Ensure proper licensing for commercial use

### Update Company Information

Edit the **Impressum page** (`html/impressum.html`) with your actual company details:
- Company name and address
- Contact information
- Legal representatives
- VAT ID and registration numbers

### Modify SEO

Update meta tags in each HTML file:
```html
<meta name="description" content="Your custom description">
<meta name="keywords" content="metal, steel, industrial, machinery, engineering, fabrication, cnc">
```

---

## 🎯 Key Features Explained

### 📸 Interactive Project Gallery
- 5 projects displayed with paper-like shadow effects
- Each image rotates slightly toward the center for visual interest
- Smooth hover effects with scale and rotation
- Click images to view detailed project pages with watermarked backgrounds

### 🎨 Professional Styling
- **Header**: Dark sepia background with fixed gear logo
- **Content**: Flexible layout with clean typography
- **Footer**: Fixed at bottom of viewport with impressum link
- **Navigation**: Responsive menu with hover effects and ARIA labels

### ♿ Accessibility Features
- Semantic HTML5 elements (`<header>`, `<nav>`, `<main>`, `<article>`, `<section>`, `<footer>`)
- ARIA labels for navigation and links
- `aria-current="page"` for current page indication
- Descriptive alt text for all images
- Keyboard navigation support

### 🔍 SEO Optimization
- Unique meta descriptions for each page
- Targeted keywords (metal, steel, industrial, machinery, engineering, fabrication, cnc)
- Proper heading hierarchy (H1, H2, H3)
- Author meta tags
- Structured content with semantic elements

### 🔒 Privacy & Legal Compliance
- Impressum page with complete legal notice template
- About and Contact pages excluded from search engines for privacy
- Excluded from search engines via:
  - Meta robots tags (`noindex, nofollow, noarchive, nosnippet`)
  - robots.txt configuration
- Accessible via footer link (Impressum) and navigation (About, Contact) on all pages

### 🔗 Navigation Structure
```
Home (index.html)
├── About (about.html) [excluded from search]
├── Contact (contact.html) [excluded from search]
├── Impressum (impressum.html) [excluded from search]
├── Project 1 Detail (image1.html) [with watermark]
├── Project 2 Detail (image2.html) [with watermark]
├── Project 3 Detail (image3.html) [with watermark]
├── Project 4 Detail (image4.html) [with watermark]
└── Project 5 Detail (image5.html) [with watermark]
```

---

## 📋 Browser Support

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Opera (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

---

## 🛠️ Technical Details

### CSS Organization
The stylesheet is organized into clear sections:
- Global Styles
- Header Styles
- Logo Styles
- Navigation Styles
- Content Area Styles
- Watermark Background Styles
- Image Gallery Styles
- Footer Styles

### HTML5 Best Practices
- Valid DOCTYPE declaration
- Proper meta tags for character encoding and viewport
- Semantic HTML elements
- ARIA accessibility attributes
- Organized head section with comments
- Clean code structure with proper indentation

---

## 📝 Version History

### v0.1.0 (Current - November 2025)
- ✨ Initial release
- 🎨 Dark sepia theme with warm industrial aesthetics
- 🖼️ 5-project gallery with paper shadows and rotation effects
- 📱 Responsive design for all devices
- ⚙️ Custom gear logo and favicon
- ♿ Full accessibility features with ARIA labels
- 🔍 SEO optimized with meta tags and keywords
- 🔒 Privacy-compliant pages (About, Contact, Impressum excluded from search)
- 🤖 robots.txt for crawler management
- 🎭 Watermarked backgrounds on project detail pages
- 📚 Comprehensive documentation
- ⚠️ **Note**: Placeholder images must be replaced with properly licensed images before commercial use

---

## 📄 License

This project is open source and available for personal and commercial use.

---

## 👤 Author

**iosan**

- GitHub: [@iosan](https://github.com/iosan)
- Repository: [webup](https://github.com/iosan/webup)

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

Feel free to check the [issues page](https://github.com/iosan/webup/issues) if you want to contribute.

### Development Guidelines
1. Maintain semantic HTML structure
2. Keep accessibility features intact
3. Follow the existing code organization
4. Test across multiple browsers
5. Update documentation as needed

---

## 🙏 Acknowledgments

- Design inspired by modern industrial aesthetics
- Paper shadow effects for engaging visual presentation
- Focus on accessibility and web standards compliance

---

<div align="center">
  <p>Made with ❤️ and ⚙️ by iosan</p>
  <p>⭐️ Star this repo if you like it!</p>
  <p><strong>WebUp Industrial Engineering</strong> - Precision. Quality. Innovation.</p>
</div>

