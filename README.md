# Build with Spark - Marketing Website

AI assistants for busy professionals. Built with Next.js 14, Tailwind CSS, and TypeScript.

## Quick Start

### Option 1: Build with Gemini CLI

1. Open Gemini CLI
2. Copy the contents of `GEMINI-PROMPT.md` and paste it
3. Let Gemini build the site
4. Review and iterate

### Option 2: Manual Development

```bash
# Install dependencies
npm install

# Run development server
npm run dev

# Build for production
npm run build
```

## Project Structure

```
├── BUILD-SPEC.md        # Complete specification document
├── GEMINI-PROMPT.md     # Ready-to-paste prompt for Gemini CLI
├── src/
│   ├── app/
│   │   ├── page.tsx     # Homepage
│   │   └── realestate/  # Real estate landing page
│   └── components/      # React components
```

## Pages

- **/** - Homepage (general introduction)
- **/realestate** - Real estate agents landing page

## Tech Stack

- Next.js 14+ with App Router
- TypeScript
- Tailwind CSS
- Plus Jakarta Sans + Inter fonts
- Lucide React icons

## Design System

- **Primary Color:** Orange (#E85D04)
- **Secondary Color:** Navy (#1A365D)
- **Background:** Warm off-white (#FFFAF5)

See `BUILD-SPEC.md` for complete design documentation.

## Deployment

Deploy to Vercel:

```bash
vercel
```

Or connect this repo to Vercel for automatic deployments.

## License

Private - Build with Spark © 2026
