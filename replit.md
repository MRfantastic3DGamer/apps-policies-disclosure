# Fit Empire Legal & Policy Website

## Overview
This is a static HTML website that hosts legal documentation for the Fit Empire fitness center management Android application. The website provides comprehensive policy pages required for Google Play Store publishing.

**Pages:**
- Homepage with modern gradient design and card-based navigation
- Privacy Policy with detailed data handling information
- Terms of Service with comprehensive legal terms

**Current State:** Fully functional and ready for deployment. All pages are Play Store compliant.

## Recent Changes
- **November 10, 2025:** Enhanced website for Android app publishing
  - Improved markdown formatting in Privacy Policy with proper sections, bullet points, and horizontal rules
  - Created comprehensive Terms of Service page with Play Store-compliant sections:
    * Detailed service description with all app features
    * Explicit warranties and disclaimers (including mobile compatibility)
    * Medical and health disclaimers
    * Comprehensive liability limitations
    * Structured dispute resolution process (India jurisdiction)
    * Enhanced contact information with categorized support
  - Redesigned homepage with gradient background and professional card layout
  - All pages tested and verified to render correctly
  
- **November 10, 2025:** Initial Replit setup completed
  - Configured Python HTTP server for static file serving
  - Set up workflow to run on port 5000
  - Configured deployment settings for production
  - Added .gitignore for Python

## Project Structure
```
.
├── index.html                        # Homepage with gradient design and card navigation
├── fit_empire_data_safty.html       # Privacy policy page (Play Store compliant)
├── terms_of_service.html            # Terms of Service page (Play Store compliant)
├── .gitignore                        # Python gitignore
└── replit.md                         # This file
```

## Technology Stack
- **Frontend:** Pure HTML, CSS (inline and Tailwind CDN), JavaScript
- **Server:** Python 3.11 built-in HTTP server
- **Dependencies:** 
  - Tailwind CSS (via CDN)
  - Marked.js (Markdown parser, via CDN)

## Local Development
The website runs on port 5000 using Python's built-in HTTP server:
```bash
python -m http.server 5000 --bind 0.0.0.0
```

The workflow is configured to automatically start the server when the project runs.

## Pages
1. **Homepage (index.html):** Modern landing page with gradient background and card-based navigation to both policy pages
2. **Privacy Policy (fit_empire_data_safty.html):** Comprehensive privacy policy with improved markdown formatting, proper sections, and bullet points
3. **Terms of Service (terms_of_service.html):** Play Store-compliant legal terms covering service description, warranties, disclaimers, liability, dispute resolution, and contact information

## Deployment
Configured for Replit Autoscale deployment with the following settings:
- Deployment type: Autoscale (stateless website)
- Run command: `python -m http.server 5000 --bind 0.0.0.0`
- Port: 5000

## Notes
- This is a static website with no backend or database
- All styling is embedded in HTML files
- External dependencies (Tailwind, Marked.js) are loaded via CDN
- The privacy policy content is stored in a template tag and rendered client-side
