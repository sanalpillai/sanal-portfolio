# Sanal Pillai — Portfolio

Personal portfolio / professional profile site.

## Deploy to Vercel

### Option 1: One-click (Fastest)
1. Push this folder to a GitHub repo
2. Go to [vercel.com/new](https://vercel.com/new)
3. Import your GitHub repo
4. Vercel auto-detects static site — click **Deploy**
5. Add custom domain `sanalpillai.com` in Settings → Domains

### Option 2: Vercel CLI
```bash
npm i -g vercel
cd sanal-portfolio
vercel
```

### Option 3: Drag & Drop
1. Go to [vercel.com/new](https://vercel.com/new)
2. Drag the `public` folder directly onto the page
3. Done

## Custom Domain Setup
1. In Vercel dashboard → your project → Settings → Domains
2. Add `sanalpillai.com`
3. Update your domain's DNS:
   - **A Record**: `76.76.21.21`
   - **CNAME**: `cname.vercel-dns.com`

## Project Structure
```
sanal-portfolio/
├── public/
│   └── index.html    ← The entire site (single file)
├── vercel.json       ← Vercel config
└── README.md
```

## Customization
Everything is in `public/index.html`. Key sections to edit:
- **Hero**: Your name, tagline, typewriter phrases
- **Metrics marquee**: Impact numbers
- **Experience timeline**: Work history
- **Case studies**: Expandable project cards
- **Skills**: Grouped skill chips
- **Testimonials**: Quotes (replace with real ones)
- **Contact**: Email, phone, LinkedIn

## Interactive Features
- Mouse-following gradient spotlight
- Particle canvas with mouse repulsion
- Typewriter cycling through titles
- Text scramble effect on section headers (hover)
- Magnetic buttons (subtle cursor-follow)
- Scroll progress bar
- Blur-fade scroll reveal animations
- Expandable case study cards with glow borders
- Horizontal scrolling metrics marquee
- Parallax floating gradient blobs
- Active nav link tracking
- Scroll-to-top button

## To Add Your Resume PDF
1. Place `Sanal_Pillai_Resume.pdf` in the `public/` folder
2. Update the resume download link in the HTML:
   ```html
   <a href="/Sanal_Pillai_Resume.pdf" class="contact-link" download>
   ```

## To Add Your Photo
1. Place your photo in `public/` (e.g., `photo.jpg`)
2. Add an `<img>` tag in the hero section
