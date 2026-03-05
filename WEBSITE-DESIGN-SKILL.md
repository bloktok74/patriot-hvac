# SKILL: World-Class Website Design & Reconstruction
**For Claude Code — Autonomous Web Development**

---

## PURPOSE

This skill governs how Claude Code approaches ALL website work — whether building from scratch, reverse-engineering an existing site, or creating industry-specific templates. The goal is always the same: **deliver a website so refined, so intentional, and so functional that it makes the original look like a rough draft.**

This is not a template-filling exercise. This is craft.

---

## PART 1: AUTONOMOUS DEVELOPMENT PROTOCOL

Before writing a single line of code, Claude Code must execute this protocol:

### Step 1 — Understand the Mission
Answer these questions internally before proceeding:
- What is the **business purpose** of this site? (generate leads, sell product, build authority, serve users?)
- Who is the **target audience**? (demographics, device preferences, intent)
- What **action** should a visitor take? (the ONE conversion goal)
- What **feeling** should the site evoke? (trusted, excited, luxurious, inspired, urgent?)
- What **industry conventions** exist — and which ones should be broken?

### Step 2 — Commit to an Aesthetic Direction
Pick a clear, bold visual identity. Do NOT be generic. Options include:
- **Editorial Luxury** — oversized type, restraint, negative space, monochromatic with one accent
- **Kinetic Energy** — motion-first, layered elements, bold typography in motion, dark base
- **Clean Authority** — crisp grid, data-forward, confident sans-serif, professional cool
- **Organic Premium** — warm tones, textured backgrounds, serif display fonts, human photography
- **Neo-Brutalist** — raw structure, high contrast, unpolished-yet-intentional, makes you stop
- **Immersive Dark** — deep dark backgrounds, glowing accents, glass morphism, futuristic
- **Soft Prestige** — light backgrounds, refined micro-details, pastel accents, approachable luxury

**RULE: Name the aesthetic before writing code.** If you can't name it, you haven't decided yet.

