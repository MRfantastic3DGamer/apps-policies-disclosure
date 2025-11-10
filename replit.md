# Fit Empire Privacy Policy Website

## Overview
This is a simple static HTML website that hosts privacy policy and data security documentation for the Fit Empire fitness center management application. The website consists of two pages:
- Homepage with navigation
- Privacy policy page with detailed data handling information

**Current State:** Fully functional and ready for deployment

## Recent Changes
- **November 10, 2025:** Initial Replit setup completed
  - Configured Python HTTP server for static file serving
  - Set up workflow to run on port 5000
  - Configured deployment settings for production
  - Added .gitignore for Python

## Project Structure
```
.
├── index.html                        # Homepage with navigation
├── fit_empire_data_safty.html       # Privacy policy page
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
1. **Homepage (index.html):** Simple landing page with clean styling and link to privacy policy
2. **Privacy Policy (fit_empire_data_safty.html):** Detailed privacy policy using Markdown content rendered with Marked.js

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
