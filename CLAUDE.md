# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the "AI på Arbejde" (AI at Work) website repository - a promotional website for the book by the same name. The site features the three authors and provides information about the book.

## Development Commands

```bash
# Start development server
npm run start
# or
npm run dev
# or 
npm run serve

# Build for production
npm run build

# Clean build directory
npm run clean
```

The development server runs on http://localhost:8000 using Python's built-in HTTP server.

## Project Structure

```
├── index.html          # Main website page
├── styles/
│   └── main.css        # All styling and responsive design
├── scripts/
│   └── main.js         # Interactive functionality and smooth scrolling
├── *.JPG               # Author photos (C Hendriksen, M Friis Hau, S Zambach)
├── package.json        # Project configuration and scripts
└── README.md          # Basic project info
```

## Architecture Notes

- **Static Website**: Pure HTML/CSS/JavaScript with no build tools or frameworks
- **Responsive Design**: Mobile-first approach with CSS Grid and Flexbox
- **Danish Language**: All content is in Danish as the book targets Danish readers
- **Author Integration**: Displays the three authors with their provided photos
- **Smooth Interactions**: JavaScript handles smooth scrolling and button animations

## Key Features

- Sticky navigation with auto-hide on scroll
- Smooth scrolling between sections
- Responsive author grid
- Button ripple effects
- Modern CSS with gradients and shadows