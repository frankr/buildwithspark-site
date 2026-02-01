# Gemini CLI Build Prompt for Build with Spark

**Copy everything below this line and paste into Gemini CLI:**

---

## Build the Build with Spark Landing Page Website

Build a complete Next.js marketing website for "Build with Spark" — an AI assistant service for busy professionals. This is a two-page website: Homepage and Real Estate vertical page.

### Project Setup

Initialize a new Next.js 14+ project with App Router:
- Use TypeScript
- Use Tailwind CSS for styling
- Install Google Fonts: Plus Jakarta Sans (headings) and Inter (body)
- Install Lucide React for icons
- Set up the following structure:

```
src/
├── app/
│   ├── layout.tsx
│   ├── page.tsx (Homepage)
│   ├── realestate/page.tsx (Real Estate page)
│   └── globals.css
├── components/
│   ├── ui/ (Button, Card, Input, Badge)
│   ├── layout/ (Header, Footer)
│   └── sections/ (Hero, Features, Pricing, FAQ, Testimonials, CTA)
```

### Design System

Use these exact colors in tailwind.config.ts:

```js
colors: {
  primary: {
    50: '#FFF7ED',
    100: '#FFEDD5',
    200: '#FED7AA',
    300: '#FDBA74',
    400: '#FB923C',
    500: '#E85D04', // Main orange
    600: '#D45203',
    700: '#B84602',
    800: '#9A3412',
    900: '#7C2D12',
  },
  secondary: {
    50: '#F8FAFC',
    100: '#E2E8F0',
    500: '#64748B',
    800: '#1E3A5F',
    900: '#1A365D', // Main navy
  },
  background: '#FFFAF5', // Warm off-white
}
```

Use Plus Jakarta Sans for headings (font-semibold and font-bold) and Inter for body text.

### Homepage (/)

Build these sections in order:

**1. Navigation Header**
- Logo text: "Build with Spark" with spark emoji ✨
- Nav links: Pricing, For Real Estate, Contact
- Sticky on scroll with backdrop blur
- Mobile hamburger menu

**2. Hero Section**
- Headline: "Your AI Assistant Who Actually Feels Like Part of Your Team"
- Subhead: "Handles leads, schedules meetings, updates your CRM — and remembers every conversation."
- Primary CTA: "Meet Your Assistant" (orange button)
- Secondary CTA: "See How It Works" (outline button)
- Right side: Mockup of chat interface showing conversation

**3. Problem Section**
- Section title: "Still Chasing Leads at 11pm?"
- 3 pain point cards:
  1. Clock icon - "Slow Follow-Up Loses Deals" - "Respond in 5 minutes or lose them forever. But you can't watch your inbox 24/7."
  2. DollarSign icon - "Human VAs Cost a Fortune" - "$1,500-3,500/month for quality help. And they still take vacation."
  3. Bot icon - "Chatbots Feel Like Chatbots" - "Scripted responses. No memory. Clients can tell instantly."
- Closing text: "There's never been a good middle ground — until now."

**4. Solution Section**
- Section title: "Not a Chatbot. An Actual Assistant."
- 6 feature cards in 3x2 grid:
  1. Brain icon - "Real Memory" - "Remembers every conversation and uses context to build real relationships"
  2. Mail icon - "Own Email Address" - "Gets a real email at your domain — clients email Sarah@yourbrokerage.com"
  3. Moon icon - "Available 24/7" - "2am inquiry? Sunday callback? Already handled. Never takes a day off"
  4. MessageSquare icon - "Real Personality" - "Not robotic or scripted — adapts tone and style to each conversation"
  5. Link icon - "Full Integrations" - "Connects to your CRM, calendar, email, and all your existing tools"
  6. Smile icon - "Indistinguishable" - "In blind tests, 87% of leads thought they were talking to a human"

**5. How It Works Section**
- Section title: "Up and Running in 24 Hours"
- 3 numbered steps with icons:
  1. "Tell Us About Your Business" - "15-minute call. Your style, your listings, your preferences."
  2. "Meet Your Assistant" - "We customize their personality and set up their email and integrations."
  3. "Watch Them Work" - "Spark starts engaging leads immediately. You focus on closing."
- CTA: "Start Your Setup"

**6. Testimonials Section**
- Section title: "What Agents Are Saying"
- Featured large testimonial with avatar placeholder:
  - Quote: "Spark scheduled 47 showings last month while I focused on closings. I've already paid for a year of service from one deal alone."
  - Name: "Marcus Chen"
  - Company: "Keller Williams San Diego"
- 2 smaller testimonial cards below

**7. Pricing Section**
- Section title: "Simple Pricing. Serious ROI."
- 2 pricing cards side by side:
  
  Card 1 - Starter:
  - Price: $299/month
  - Description: "Solo agents getting started"
  - Features: Lead follow-up & qualification, Calendar scheduling, Basic CRM sync, Email support
  - CTA: "Get Started"
  
  Card 2 - Pro (with "Most Popular" badge):
  - Price: $499/month
  - Description: "Producing agents"
  - Features: Everything in Starter, MLS monitoring & alerts, Social media assistance, Priority support, Full CRM integration
  - CTA: "Get Started"

