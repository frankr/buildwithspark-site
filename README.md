# Build with Spark - Website

Marketing website for Build with Spark AI assistant service.

## Pages

- `index.html` - Main landing page
- `realestate.html` - Real estate vertical landing page

## Tech Stack

- **HTML5** - Static HTML pages
- **Tailwind CSS** (via CDN) - Styling
- **Alpine.js** (via CDN) - Minimal interactivity (mobile menu, FAQ accordion, form handling)
- **Formspree** - Form submissions

## Form Setup

Both pages include waitlist forms using Formspree. **You need to update the form endpoint:**

1. Go to [formspree.io](https://formspree.io) and create an account
2. Create a new form
3. Copy your form endpoint (looks like `https://formspree.io/f/abc12345`)
4. Replace `https://formspree.io/f/xyzzzzzz` in both HTML files with your endpoint

Search for: `formspree.io/f/xyzzzzzz`

## Deployment

### Option 1: Vercel (Recommended)

1. Push to GitHub
2. Go to [vercel.com](https://vercel.com) and sign in with GitHub
3. Click "New Project" → Import your repo
4. Framework preset: **Other** (or leave as auto-detect)
5. Click Deploy

That's it. Vercel auto-detects static sites.

### Option 2: Netlify

1. Push to GitHub
2. Go to [netlify.com](https://netlify.com) and sign in with GitHub
3. Click "Add new site" → "Import an existing project"
4. Connect your repo
5. Build settings:
   - **Build command:** (leave empty)
   - **Publish directory:** `.` (root)
6. Click Deploy

### Option 3: Cloudflare Pages

1. Push to GitHub
2. Go to Cloudflare dashboard → Pages
3. Create a project → Connect to Git
4. Select your repo
5. Build settings:
   - **Framework preset:** None
   - **Build command:** (leave empty)
   - **Build output directory:** `/`
6. Deploy

### Option 4: Manual / Any Static Host

Just upload the files. The site is pure static HTML - no build step required.

Required files:
```
index.html
realestate.html
images/        (if any images are added later)
```

## Local Development

Just open `index.html` in a browser. No build tools needed.

For live reload during development:
```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx serve .

# Using PHP
php -S localhost:8000
```

## Custom Domain

After deploying to Vercel/Netlify/Cloudflare:

1. Add your domain in the dashboard (e.g., `buildwithspark.com`)
2. Update DNS records as instructed:
   - **Vercel:** CNAME to `cname.vercel-dns.com`
   - **Netlify:** CNAME to your Netlify subdomain
   - **Cloudflare:** Already handled if using Cloudflare DNS

SSL is automatic on all three platforms.

## Colors

- **Spark Orange:** `#E85D04`
- **Navy:** `#1A365D` (primary dark)
- **Navy Dark:** `#102a43`, `#0a1929`

See the Tailwind config in the `<script>` tag for full color palette.

## Assets

All assets currently use relative paths and CDNs:
- Fonts: Google Fonts CDN
- Icons: Inline SVG
- Tailwind: CDN
- Alpine.js: CDN

No local assets to manage (unless you add images to the `images/` folder).

---

Built with ✨ by Spark