### Step 3 — Plan the Architecture
Map out:
- **Page sections** in order (hero, social proof, features, how it works, CTA, footer, etc.)
- **Navigation structure** (what goes in nav, what's hidden, sticky or transparent?)
- **Responsive breakpoints** (mobile-first or desktop-down — decide and be consistent)
- **Interactive elements** (what animates, what has hover states, what triggers on scroll)

### Step 4 — Build in This Order
1. HTML structure with semantic markup
2. CSS design system (variables, typography scale, spacing system, color palette)
3. Layout (grid/flex structure, section spacing)
4. Visual design (colors, textures, imagery, backgrounds)
5. Typography (font pairing, hierarchy, sizing, line-height)
6. Animations and micro-interactions
7. Mobile responsiveness
8. Final polish pass (spacing, shadows, transitions, edge cases)

---

## PART 2: BUILDING BEAUTIFUL SITES FROM SCRATCH

### Non-Negotiables for Every Site

**Typography**
- Import from Google Fonts or use system alternatives — NEVER default to Arial, Helvetica, or system-ui without intention
- Use a **display font** (for headlines) + **body font** (for text) pairing — always two different typefaces
- Font size scale: use a modular scale (1.25x or 1.333x ratio). Never random sizes.
- Line height: 1.1–1.3 for headlines, 1.6–1.75 for body
- Letter spacing: tighten display type (-0.02em to -0.04em), loosen all-caps labels (+0.1em)

**Color System**
```css
:root {
  --color-bg:        /* site background */
  --color-surface:   /* card/panel backgrounds */
  --color-border:    /* subtle dividers */
  --color-text:      /* primary text */
  --color-muted:     /* secondary/supporting text */
  --color-accent:    /* primary brand action color */
  --color-accent-2:  /* secondary accent if needed */
}
```
Use these variables EVERYWHERE. Changing the theme means changing 6 lines.

**Spacing System**
Use an 8px base grid. All spacing values should be multiples of 8:
`8px, 16px, 24px, 32px, 48px, 64px, 96px, 128px`

**Visual Depth**
Every site needs atmosphere. Choose at least TWO from:
- Gradient mesh backgrounds
- Subtle noise/grain texture overlay
- Layered transparency (glassmorphism)
- Deep drop shadows with color tint
- Background geometric shapes (blurred, low opacity)
- Diagonal or curved section dividers
- Border gradients on cards

### Hero Section — The Most Important Section
The hero must accomplish in 3 seconds:
1. **Who this is for** (audience clarity)
2. **What they get** (value clarity)  
3. **What to do next** (action clarity)

Hero formula that works:
```
[CATEGORY LABEL in small caps]
[BOLD HEADLINE — 3-7 words, max impact]
[ONE supporting sentence — specific, not vague]
[PRIMARY CTA BUTTON] [Secondary ghost button or trust signal]
[Social proof: avatars + "X customers" OR media logos]
[Hero visual: product, person, or abstract that reinforces message]
```

**NEVER write headlines like:**
- "Welcome to [Company Name]" ❌
- "We provide solutions for your business" ❌
- "Innovative, cutting-edge, world-class services" ❌

**ALWAYS write headlines like:**
- "Debt-Free in 36 Months or We Work Free" ✓
- "Your Home. Managed Like You Own the Building." ✓
- "The AI Voice Agent That Closes Leads at 2AM" ✓

### Animation Principles
- **Page load**: Stagger fade-up animations on hero elements (0ms, 100ms, 200ms, 300ms delays)
- **Scroll reveal**: Elements fade/slide in as user scrolls (use Intersection Observer)
- **Hover states**: Every clickable element needs a hover response (transform, color shift, or glow)
- **Transitions**: All color/opacity changes: `transition: 0.2s ease`; transforms: `transition: 0.3s cubic-bezier(0.34, 1.56, 0.64, 1)` for spring feel
- **NEVER animate everything** — motion should highlight importance, not decorate everything

---

## PART 3: CLONING & UPGRADING EXISTING WEBSITES

When given a URL or screenshot of an existing site, follow this protocol:

### Phase 1 — Audit the Original
Systematically evaluate:

| Category | What to Assess |
|---|---|
| **Structure** | Navigation, sections, page flow, information hierarchy |
| **Functionality** | Forms, CTAs, interactive elements, integrations |
| **Messaging** | Headlines, subheadlines, body copy, CTAs, value props |
| **Visual Design** | Colors, fonts, spacing, imagery, brand consistency |
| **Trust Signals** | Reviews, logos, certifications, team, stats |
| **Mobile** | Responsive behavior, touch targets, readability |
| **Performance** | Load speed indicators, image optimization, code bloat |

### Phase 2 — Identify What to Keep, Upgrade, and Reimagine

**KEEP** (preserve functionality and messaging that works):
- Core navigation structure (if logical)
- Proven conversion sections (testimonials, before/after, guarantee)
- Business-critical information (contact, location, services)
- Existing brand identity elements if client wants continuity

**UPGRADE** (improve execution of existing intent):
- Weak headlines → powerful, specific, benefit-driven headlines
- Generic stock photos → intentional visual direction
- Cluttered layouts → breathing room and visual hierarchy
- Inconsistent spacing → systematic grid
- Missing animations → purposeful motion
- Poor mobile → mobile-first rebuild

**REIMAGINE** (replace entirely with superior approach):
- Outdated visual design → fresh aesthetic aligned to industry + brand
- Confusing navigation → streamlined, user-goal-oriented nav
- Weak CTAs → high-conversion button copy and placement
- Missing social proof → structured trust section
- No visual hierarchy → clear typographic scale

### Phase 3 — Rebuild with Full Fidelity
The rebuilt site must:
1. **Preserve all original content** (unless instructed to rewrite)
2. **Match or exceed all original functionality** (forms, links, interactions)
3. **Look 10x more professional** than the original
4. **Load faster** (no unnecessary libraries, optimized CSS)
5. **Work perfectly on mobile** (not just "responsive" — actually optimized)

### Code Comment Standard for Rebuilt Sites
Add a comment block at the top of rebuilt sites:
```html
<!--
  REBUILT SITE: [Original URL or Name]
  Original audit: [2-3 sentence summary of original's issues]
  Design direction: [Named aesthetic chosen]
  Key improvements: [List top 5 changes]
  Preserved functionality: [What was carried over]
-->
```

---

## PART 4: INDUSTRY-SPECIFIC TEMPLATES

Each industry has **conversion patterns, trust signals, and visual conventions** that work. Know them — then elevate them.

---

### 🏠 Property Management
**What users need to see:** Professionalism, responsiveness, trustworthiness with their asset
**Conversion goal:** Owner inquiry form OR tenant application
**Must-have sections:**
- Hero with property photo + "Peace of Mind for Property Owners" type messaging
- Services breakdown (what's included in management)
- Geographic coverage map or city list
- Owner testimonials (NOT tenant testimonials — owners are the client)
- Fee transparency or "get a free analysis" CTA
- Emergency maintenance line prominently displayed
**Aesthetic:** Clean Authority or Organic Premium
**Color palette inspiration:** Deep navy or forest green + white + warm gold accent
**Trust signals:** Number of properties managed, years in business, licensed badge, BBB/Google rating

---

### 💰 Debt Relief / Financial Services
**What users need to see:** Hope, legitimacy, expertise, non-judgment
**Conversion goal:** Free consultation form submission or phone call
**Must-have sections:**
- Hero with empathetic, qualifying headline ("If you owe $10k+ in credit card debt...")
- How it works (3-step process, simplified)
- Savings calculator or "see if you qualify" widget
- Real client results ($ saved, months to freedom)
- Accreditation badges (AFCC, IAPDA, BBB A+)
- FAQ addressing objections (will this hurt my credit? is this legit?)
- Sticky CTA bar on mobile
**Aesthetic:** Clean Authority with warm tones — NEVER cold/corporate
**Color palette inspiration:** Deep blue + white + emerald green (not red — too alarming)
**Trust signals:** AFCC member, years in business, total debt resolved ($), accreditations
**CRITICAL:** Compliance-safe copy — avoid guarantees on specific outcomes

---

### 💉 Cosmetic Surgery / Medical Aesthetics
**What users need to see:** Expertise, beautiful results, safety, discretion
**Conversion goal:** Consultation booking
**Must-have sections:**
- Hero with aspirational imagery (not before/after — those go lower)
- Procedures menu (organized, filterable)
- Surgeon/provider credentials and bio
- Before & after gallery (with consent, mobile-optimized)
- Patient testimonials (video preferred)
- Financing options (everyone wants to know)
- Awards, board certifications, affiliations
- Virtual consultation option
**Aesthetic:** Editorial Luxury or Soft Prestige
**Color palette inspiration:** Off-white or warm ivory + black + rose gold OR sage green
**Trust signals:** Board certification, number of procedures performed, media features, reviews
**NEVER:** Stock medical imagery, clip art, cluttered service menus, unclear pricing

---

### 🏗️ Construction / Contracting
**What users need to see:** Credibility, portfolio quality, reliability, local presence
**Conversion goal:** Free estimate request
**Must-have sections:**
- Hero with real project photo (not stock) + clear service area
- Services offered (organized by category)
- Project portfolio / gallery (LARGE images)
- Licensing & insurance badges (critical for trust)
- Process timeline (how working with us works)
- Client testimonials with project type
- Financing or payment plan info
- Emergency services line if applicable
**Aesthetic:** Clean Authority or Industrial/Utilitarian with premium touches
**Color palette inspiration:** Charcoal + white + orange or yellow accent OR navy + white + red
**Trust signals:** License number visible, insurance verified, years in business, local address
**NEVER:** Cheesy clip art hammers, Comic Sans, unclear service area, no portfolio

---

### 🤖 AI / Automation Agency (like Happi Agents)
**What users need to see:** Intelligence, ROI clarity, modern credibility, trust in tech
**Conversion goal:** Discovery call booking or demo request
**Must-have sections:**
- Hero with bold ROI headline ("Automate 80% of Your Lead Follow-Up — Before Your Competitor Does")
- Use-case breakdown by industry or workflow type
- How it works (visual flow diagram)
- Results/case studies with metrics (hours saved, conversion lift, cost reduction)
- Technology stack logos (n8n, OpenAI, Retell, etc.) — builds credibility
- Pricing tiers OR "custom quote" CTA
- FAQ (what do I need to get started? how long to implement?)
- Integration logos grid
**Aesthetic:** Immersive Dark or Kinetic Energy — must feel cutting-edge
**Color palette inspiration:** Deep black + electric cyan or green + white text
**Trust signals:** Client logos, case study metrics, integrations, founder credentials

---

### 🏥 Healthcare / FQHC / Medical Centers
**What users need to see:** Care, safety, accessibility, multilingual support
**Conversion goal:** Appointment booking
**Must-have sections:**
- Hero with welcoming, diverse imagery + "Accepting New Patients" badge
- Services / specialties organized clearly
- Insurance accepted (HUGE trust factor)
- Provider bios with photos
- Patient portal link (prominent)
- Locations map + hours
- Telehealth option if available
- Multilingual support indicator
**Aesthetic:** Clean Authority with warm, human touches
**Color palette inspiration:** Healthcare blue + white + soft teal or green
**Trust signals:** FQHC designation, JCAHO, NCQA, patient ratings, years serving community

---

## PART 5: CODE QUALITY STANDARDS

### HTML
- Semantic tags always: `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`
- All images have meaningful `alt` text
- Forms have proper `label` elements tied to inputs
- Logical heading hierarchy: one `<h1>`, then `<h2>`, `<h3>` as needed
- ARIA attributes where needed for accessibility

### CSS
- Design system variables declared in `:root` — used everywhere
- Mobile-first media queries: `@media (min-width: 768px) { }`
- No magic numbers — all values trace back to the spacing/sizing system
- No inline styles except for dynamic JS-injected values
- Class names: BEM methodology or clear utility names
- Animations defined in `@keyframes` at bottom of CSS block

### JavaScript
- Vanilla JS preferred for simple interactions (no jQuery dependency)
- Intersection Observer for scroll animations (not scroll event listeners)
- Event delegation where possible
- No console.log() in production code
- Form validation with helpful error messages

### Performance
- No unused CSS frameworks (don't import all of Bootstrap for a hero section)
- Google Fonts loaded with `display=swap`
- Images use `loading="lazy"` except above-the-fold hero
- Animations use `transform` and `opacity` only (GPU-composited, no layout thrashing)
- CSS custom properties over repeated values

---

## PART 6: DELIVERABLE CHECKLIST

Before declaring a site complete, verify:

**Content**
- [ ] All placeholder text replaced with real or realistic content
- [ ] All links functional or noted as placeholder
- [ ] Forms have validation and submission feedback
- [ ] Mobile navigation works (hamburger menu or drawer)

**Design**
- [ ] Consistent spacing throughout (no random gaps)
- [ ] Clear visual hierarchy on every section
- [ ] All hover states implemented
- [ ] Animations don't cause layout shift
- [ ] Color contrast passes WCAG AA (4.5:1 for text)

**Mobile**
- [ ] Tested at 375px (iPhone SE) and 390px (iPhone 14)
- [ ] Touch targets minimum 44x44px
- [ ] Text readable without zooming
- [ ] No horizontal scroll

**Code**
- [ ] Design system variables in use
- [ ] Semantic HTML structure
- [ ] No console errors
- [ ] Single file unless project requires separation

---

## QUICK REFERENCE: FONT PAIRINGS BY AESTHETIC

| Aesthetic | Display Font | Body Font |
|---|---|---|
| Editorial Luxury | Playfair Display | Lato |
| Kinetic Energy | Anton | DM Sans |
| Clean Authority | Syne | Source Sans 3 |
| Organic Premium | Cormorant Garamond | Nunito |
| Neo-Brutalist | Bebas Neue | IBM Plex Mono |
| Immersive Dark | Orbitron | Exo 2 |
| Soft Prestige | Libre Baskerville | Mulish |
| Modern Agency | Cabinet Grotesk | General Sans |

---

## QUICK REFERENCE: DO / NEVER

| ✅ ALWAYS DO | ❌ NEVER DO |
|---|---|
| Name the aesthetic before coding | Start coding without a design direction |
| Use CSS custom properties for colors | Hardcode hex values throughout |
| Write specific, benefit-driven headlines | Write vague "welcome to our company" copy |
| Add scroll animations with Intersection Observer | Use scroll event listener for animations |
| Mobile-first responsive CSS | Desktop-only then "fix" mobile after |
| Real content or realistic placeholders | Lorem ipsum in final deliverables |
| Semantic HTML (header, nav, main, section) | Div soup |
| 8px grid spacing system | Random margin/padding values |
| Include hover states on all interactive elements | Leave buttons flat with zero hover feedback |
| Pair two distinct typefaces | Use one font for everything |

---

*This skill is maintained by Happi Agents. Update as new patterns, industries, and techniques are validated through client projects.*
