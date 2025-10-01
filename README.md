# Miami Dubai AI Workshop - Landing Page

A clean, modern landing page for the Miami Dubai AI Workshop. Learn how small business owners are using AI to save time, increase production, and make more money.

## Features

- 🎨 **Clean Design**: Professional, minimalist aesthetic
- 📱 **Fully Responsive**: Optimized for all devices
- ⚡ **Fast Loading**: Lightweight with minimal JavaScript
- 🎬 **Video Section**: Embedded workshop preview
- 🎯 **Conversion Optimized**: Clear CTAs and registration flow
- 🚀 **GitHub Pages Ready**: Deploy in minutes

## Workshop Details

**Instructors**: Erik Ten Have & Laz Cor
**Date**: October 13, 2025 • 17:00 CET
**Format**: Free 90-minute live Zoom workshop
**Target**: Small business owners (1-250 people, $1-$24M revenue)

## Quick Start (Local Development)

1. **Clone or Download**:
```bash
cd ai-landing-page
```

2. **Start Local Server**:
```bash
# Option 1: Node.js (requires npm install first)
npm start

# Option 2: Python
python3 -m http.server 3000

# Option 3: Open directly in browser
open index.html
```

3. **Open in Browser**:
Navigate to [http://localhost:3000](http://localhost:3000)

## Deploy to GitHub Pages

**See [DEPLOY.md](DEPLOY.md) for complete deployment instructions.**

### Quick Deploy Steps:

```bash
# 1. Initialize git
git init
git add .
git commit -m "Initial commit"

# 2. Create repository on GitHub, then:
git remote add origin https://github.com/YOUR_USERNAME/ai-landing-page.git
git push -u origin main

# 3. Enable GitHub Pages in repository Settings → Pages
# Select branch: main, folder: / (root)

# Your site will be live at:
# https://YOUR_USERNAME.github.io/ai-landing-page/
```

## Project Structure

```
ai-landing-page/
├── index.html          # Main landing page (GitHub Pages serves this)
├── script.js           # JavaScript file
├── public/             # Backup/source files
│   ├── index.html
│   └── script.js
├── server.js           # Local development server (optional)
├── package.json        # Node.js config (optional)
├── DEPLOY.md          # Deployment guide
├── .gitignore         # Git ignore rules
└── README.md          # This file
```

## Page Sections

1. **Hero**: Workshop title, date, and registration CTA
2. **Value Proposition**: The AI transformation promise
3. **3 Leverage Points**: Speed, Accuracy, Output
4. **Video Preview**: Workshop demonstration
5. **What You'll Get**: Workshop outcomes and bonuses
6. **Who Should Attend**: Target audience
7. **Meet the Guides**: Erik Ten Have & Laz Cor bios
8. **One Last Reason**: Emotional connection
9. **Workshop Details**: Date, time, format, investment
10. **FAQ**: Common questions
11. **Registration CTA**: Final conversion point

## Customization

### Update Content
Edit `index.html` directly:
- Workshop dates and times
- Instructor information
- Bonuses and offerings
- Video embed URL
- Registration email/link

### Update Styles
Tailwind CSS is loaded via CDN. Modify inline styles in `<style>` tag:
```css
/* Current brand colors */
--blue: #3b9ad5, #188bf6
--green: #37ca37
```

### Update Video
Replace YouTube embed URL around line 145:
```html
<iframe src="https://www.youtube.com/embed/YOUR_VIDEO_ID" ...>
```

## Tech Stack

- **HTML5**: Semantic markup
- **Tailwind CSS**: Utility-first CSS (CDN)
- **JavaScript**: Minimal vanilla JS
- **Fonts**: Inter + Montserrat (Google Fonts)

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome)

## Performance

- Loads in < 2 seconds
- Minimal JavaScript (< 1KB)
- CDN-delivered CSS and fonts
- No external dependencies
- Optimized for Core Web Vitals

## License

MIT License - Free to use for your projects

## Support

For deployment help, see [DEPLOY.md](DEPLOY.md)
For GitHub Pages issues: [GitHub Pages Docs](https://docs.github.com/en/pages)

## Credits

**Workshop by**: Erik Ten Have & Laz Cor
**Website**: https://leverageaiforsmallbusiness.com
**Content**: All content from official workshop materials
