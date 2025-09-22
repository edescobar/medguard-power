# MedGuard Power - Brand Book
## Miami Retro Healthcare Style Guide

---

## 🎨 Brand Personality

**Brand Essence:** Professional healthcare meets Miami retro charm

**Voice & Tone:**
- **Professional** yet approachable
- **Confident** without being corporate
- **Warm** like Miami hospitality
- **Trustworthy** as healthcare demands
- **Energetic** reflecting emergency response readiness

**Visual Style:** 1950s Miami Beach meets modern healthcare - combining nostalgic warmth with clinical precision

---

## 🎨 Color Palette

### Primary Colors
```css
--clr-brand-teal: #0D4B4B;      /* Deep Teal - Primary brand color (logo) */
--clr-brand-teal-light: #1A6B6B; /* Medium Teal - Headers */
--clr-safety-orange: #F25C2A;    /* Safety Orange - CTAs, alerts */
--clr-coral: #FF7A45;            /* Coral - Hover states, accents */
```

### Background Colors
```css
--clr-bg-warm: #F5EFE6;          /* Warm Beige - Primary background */
--clr-bg-white: #FFFFFF;         /* Pure White - Cards, sections */
--clr-bg-cream: #FFF9F5;         /* Soft Cream - Alternative sections */
```

### Text Colors
```css
--clr-ink-primary: #0F2D35;      /* Deep Teal-Black - Body text */
--clr-ink-muted: #5C6B70;        /* Muted Gray - Secondary text */
--clr-ink-light: #8A9499;        /* Light Gray - Captions */
```

### Utility Colors
```css
--clr-success: #00A86B;          /* Green - Success, compliance */
--clr-warning: #FFB84D;          /* Amber - Warnings */
--clr-danger: #E74C3C;           /* Red - Urgent, errors */
--clr-border: #E5E0D6;           /* Light Border */
```

### Color Usage Rules
- **Teal** → Headers, logos, primary navigation
- **Orange** → CTAs, emergency messaging, highlights
- **Beige** → Background for warmth and approachability
- **White** → Content cards, form backgrounds
- Always maintain 4.5:1 contrast ratio for accessibility

---

## 📝 Typography

### Font Families

**Display/Logo Font:** Pacifico
- Used for: Logo, hero headlines, special callouts
- Character: Retro script, friendly, memorable
- Never use below 24px

**Primary Font:** League Spartan
- Used for: Headers, buttons, navigation
- Weights: 400 (Regular), 600 (SemiBold), 700 (Bold), 800 (ExtraBold), 900 (Black)
- Character: Strong, clean, professional

**Fallback Stack:**
```css
--ff-display: "Pacifico", "Brush Script MT", cursive;
--ff-sans: "League Spartan", "Montserrat", "Inter", system-ui, -apple-system, sans-serif;
```

### Type Scale
```css
--fs-900: clamp(2.6rem, 5vw, 4rem);     /* Hero headlines */
--fs-800: clamp(2rem, 4vw, 3rem);       /* Section headers */
--fs-700: clamp(1.6rem, 3vw, 2.2rem);   /* Subsection headers */
--fs-600: 1.25rem;                      /* Large body */
--fs-500: 1.125rem;                     /* Medium body */
--fs-400: 1rem;                         /* Base body */
--fs-300: 0.875rem;                     /* Small text */
```

### Typography Rules
- **Headers:** Always use League Spartan Bold/ExtraBold
- **Body:** League Spartan Regular, line-height 1.6
- **Logo text:** Pacifico for "MedGuard", League Spartan Black for "POWER SERVICES"
- **Buttons:** League Spartan ExtraBold, uppercase, letter-spacing 0.08em

---

## 🎯 Logo Usage

### Logo Composition
```
[Pacifico Script] MedGuard [Orange Starburst]
[League Spartan] POWER SERVICES
```

### Logo Variations
1. **Primary:** Full color on light background
2. **Reverse:** White on dark teal background
3. **Monochrome:** Single color for documents
4. **Icon:** Starburst alone for favicons/apps

### Clear Space
- Minimum clear space = height of the starburst icon
- Never place logo on busy backgrounds
- Always maintain proper contrast

### Logo Don'ts
- ❌ Don't stretch or distort
- ❌ Don't change colors arbitrarily
- ❌ Don't add drop shadows or effects
- ❌ Don't use on orange backgrounds

---

## 🎨 Visual Elements

