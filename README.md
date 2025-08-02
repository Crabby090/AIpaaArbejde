# AI på Arbejde - Website

Website for the book "AI på Arbejde" by Mark Friis Hau, Christian Hendriksen, and Sine Zambach.

## Project Overview

This is a promotional website for the book "AI på arbejde – din kritiske guide til ChatGPT og generativ AI i en dansk kontekst". The site features:

- Book overview with detailed chapter breakdown
- Author biographies and photos
- Direct links to purchase the book
- Contact information for booking workshops and presentations

## Development

### Prerequisites
- Node.js (v14 or higher)

### Local Development
```bash
# Start development server
npm run start
# or
npm run dev

# The site will be available at http://localhost:8000
```

### Build for Production
```bash
# Create production build
npm run build

# Clean build directory
npm run clean
```

## Deployment Guide (Render + Cloudflare)

### Pre-deployment Checklist
✅ SEO meta tags and Open Graph tags added  
✅ Favicon configured (using book cover)  
✅ Images optimized (162K-325K file sizes)  
✅ Render configuration (`render.yaml`) created  
✅ Redirects file (`_redirects`) configured  
✅ Build process tested and working  

### Deployment Steps

#### 1. Push to GitHub
```bash
git init
git add .
git commit -m "Initial website deployment"
git remote add origin [your-github-repo-url]
git push -u origin main
```

#### 2. Deploy on Render
- Connect your GitHub repository to Render
- Render will automatically detect the `render.yaml` configuration
- Build command: `npm run build`
- Publish directory: `dist`
- The site will be automatically deployed

#### 3. Configure Cloudflare
- Add your domain to Cloudflare
- Point your domain to Render's provided URL
- Enable Cloudflare's performance features:
  - Caching
  - Minification
  - Image optimization

#### 4. Update Domain URLs
Once you have your final domain, update the following in `index.html`:
- Lines 13, 16, 20, 23: Replace `https://aipaaarbejde.dk/` with your actual domain

### Technical Details

**Architecture**: Static website (HTML/CSS/JavaScript)  
**Responsive Design**: Mobile-first approach with CSS Grid and Flexbox  
**Language**: Danish (target audience)  
**Hosting**: Render (static site hosting)  
**CDN**: Cloudflare  
**Domain Management**: Cloudflare DNS  

### File Structure
```
├── index.html              # Main website page
├── styles/main.css         # All styling and responsive design
├── scripts/main.js         # Interactive functionality
├── *.JPG                   # Author photos
├── AI på Arbejde forside.png # Book cover image
├── render.yaml             # Render deployment config
├── _redirects              # Routing configuration
└── package.json            # Project configuration
```

### Contact

For questions about the book or to book workshops and presentations:
- Email: che.om@cbs.dk
- Purchase: [Akademisk Forlag](https://www.akademisk.dk/organisation-og-ledelse-0/innovation/produkt/ai-pa-arbejde)

### Authors

- **Mark Friis Hau** - Ph.d, Roskilde Universitet
- **Christian Hendriksen** - Ph.d, Copenhagen Business School  
- **Sine Zambach** - Ph.d, Copenhagen Business School