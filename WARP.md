# WARP.md

This file provides guidance to WARP (warp.dev) when working with code in this repository.

## Project Overview

This is a static website project showcasing a Roller Derby theme using Bootstrap 5. The site is a single-page application with smooth scrolling navigation and modern Bootstrap components.

### Architecture

- **Frontend Framework**: Bootstrap 5.3.3 (via CDN)
- **Icons**: Bootstrap Icons 1.11.3
- **Structure**: Single HTML file with external CSS
- **Deployment**: Static hosting ready (no build process required)

### Key Files

- `index.html` - Main HTML file containing all page content and structure
- `style.css` - Custom CSS overrides and hero section styling

## Common Development Commands

Since this is a static site, there are no build tools or package managers. Development is straightforward:

### Local Development
```bash
# Serve the site locally using Python's built-in server
python3 -m http.server 8000

# Or using Node.js (if installed)
npx http-server

# Or using PHP (if installed)
php -S localhost:8000
```

### Deployment
The site can be deployed to any static hosting service by uploading the files directly.

## Code Structure

### HTML Structure
The site uses Bootstrap's standard layout patterns:
- Fixed navbar with smooth scrolling links
- Full-height hero section with background image overlay
- Bootstrap grid system for responsive layouts
- Card components for team member profiles
- Standard footer

### CSS Organization
- Custom CSS is minimal and focused on the hero section
- Uses CSS custom properties for color theming
- Smooth scroll behavior is enabled globally
- Bootstrap classes handle most styling

### Bootstrap Components Used
- Navbar with collapse functionality
- Cards for team member profiles
- Grid system for responsive layout
- Buttons with custom color variants
- Image utilities for gallery

## Development Notes

### Adding Content
- New sections should follow Bootstrap's container > row > column pattern
- Maintain the existing scroll-margin-top for proper navbar offset
- Use semantic HTML5 elements (section, header, footer)

### Styling Guidelines
- Keep custom CSS minimal - leverage Bootstrap classes first
- Use Bootstrap's utility classes for spacing and positioning
- Maintain the existing color scheme (reds and dark grays)
- Ensure responsive design principles are followed

### Image Assets
- Currently uses external image URLs (Pexels, archive.org)
- For production, consider hosting images locally
- Maintain aspect ratios for card images (approximately 4:3)
- Use appropriate alt text for accessibility