### Starburst Icon
- 8-pointed star
- Primary: Orange (#F25C2A)
- Secondary: Teal outline variant
- Represents: Energy, power, reliability

### Border Radius
```css
--radius: 14px;        /* Standard cards, buttons */
--radius-lg: 22px;     /* Large cards, hero sections */
--radius-full: 999px;  /* Pills, round buttons */
```

### Shadows
```css
--shadow-1: 0 6px 18px rgba(15,45,53,0.08);   /* Subtle depth */
--shadow-2: 0 18px 40px rgba(15,45,53,0.14);  /* Hover states */
--shadow-3: 0 24px 60px rgba(15,45,53,0.20);  /* Modals */
```

### Patterns
- Subtle grid pattern for backgrounds (10% opacity)
- Wave pattern for section dividers (Miami beach inspired)
- Dot pattern for testimonial backgrounds

---

## 🔘 Component Styles

### Buttons

**Primary Button**
```css
background: var(--clr-safety-orange);
color: white;
border-radius: 999px;
padding: 0.9rem 1.6rem;
font-weight: 800;
letter-spacing: 0.08em;
text-transform: uppercase;
```

**Secondary Button**
```css
background: transparent;
color: var(--clr-brand-teal);
border: 2px solid var(--clr-brand-teal);
```

**Emergency Button**
```css
background: var(--clr-danger);
animation: pulse 2s infinite;
```

### Cards
```css
background: white;
border: 1px solid var(--clr-border);
border-radius: var(--radius);
padding: 1.5rem;
box-shadow: var(--shadow-1);
```

### Forms
- Rounded corners (12px)
- Thick borders on focus (2px orange)
- Warm white backgrounds
- Clear error states with red borders

---

## 📐 Layout Principles

### Grid System
- Max width: 1200px
- Gutter: 1.5rem
- Mobile first approach
- Breakpoints: 640px, 768px, 1024px

### Spacing Scale
```css
--space-xs: 0.25rem;   /* 4px */
--space-sm: 0.5rem;    /* 8px */
--space-md: 1rem;      /* 16px */
--space-lg: 1.5rem;    /* 24px */
--space-xl: 2rem;      /* 32px */
--space-2xl: 3rem;     /* 48px */
--space-3xl: 4rem;     /* 64px */
```

### Section Padding
```css
padding: clamp(3rem, 6vw, 6rem) 0;
```

---

## 💬 Voice & Messaging

### Headlines
- **DO:** "Never Fail an AHCA Inspection Again"
- **DON'T:** "Generator Maintenance Services Available"

### CTAs
- **Primary:** "Get Your Free Compliance Audit"
- **Secondary:** "See Our Compliance Checklist"
- **Emergency:** "24/7 Emergency Response"

### Value Props (Always emphasize)
1. Healthcare-only focus
2. AHCA compliance expertise
3. 4-hour emergency response
4. Digital documentation
5. Bilingual service

### Tone Examples
- **Confident:** "We guarantee AHCA compliance"
- **Warm:** "Your trusted healthcare power partner"
- **Urgent:** "Don't risk patient safety - call now"
- **Professional:** "Certified, licensed, and insured"

---

## 🖼️ Photography & Imagery

### Photo Style
- Bright, clean, professional
- Show real technicians at work
- Include diverse healthcare facilities
- Warm lighting (golden hour feel)
- Always show safety equipment

### Image Treatment
- Slight warm filter to match brand
- Rounded corners on all images
- Soft shadows for depth
- Never use stock photos of generic generators

### Icons
- Use emoji/symbols sparingly for digital
- Custom line icons for print materials
- Always match brand colors
- Maintain consistent stroke width

---

## 📱 Digital Applications

### Website
- Sticky navigation with blur effect
- Smooth scroll animations
- Mobile-first responsive design
- Fast loading (optimize all images)

### Email Signatures
```html
MedGuard Power Services
[Name] | [Title]
📞 (305) XXX-XXXX
📧 name@medguardpower.com
🚨 24/7 Emergency: (305) XXX-XXXX
```

### Social Media
- Profile: Logo on warm beige
- Cover: Miami skyline with generators
- Posts: Always include starburst element
- Hashtags: #MedGuardPower #AHCACompliance #MiamiGenerators

---

## ✅ Brand Checklist

Before publishing any material:
- [ ] Uses correct color palette
- [ ] Typography follows guidelines
- [ ] Logo has proper clear space
- [ ] Messaging emphasizes healthcare focus
- [ ] CTAs are clear and urgent
- [ ] Images are high quality and on-brand
- [ ] Accessibility standards met (contrast, alt text)
- [ ] Mobile responsive
- [ ] Includes emergency contact info
- [ ] Maintains Miami retro warmth

---

## 🚫 What to Avoid

- ❌ Cold, corporate messaging
- ❌ Generic stock photos
- ❌ Too many fonts (max 2)
- ❌ Cluttered layouts
- ❌ Small, hard-to-read text
- ❌ Forgetting the starburst icon
- ❌ Using competitor colors (blue/yellow)
- ❌ Overly technical jargon

---

## 📊 Implementation Priority

1. **Immediate:** Update website with new styles
2. **This Week:** Apply to all sales materials
3. **This Month:** Business cards, vehicle wraps
4. **Ongoing:** Maintain consistency across all touchpoints

---

*Brand Book Version 1.0 - January 2025*
*MedGuard Power - Where Healthcare Meets Reliability*