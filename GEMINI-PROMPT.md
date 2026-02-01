# Gemini CLI Build Prompt for Build with Spark

**Copy everything below this line and paste into Gemini CLI:**

---

## Build the Build with Spark Landing Page Website

Build a complete static HTML + Tailwind CSS marketing website for "Build with Spark" — an AI assistant service for busy professionals. This is a two-page website: Homepage and Real Estate vertical page.

### Tech Stack

- **HTML5** — Static pages, no framework
- **Tailwind CSS** — Via CDN (https://cdn.tailwindcss.com)
- **Alpine.js** — For mobile menu toggle and simple interactivity
- **Google Fonts** — Plus Jakarta Sans (headings) and Inter (body)
- **Heroicons** — SVG icons inline

### Project Structure

Create these files:
```
buildwithspark-site/
├── index.html              # Homepage
├── realestate.html         # Real estate landing page
├── images/                 # Image folder (create placeholder structure)
└── README.md
```

### Design System

Use these Tailwind config colors (inline in the HTML script tag):

```html
<script>
  tailwind.config = {
    theme: {
      extend: {
        colors: {
          primary: {
            50: '#FFF7ED',
            100: '#FFEDD5',
            400: '#FB923C',
            500: '#E85D04',
            600: '#D45203',
            700: '#B84602',
          },
          secondary: {
            100: '#E2E8F0',
            800: '#1E3A5F',
            900: '#1A365D',
          },
        },
        fontFamily: {
          heading: ['Plus Jakarta Sans', 'sans-serif'],
          body: ['Inter', 'sans-serif'],
        },
      },
    },
  }
</script>
```

Use warm off-white background: `bg-[#FFFAF5]`

### Homepage (index.html)

Build a single HTML file with all these sections:

**1. Head Section**
- Title: "Build with Spark — AI Assistants That Actually Work"
- Meta description for SEO
- Google Fonts links for Plus Jakarta Sans and Inter
- Tailwind CDN script
- Alpine.js CDN script

**2. Navigation Header**
- Logo text: "Build with Spark" with ✨ emoji
- Nav links: Pricing, For Real Estate, Contact
- Sticky with `fixed top-0 w-full bg-white/80 backdrop-blur-md`
- Mobile hamburger menu using Alpine.js `x-data="{ open: false }"`

**3. Hero Section**
- Headline: "Your AI Assistant Who Actually Feels Like Part of Your Team"
- Subhead: "Handles leads, schedules meetings, updates your CRM — and remembers every conversation."
- Primary CTA button (orange): "Meet Your Assistant"
- Secondary CTA button (outline): "See How It Works"
- Add a simple placeholder div for mockup image

**4. Problem Section**
- Section title: "Still Chasing Leads at 11pm?"
- 3 pain point cards in a grid:
  1. "Slow Follow-Up Loses Deals" — Respond in 5 minutes or lose them forever.
  2. "Human VAs Cost a Fortune" — $1,500-3,500/month for quality help.
  3. "Chatbots Feel Like Chatbots" — Scripted responses. No memory.

**5. Solution Section**
- Section title: "Not a Chatbot. An Actual Assistant."
- 6 feature cards (3x2 grid):
  1. Real Memory — Remembers every conversation
  2. Own Email Address — Gets a real email at your domain
  3. Available 24/7 — Never takes a day off
  4. Real Personality — Not robotic or scripted
  5. Full Integrations — Connects to your CRM, calendar, email
  6. Indistinguishable — 87% of leads thought they were talking to a human

**6. How It Works Section**
- Section title: "Up and Running in 24 Hours"
- 3 numbered steps:
  1. Tell Us About Your Business — 30-minute onboarding call
  2. We Build Your Assistant — Custom personality, integrations, workflows
  3. Start Delegating — Your assistant handles leads while you sleep

**7. Pricing Section**
- Section title: "Simple, Transparent Pricing"
- Single pricing card or "Contact for Pricing" CTA
- Mention: "Starting at $299/month"
- Include what's included: 24/7 availability, own email, CRM integration, etc.

**8. FAQ Section**
- Section title: "Questions? We've Got Answers."
- 5-6 collapsible FAQ items using Alpine.js
- Questions:
  - "Is it really AI or a human?" — 100% AI, but designed to feel human
  - "How is this different from a chatbot?" — Memory, personality, real email
  - "What if my clients realize it's AI?" — Most can't tell
  - "How long to get started?" — 24-48 hours
  - "Can I customize the personality?" — Yes, completely
  - "What happens if something goes wrong?" — Human escalation built-in

**9. Final CTA Section**
- Headline: "Ready to Stop Missing Leads?"
- Subhead: "Your AI assistant is one call away."
- Big orange CTA button: "Get Started Today"

**10. Footer**
- Logo and tagline
- Links: Home, Real Estate, Pricing, Contact
- Copyright: © 2026 Build with Spark

### Real Estate Page (realestate.html)

Similar structure but with real-estate-specific content:

**Hero**
- Headline: "Never Miss Another Lead. Ever."
- Subhead: "AI assistants built specifically for real estate agents. Respond instantly, nurture automatically, close more deals."

**Pain Points** (RE-specific)
- "Leads Go Cold While You're Showing Houses"
- "Your CRM Is a Graveyard of Good Intentions"  
- "You Can't Clone Yourself (We Did It For You)"

**Features** (RE-specific)
- Instant Lead Response — Under 60 seconds, 24/7
- Showing Scheduler — Books appointments directly to your calendar
- MLS Monitoring — Alerts matched to buyer preferences
- Past Client Nurture — Automated anniversary/check-in messages
- CRM Auto-Updates — Notes logged after every conversation

**ROI Story**
- "One Extra Deal Per Year = $10,000+ in Commission"
- "Your Spark assistant costs less than $6,000/year"
- "That's 60% ROI from ONE deal"

**Testimonials Placeholder**
- 2-3 placeholder testimonial cards
- "Coming soon: Real stories from real agents"

**CTA**
- "Join the Waitlist for Real Estate Agents"
- Email capture form using Formspree

### Forms

Use Formspree for form handling:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
  <input type="email" name="email" placeholder="Enter your email" required>
  <button type="submit">Join Waitlist</button>
</form>
```

### Style Guidelines

- Use `font-heading` for all headings (h1, h2, h3)
- Use `font-body` for body text
- Primary buttons: `bg-primary-500 hover:bg-primary-600 text-white px-6 py-3 rounded-lg`
- Secondary buttons: `border-2 border-primary-500 text-primary-500 hover:bg-primary-50 px-6 py-3 rounded-lg`
- Section padding: `py-20 px-4 md:px-8 lg:px-16`
- Max content width: `max-w-7xl mx-auto`
- Card shadows: `shadow-lg hover:shadow-xl transition-shadow`

### Mobile Responsive

- Stack everything vertically on mobile
- Hide nav links on mobile, show hamburger
- Reduce heading sizes on mobile
- Use Tailwind responsive prefixes: `md:`, `lg:`

---

Build both complete HTML files with all sections. Make them production-ready with proper spacing, typography, and responsive design. The site should look professional and convert visitors.