- Below cards: "Compare: Human VAs cost $1,500-3,500/month. One closed deal pays for a year of Spark."

**8. FAQ Section**
- Section title: "Questions? We've Got Answers."
- Accordion-style FAQ with these Q&As:
  1. Q: "Is this a chatbot?" A: "No. Chatbots follow scripts and decision trees. Spark uses advanced AI that reasons, remembers context, and holds genuine conversations."
  2. Q: "Will my clients know it's AI?" A: "In testing, 87% of leads thought they were talking to a human. You can also choose to disclose it's AI."
  3. Q: "What if I want human oversight?" A: "You're always in control. Review any conversation, set escalation rules, or take over any chat instantly."
  4. Q: "Is my data secure?" A: "Your data never trains public AI models. We use enterprise-grade encryption and follow strict privacy practices."
  5. Q: "How long does setup take?" A: "Most agents are fully live within 24 hours. We handle the technical work."
  6. Q: "Can I cancel anytime?" A: "Yes. No long-term contracts required."

**9. Final CTA Section**
- Dark navy background
- Headline: "Ready to Meet Your New Assistant?"
- Subhead: "Join hundreds of professionals who've upgraded from burnout to balance."
- CTA: "Get Your AI Assistant" (orange button)
- Trust line: "✓ Setup in 24 hours · ✓ No contracts · ✓ Cancel anytime"

**10. Footer**
- Logo
- Links: For Real Estate, Pricing, About, Contact, Privacy Policy, Terms
- Copyright: "© 2026 Build with Spark. All rights reserved."

### Real Estate Page (/realestate)

Build these sections:

**1. Hero**
- Headline: "Built for Agents Who Close, Not Chase"
- Subhead: "Real estate moves fast. Your AI assistant moves faster. Spark handles the leads. You handle the deals."
- CTA: "Get Your Real Estate Assistant"

**2. Pain Points**
- Section title: "Sound Familiar?"
- 4 pain points with emoji:
  1. 😩 "Zillow lead at 11pm — you respond at 8am — they've already talked to 3 other agents"
  2. 😩 "Great open house, 20 sign-ins, zero follow-ups because... life happened"
  3. 😩 "CRM is a graveyard of 'I'll circle back' leads you never did"
  4. 😩 "Thought about a VA but $1,500/month for someone who doesn't even know real estate?"

**3. Features**
- Section title: "Your Assistant Knows Real Estate"
- 4 feature blocks (alternating image/text layout):
  1. "Qualifies Leads Instantly" - "What's your timeline? Are you pre-approved? What areas are you considering? Spark asks the right questions."
  2. "Books Showings on Autopilot" - "Checks your calendar, finds times, books the appointment, sends the address and lockbox code."
  3. "Nurtures Until They're Ready" - "That 'just looking' lead? Spark stays in touch for months. When they're ready, they remember you."
  4. "Updates Your CRM Automatically" - "Every conversation logged. Every status updated. No more manual data entry at 10pm."

**4. ROI Section**
- Section title: "The Math Makes Sense"
- Display: Average commission $8,000 / Spark cost $299/mo = One extra deal = 27x ROI
- Text: "Most agents close 2-3 extra deals in the first 6 months."
- CTA: "Start Closing More Deals"

**5. Comparison Table**
- Section title: "Spark vs. The Alternatives"
- Table comparing: Spark, Human VA, Chatbot, DIY
- Rows: Monthly cost, Available 24/7, Remembers context, Feels human, Own email, Never quits, Knows real estate
- Use checkmarks and X marks

**6. Testimonials**
- Section title: "Agents Love Spark"
- 3 testimonial cards with quotes and names

**7. Final CTA**
- Gradient or image background
- Headline: "Stop Losing Leads. Start Closing Deals."
- Subhead: "Join 100+ real estate agents who upgraded their follow-up"
- CTA: "Get Your AI Assistant — $299/month"
- Trust: "✓ Setup in 24 hours · ✓ No contracts · ✓ Cancel anytime"

### Contact Form Component

Create a reusable contact form with:
- Name (required)
- Email (required)  
- Phone (optional)
- Company/Brokerage (optional)
- Message textarea (optional)
- Submit button: "Get Started"

Use Formspree for form handling. The form action URL will be added later as an environment variable.

### Technical Requirements

1. All pages must be mobile-first responsive
2. Use semantic HTML
3. Add smooth scroll behavior
4. FAQ should be interactive accordion
5. Add hover effects on buttons and cards
6. Implement proper TypeScript types
7. Use Tailwind's container class for max-width
8. Add proper meta tags in layout.tsx:
   - Title: "Build with Spark - AI Assistants That Feel Like Real Team Members"
   - Description: "Get a dedicated AI assistant with personality, memory, and their own email. 80% less than human VAs."

### Component Guidelines

- Keep components modular and reusable
- Extract repeated patterns into UI components
- Use consistent spacing (py-16 md:py-24 for sections)
- Cards should have subtle shadows and rounded corners (rounded-xl)
- Orange buttons: bg-primary-500 hover:bg-primary-600 text-white
- Navy backgrounds for CTA sections: bg-secondary-900

Build the complete site with all sections, making it production-ready. Focus on clean code, proper TypeScript, and beautiful responsive design.
