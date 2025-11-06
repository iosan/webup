# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.5.0] - 2025-11-06

### Added
- Fixed top navigation bar that stays visible while scrolling
- Button-style navigation menu with modern hover effects and borders
- Dropdown menu for Projects with links to all 5 project detail pages
- Active page indicator in navigation (highlights current page)
- Responsive design with tablet (≤768px) and mobile (≤480px) breakpoints
- Scaled navigation, typography, and images for smaller screens
- Navigation logo resized to 32px in nav bar (28px tablet, 24px mobile)
- Smooth transitions for dropdown menu (opacity, visibility)
- Triple-layer dropdown hiding (display, visibility, opacity)
- ARIA attributes for dropdown accessibility (aria-haspopup, aria-expanded)
- Focus-within support for keyboard navigation of dropdown
- Responsive header margins that match navigation height at each breakpoint
- Responsive gallery images (250px → 180px → 140px)
- Comprehensive responsive design documentation with visual screenshots
- SVG screenshots showing desktop, tablet, and mobile layouts
- `docs/responsive-design.adoc` - Complete responsive design guide
- `docs/screenshots/` directory with layout visualizations
- 2-column auto-fit gallery grid for tablet devices
- Single-column centered gallery for mobile devices
- Mobile-specific optimizations (no rotation, right-aligned dropdown)
- W3C validator badges in footer (HTML5 and CSS3)
- Architecture diagrams (7 PlantUML diagrams)
- Build automation via Makefile
- Learning guide with curated HTML5/CSS resources
- Comprehensive documentation in AsciiDoc format

### Changed
- Moved logo from header to navigation bar (left side)
- Simplified header to centered title only (no logo or navigation)
- Changed footer from fixed to scrolling naturally with content
- Navigation now uses flexbox for logo and menu alignment
- Menu items styled as buttons instead of plain links
- Header margin-top adjusts per breakpoint (48px → 40px → 32px)
- Image boxes scale down on tablet and mobile with reduced padding
- Gallery gap reduces on smaller screens (40px → 30px → 20px)
- Typography scales down at mobile and tablet sizes
- Validator badges stack vertically on mobile, wrap on tablet
- Navigation gaps optimize per device (15px → 8px → 4px)
- Button padding scales responsively (8/16px → 6/12px → 5/8px)
- Content padding optimized for mobile (reduced to 10px)
- List padding-left reduced to 20px on mobile
- Dropdown menu right-aligned on mobile to prevent overflow
- Gallery uses CSS Grid with auto-fit for flexible columns
- Rotation effects disabled on mobile for cleaner appearance
- Hover effects simplified to scale(1.02) on mobile
- Semantic HTML improvement: Changed gallery from article to figure/figcaption

### Fixed
- Dropdown menu properly hidden when not hovered (multiple CSS properties)
- No gap between navigation and header on tablet/mobile sizes
- Proper keyboard navigation and focus management for dropdown
- Menu items no longer wrap or overflow on small screens
- Dropdown positioning stays within viewport bounds
- Image gallery properly centers on all screen sizes
- HTML5 validation errors (article without heading → figure)

## [0.1.0] - 2025-11-06

### Added
- Initial release of WebUp Industrial Engineering website
- Homepage with 5-project gallery featuring paper shadows and rotation effects
- About, Contact, and Impressum pages
- Individual project detail pages with watermarked backgrounds
- Dark sepia theme for professional industrial aesthetics
- Responsive design for all devices
- Custom gear logo and favicon
- Full accessibility features with ARIA labels
- SEO optimization with meta tags and keywords
- Privacy-compliant pages excluded from search engines
- robots.txt for crawler management
- Comprehensive README.md documentation
- Organized and commented CSS structure
- Semantic HTML5 with proper accessibility attributes

### Notes
- Placeholder images must be replaced with properly licensed images before commercial use
- All HTML pages include proper meta tags for SEO and accessibility
- Three pages (about.html, contact.html, impressum.html) excluded from search engines

[0.5.0]: https://github.com/iosan/webup/releases/tag/v0.5.0
[0.1.0]: https://github.com/iosan/webup/releases/tag/v0.1.0
