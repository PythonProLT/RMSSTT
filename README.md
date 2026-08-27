# Roosevelt Middle School — Chromebook Student Guide

A professional, multi-section student guide website for Roosevelt Middle School,
covering everything students need to know about using their school Chromebooks.

## Sections Covered
- Getting Started (login, shelf, launcher, special keys)
- Keyboard Languages (switching input methods)
- Accessibility & ChromeVOX (screen reader + all accessibility tools)
- Keyboard Shortcuts (browser, editing, system, screenshots)
- Special Features & Built-In Apps
- Google Workspace: Docs, Slides, Sheets, Forms, Sites, Drawings
- Student Platforms: Clever, Google Classroom, Gmail, Khan Academy, Student Connect, TCI
- Care, Cleaning & Charging Tips
- Quick Reference Card

## Deploying to GitHub Pages

1. Create a new GitHub repository (e.g., `rms-chromebook-guide`)
2. Upload all files from this folder to the repository root
3. Go to **Settings → Pages**
4. Under *Source*, select `main` branch and `/ (root)` folder
5. Click Save — your site will be live at:
   `https://your-username.github.io/rms-chromebook-guide/`

## Customizing Colors

All colors are defined as CSS variables at the top of `css/style.css`.
To change the primary red, update:
```css
--red:      #C41230;
--red-dark: #9B0E24;
```

## Adding School Photos

Replace the hero section background or add an `<img>` inside `.hero-inner`
in `index.html`. Recommended: a banner-style photo of students using Chromebooks,
or the school building/logo.

## Adding the School Logo

Place your logo image in the `assets/` folder, then in `index.html` replace
the `.brand-badge` div:
```html
<img src="assets/rms-logo.png" alt="Roosevelt Middle School" class="brand-logo" />
```
And add in `css/style.css`:
```css
.brand-logo { height: 44px; width: auto; }
```
