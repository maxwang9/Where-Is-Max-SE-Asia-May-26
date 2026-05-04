# 2026 Southeast Asia Travel Tracker

A beautiful, interactive travel tracking website for Max & Emily's Singapore & Thailand adventure (May 6-16, 2026).

## Features

- **Live World Clocks**: Real-time clocks showing time in 5 locations (New York, San Francisco, Manila, Singapore, Bangkok)
- **Interactive Map**: Leaflet.js-powered map with clickable flight paths and custom airport markers
- **Boarding Pass Style**: Flight tickets styled as realistic boarding passes with perforated edges
- **Hotel & Boat Transfers**: Beautifully styled cards for accommodations and transfers
- **Flight Tracking Links**: Direct links to FlightAware for real-time flight tracking
- **Smooth Flight Paths**: Bezier-curve flight paths that follow realistic great circle routes

## Mobile Optimization

**This website is fully responsive and optimized for mobile devices!**

### Responsive Breakpoints:
- **Desktop**: > 1024px (full layout with all features)
- **Tablet**: 768px - 1024px (adjusted grid layouts, 2-column details)
- **Mobile**: 480px - 768px (single column, stacked layouts, readable text)
- **Small Phones**: < 480px (optimized for smaller screens, compact spacing)

### Mobile Features:
- ✅ Responsive typography that scales appropriately
- ✅ Touch-friendly buttons and links
- ✅ Single-column boarding pass layouts
- ✅ Vertical airport route displays
- ✅ Optimized map height for mobile screens
- ✅ Readable clock displays on small screens
- ✅ Proper spacing and padding for touch interactions

## Technology Stack

- **HTML5** - Semantic markup
- **CSS3** - Modern responsive design with media queries
- **JavaScript (Vanilla)** - No frameworks needed
- **Leaflet.js** - Interactive mapping library
- **OpenStreetMap** - Map tile provider

## File Structure

```
2026 Southeast Asia Travel Tracker/
├── index.html          # Main website file (self-contained)
└── README.md          # This file
```

## Testing on Mobile

### Option 1: Local Web Server (Recommended)
```bash
# Navigate to the project directory
cd "C:\Users\maxjwang\Documents\Projects\2026 Southeast Asia Travel Tracker"

# Start Python HTTP server
python -m http.server 8000

# Find your computer's IP address
ipconfig

# On your phone (same WiFi), navigate to:
# http://[YOUR-IP]:8000/index.html
```

### Option 2: GitHub Pages
1. Push to GitHub repository
2. Enable GitHub Pages in settings
3. Access via: `https://[username].github.io/[repo]/index.html`

### Option 3: Direct File Opening
Simply open `index.html` in any modern browser on your phone.

## Future Updates - Mobile-First Principles

**IMPORTANT**: When making future updates to this project, always ensure mobile compatibility:

1. **Test at multiple breakpoints**: 480px, 768px, 1024px, and desktop
2. **Touch targets**: Ensure buttons and links are at least 44x44px
3. **Font sizes**: Never go below 14px for body text on mobile
4. **Images**: Always use responsive images with proper loading
5. **Avoid horizontal scrolling**: Test on actual mobile devices
6. **Performance**: Keep the site lightweight and fast-loading

### Adding New Sections

When adding new content, always include mobile styles:

```css
/* Desktop styles first */
.new-section {
    padding: 80px 20px;
    font-size: 1.5em;
}

/* Tablet adjustments */
@media (max-width: 1024px) {
    .new-section {
        font-size: 1.3em;
    }
}

/* Mobile adjustments */
@media (max-width: 768px) {
    .new-section {
        padding: 50px 15px;
        font-size: 1.1em;
    }
}

/* Small phone adjustments */
@media (max-width: 480px) {
    .new-section {
        padding: 40px 12px;
        font-size: 1em;
    }
}
```

## Browser Compatibility

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile Safari (iOS)
- ✅ Chrome Mobile (Android)

## Performance

- Single HTML file: ~115KB (uncompressed)
- External dependencies: Leaflet.js CDN + OpenStreetMap tiles
- Live clocks update every second
- Map loads on demand

## License

Personal project - All rights reserved

## Contact

Created for Max & Emily's 2026 Southeast Asia Adventure
