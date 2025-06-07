# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a personal portfolio website built with vanilla HTML, CSS, and JavaScript. It features a modern, responsive design with dark/light theme support and includes both a main landing page and an about page.

## Architecture

### Core Files
- `index.html` - Main portfolio page with hero, skills, projects, and contact sections
- `about.html` - Detailed about page with timeline, skills overview, and fun facts
- `style.css` - Unified CSS using CSS custom properties for theme management
- `script.js` - JavaScript for interactions, animations, and theme switching

### Dependencies
All dependencies are loaded via CDN:
- Bootstrap 5.3.3 (UI framework)
- Font Awesome 6.5.1 (icons)
- AOS 2.3.1 (scroll animations)
- Particles.js 2.0.0 (background particle effects)

### Theme System
The site uses CSS custom properties (`--primary-color`, `--bg-color`, etc.) that change based on the `data-bs-theme` attribute on the HTML element. The theme toggle persists the user's preference in localStorage.

### Navigation
Both pages share consistent navigation structure. The about page properly links back to sections on the main page using anchor tags with the page reference (`index.html#section`).

## Key Features

- **Responsive Design**: Bootstrap grid system with custom responsive breakpoints
- **Dark/Light Theme**: Toggle between themes with localStorage persistence
- **Animations**: AOS library for scroll-triggered animations, custom hover effects
- **Interactive Elements**: Particle background, typing effect, animated progress bars
- **Form Handling**: Contact form with basic validation (currently logs to console)

## Development Notes

- No build process required - static files served directly
- Images use placeholder URLs that should be replaced with actual assets
- Social links and contact form are placeholder implementations
- The site is deployed to GitHub Pages (evident from docs/CNAME file)

## Common Tasks

Since this is a static site with no build process, common development tasks involve:
- Direct file editing for content updates
- Testing changes by opening HTML files in browser
- Updating placeholder content (images, social links, project details)
- Customizing color scheme via CSS custom properties