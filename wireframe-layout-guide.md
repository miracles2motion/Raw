# Wireframe & Layout Guide: Virtual Home Staging Landing Page

## Design System Foundation

### Grid System
- **Desktop:** 12-column grid, 1440px max-width container
- **Tablet:** 8-column grid, 768px breakpoint
- **Mobile:** 4-column grid, 375px min-width
- **Gutter:** 24px desktop, 16px mobile
- **Margin:** 80px desktop, 40px tablet, 20px mobile

### Spacing Scale
- **XXS:** 4px (icon padding, tight spacing)
- **XS:** 8px (button padding, form fields)
- **SM:** 16px (card padding, element spacing)
- **MD:** 24px (section internal spacing)
- **LG:** 40px (between content blocks)
- **XL:** 64px (between major sections desktop)
- **XXL:** 96px (hero to next section)

### Typography Scale
**Headlines:**
- H1: 64px / 72px line-height / -1px letter-spacing (Desktop Hero)
- H2: 48px / 56px / -0.5px (Section Headers)
- H3: 32px / 40px / 0px (Subsections)
- H4: 24px / 32px / 0px (Card Titles)

**Body:**
- Large: 20px / 32px / 0px (Hero subheadline)
- Regular: 16px / 28px / 0px (Body copy)
- Small: 14px / 24px / 0px (Captions, labels)

**Font Pairing:**
- Headlines: Inter Bold / Montserrat Bold / DM Sans Bold
- Body: Inter Regular / Open Sans / DM Sans Regular

### Color System
**Primary Brand:**
- Primary-900: #1A365D (Dark navy - headers)
- Primary-600: #2D3748 (Medium - body text)
- Primary-400: #4A5568 (Light - secondary text)

**Accent:**
- Accent-600: #3182CE (Blue - primary CTA)
- Accent-500: #4299E1 (Hover state)
- Success-500: #48BB78 (Green - success states)

**Neutrals:**
- White: #FFFFFF (Backgrounds)
- Gray-50: #F7FAFC (Alternate sections)
- Gray-100: #EDF2F7 (Borders, dividers)
- Gray-800: #1A202C (Text)

### Component Library

**Buttons:**
```
Primary CTA:
- Size: 56px height × 200px width (desktop)
- Padding: 16px 32px
- Border-radius: 8px
- Font: 16px bold
- Shadow: 0 4px 12px rgba(49, 130, 206, 0.3)
- Hover: Scale(1.02), shadow deepens
- Active: Scale(0.98)

Secondary Button:
- Size: 48px height
- Border: 2px solid Primary-600
- Background: Transparent
- Hover: Background fills with Primary-50
```

**Cards:**
```
Standard Card:
- Border-radius: 12px
- Padding: 32px
- Shadow: 0 2px 8px rgba(0,0,0,0.08)
- Hover: Shadow lifts to 0 8px 24px rgba(0,0,0,0.12)
- Transition: all 0.3s ease
```

**Input Fields:**
```
Form Input:
- Height: 48px
- Border: 1px solid Gray-200
- Border-radius: 6px
- Padding: 12px 16px
- Focus: Border Primary-400, shadow glow
```

---

## Section-by-Section Layouts

## Section 1: Hero Section (Above the Fold)

### Desktop Layout (1440px)
```
┌─────────────────────────────────────────────────────────────┐
│  LOGO              Nav: Features Pricing Gallery Contact    │ 80px height
├─────────────────────────────────────────────────────────────┤
│                                                               │
│  [LEFT COLUMN - 50%]                [RIGHT COLUMN - 50%]     │
│                                                               │
│  H1: Sell Your Listings           [HERO IMAGE/ANIMATION]    │
│  50% Faster with                  ┌─────────────────────┐   │
│  AI-Powered Staging               │                     │   │
│                                    │  Before/After       │   │
│  Subheadline (20px):              │  Interactive        │   │
│  Upload photos of empty            │  Slider             │   │
│  properties and receive            │                     │   │
│  high-end furnished renders        │  [Drag Handle]      │   │
│  within 24 hours                   │                     │   │
│                                    └─────────────────────┘   │
│  [PRIMARY CTA BUTTON]                                        │
│  Upload Your First Photo Free      Trust Elements:          │
│                                    5,000+ Realtors           │
│  Secondary text:                   ⭐⭐⭐⭐⭐ 4.9/5          │
│  No credit card required                                     │
│                                                               │
└─────────────────────────────────────────────────────────────┘
                        600px viewport height
```

### Component Specifications:

**Hero Image Container:**
- Width: 600px
- Height: 500px
- Border-radius: 16px
- Shadow: 0 20px 40px rgba(0,0,0,0.15)
- Contains: Interactive before/after slider

**Slider Functionality:**
- Vertical divider line at 50%
- Drag handle (circular, 60px diameter)
- Left side: Empty room photo (grayscale filter)
- Right side: Staged room photo (color)
- Smooth drag with momentum

**CTA Button:**
- Width: 280px
- Height: 56px
- Position: 40px below subheadline
- Micro-animation: Gentle pulse every 3 seconds

**Trust Badges:**
- Position: Below CTA, 24px spacing
- Layout: Horizontal row, 16px gaps
- Size: 80px × 24px each badge

### Mobile Layout (375px)
```
┌─────────────────────┐
│ ☰  LOGO             │ 60px
├─────────────────────┤
│                     │
│ [HERO IMAGE]        │ 300px
│ Before/After        │
│ Slider Full Width   │
│                     │
├─────────────────────┤
│ H1: (48px)          │
│ Sell Your Listings  │
│ 50% Faster          │
│                     │
│ Subheadline (18px)  │
│ 3 lines max         │
│                     │
│ [CTA - Full Width]  │ 52px
│                     │
│ Trust badges        │
│ (stacked 2×2)       │
└─────────────────────┘
```

---

## Section 2: Social Proof Bar

### Layout
```
┌─────────────────────────────────────────────────────────────┐
│                     CENTERED CONTENT                          │
│  ───────────────────────────────────────────────────────────│
│                                                               │
│    [Logo 1]  [Logo 2]  [Logo 3]  [Logo 4]  [Logo 5]         │
│    Realtor   Century   Coldwell  Sotheby's  Keller          │
│    .com      21        Banker    Realty     Williams        │
│                                                               │
│  "Trusted by 5,000+ real estate professionals"               │
│                                                               │
└─────────────────────────────────────────────────────────────┘
                        120px height
```

**Specifications:**
- Background: Gray-50
- Logos: Grayscale, 40px height
- Spacing: 60px between logos
- Animation: Fade in on scroll

---

## Section 3: Before & After Gallery

### Desktop Layout
```
┌─────────────────────────────────────────────────────────────┐
│                                                               │
│              H2: See the Transformation                       │
│         Sub: Real listings, real results                      │
│                                                               │
│  ┌───────────┐  ┌───────────┐  ┌───────────┐               │
│  │           │  │           │  │           │               │
│  │  Slider   │  │  Slider   │  │  Slider   │               │
│  │  Card 1   │  │  Card 2   │  │  Card 3   │               │
│  │           │  │           │  │           │               │
│  └───────────┘  └───────────┘  └───────────┘               │
│   Living Room     Bedroom       Kitchen                      │
│   Modern          Scandinavian   Contemporary                │
│                                                               │
│  ┌───────────┐  ┌───────────┐  ┌───────────┐               │
│  │  Slider   │  │  Slider   │  │  Slider   │               │
│  │  Card 4   │  │  Card 5   │  │  Card 6   │               │
│  └───────────┘  └───────────┘  └───────────┘               │
│                                                               │
│              [VIEW FULL GALLERY BUTTON]                       │
│                                                               │
└─────────────────────────────────────────────────────────────┘
```

### Gallery Card Specifications:
```
Card Dimensions:
- Width: 400px (desktop), 100% (mobile)
- Height: 300px (maintains 4:3 ratio)
- Border-radius: 12px
- Overflow: hidden (clips slider)

Card Content:
┌─────────────────┐
│                 │
│  [Image Slider] │ 260px
│                 │
├─────────────────┤
│  Living Room    │ 40px
│  Modern • 320sf │
└─────────────────┘

Grid Layout:
- Desktop: 3 columns × 2 rows
- Tablet: 2 columns × 3 rows
- Mobile: 1 column × 6 rows
- Gap: 32px desktop, 20px mobile
```

---

## Section 4: Style Gallery

### Layout
```
┌─────────────────────────────────────────────────────────────┐
│         H2: Every Buyer Has a Style. We Have Them All.       │
│                                                               │
│  ┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐               │
│  │        │ │        │ │        │ │        │               │
│  │ Modern │ │Scandi- │ │ Mid-   │ │Contem- │               │
│  │ Minim- │ │navian  │ │Century │ │porary  │               │
│  │ alist  │ │        │ │        │ │        │               │
│  │        │ │        │ │        │ │        │               │
│  │ [IMG]  │ │ [IMG]  │ │ [IMG]  │ │ [IMG]  │               │
│  └────────┘ └────────┘ └────────┘ └────────┘               │
│                                                               │
│  ┌────────┐ ┌────────┐ ┌────────┐ ┌────────┐               │
│  │Rustic  │ │Trad-   │ │Coastal │ │Indust- │               │
│  │Farm-   │ │itional │ │        │ │rial    │               │
│  │house   │ │        │ │        │ │        │               │
│  │ [IMG]  │ │ [IMG]  │ │ [IMG]  │ │ [IMG]  │               │
│  └────────┘ └────────┘ └────────┘ └────────┘               │
│                                                               │
└─────────────────────────────────────────────────────────────┘
```

### Style Card Specifications:
```
Desktop Card:
- Width: 280px
- Height: 320px
- Composition:
  ┌──────────┐
  │          │ Image: 280×240px
  │  [Image] │ Covers top 75%
  │          │
  ├──────────┤
  │  Style   │ Label: 80px height
  │  Name    │ Centered text
  └──────────┘

Hover State:
- Image: Brightness(1.1), Scale(1.05)
- Overlay appears: "View 12 Examples →"
- Transition: 0.4s ease-out

Grid:
- 4 columns × 2 rows (desktop)
- Gap: 24px
```

---

## Section 5: How It Works

### Layout
```
┌─────────────────────────────────────────────────────────────┐
│       H2: From Empty to Irresistible in 3 Simple Steps       │
│                                                               │
│    ┌────────┐            ┌────────┐            ┌────────┐   │
│    │   1    │ ────────→  │   2    │ ────────→  │   3    │   │
│    │ [Icon] │            │ [Icon] │            │ [Icon] │   │
│    │ Upload │            │ Choose │            │Download│   │
│    │ Photos │            │ Style  │            │& List  │   │
│    │        │            │        │            │        │   │
│    │  Text  │            │  Text  │            │  Text  │   │
│    │ (100w) │            │ (100w) │            │ (100w) │   │
│    └────────┘            └────────┘            └────────┘   │
│                                                               │
│           [START YOUR FREE TRIAL BUTTON]                      │
│                                                               │
└─────────────────────────────────────────────────────────────┘
```

### Step Card Specifications:
```
Card Layout:
┌──────────────┐
│   ┌──────┐   │ Number badge
│   │  1   │   │ 60px circle
│   └──────┘   │ Primary-600 bg
│              │
│   [Icon]     │ 80×80px icon
│   Upload     │ 
│              │
│   Headline   │ H4: 24px
│   Upload     │
│   Photos     │
│              │
│   Body (14px)│ 3 lines max
│   Drag and   │ Gray-600
│   drop your  │
│   photos...  │
└──────────────┘

Connecting Arrows:
- SVG arrow path
- Animated: Dashed line draws on scroll
- Color: Primary-400
- Width: 2px
```

### Mobile Stack:
```
┌─────────────┐
│    Step 1   │
│   [Icon]    │
│   Content   │
│      ↓      │ Vertical arrow
├─────────────┤
│    Step 2   │
│   [Icon]    │
│   Content   │
│      ↓      │
├─────────────┤
│    Step 3   │
│   [Icon]    │
│   Content   │
└─────────────┘
```

---

## Section 6: Pricing Table

### Desktop Layout
```
┌─────────────────────────────────────────────────────────────┐
│       H2: Professional Staging at a Fraction of the Cost     │
│            Sub: No subscriptions. Pay only for what you use  │
│                                                               │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐         │
│  │ Per Image   │  │ 5-Image Pkg │  │ 10-Image Pkg│         │
│  │             │  │             │  │             │         │
│  │    $29      │  │    $125     │  │    $220     │         │
│  │  per image  │  │  Save $20   │  │  Save $70   │         │
│  │             │  │             │  │             │         │
│  │ • Feature 1 │  │ • Feature 1 │  │ • Feature 1 │         │
│  │ • Feature 2 │  │ • Feature 2 │  │ • Feature 2 │         │
│  │ • Feature 3 │  │ • Feature 3 │  │ • Feature 3 │         │
│  │             │  │ • Feature 4 │  │ • Feature 4 │         │
│  │             │  │             │  │ • Feature 5 │         │
│  │             │  │             │  │             │         │
│  │  [BUTTON]   │  │  [BUTTON]   │  │  [BUTTON]   │         │
│  │  Try Free   │  │  Get Started│  │  Get Started│         │
│  │             │  │ ⭐ Popular  │  │             │         │
│  └─────────────┘  └─────────────┘  └─────────────┘         │
│                                                               │
│               Need 20+ images? [Get Custom Quote]            │
│                                                               │
└─────────────────────────────────────────────────────────────┘
```

### Pricing Card Specifications:
```
Card Dimensions:
- Width: 360px
- Height: 560px (equal height all cards)
- Border: 1px solid Gray-200
- Border-radius: 16px
- Padding: 40px 32px

Popular Badge:
- Position: Absolute top-right
- Size: 100px × 32px
- Background: Accent-500
- Border-radius: 16px 16px 0 0
- Text: White, 14px bold

Price Display:
- Font-size: 48px bold
- Line-height: 1
- Margin-bottom: 8px
- Secondary text: 16px, Gray-600

Feature List:
- Spacing: 16px between items
- Checkmark icon: 20px, Success-500
- Text: 16px, Gray-700
- Min 5 items (use "—" for missing features)

CTA Button:
- Full width minus padding
- Height: 48px
- Border-radius: 8px
- Hover: Lift effect

Middle Card (Popular):
- Scale: 1.05 (slightly larger)
- Shadow: Deeper than others
- Border: 2px solid Accent-500
```

---

## Section 7: FAQ Accordion

### Layout
```
┌─────────────────────────────────────────────────────────────┐
│                H2: Frequently Asked Questions                 │
│                                                               │
│  ┌───────────────────────────────────────────────────────┐  │
│  │ ▼ Is this legal/ethical in my market?                 │  │
│  │                                                        │  │
│  │   Answer text appears here when expanded...           │  │
│  │   Multiple paragraphs supported...                    │  │
│  │                                                        │  │
│  └───────────────────────────────────────────────────────┘  │
│                                                               │
│  ┌───────────────────────────────────────────────────────┐  │
│  │ ▶ What photo quality do I need?                       │  │
│  └───────────────────────────────────────────────────────┘  │
│                                                               │
│  ┌───────────────────────────────────────────────────────┐  │
│  │ ▶ Can you stage outdoor spaces?                       │  │
│  └───────────────────────────────────────────────────────┘  │
│                                                               │
│  ┌───────────────────────────────────────────────────────┐  │
│  │ ▶ Do you offer floor plan rendering?                  │  │
│  └───────────────────────────────────────────────────────┘  │
│                                                               │
│  ┌───────────────────────────────────────────────────────┐  │
│  │ ▶ How long does rush delivery take?                   │  │
│  └───────────────────────────────────────────────────────┘  │
│                                                               │
└─────────────────────────────────────────────────────────────┘
```

### Accordion Specifications:
```
Container:
- Max-width: 800px (centered)
- Gap between items: 16px

Accordion Item (Closed):
┌────────────────────────────────┐
│ ▶ Question text           [▼] │ 64px height
└────────────────────────────────┘
- Background: White
- Border: 1px solid Gray-200
- Border-radius: 8px
- Padding: 20px 24px

Accordion Item (Open):
┌────────────────────────────────┐
│ ▼ Question text           [▲] │
├────────────────────────────────┤
│                                │
│ Answer text with proper        │
│ line height and spacing.       │
│                                │
│ Can include multiple           │
│ paragraphs.                    │
│                                │
└────────────────────────────────┘
- Border color: Accent-500 (when open)
- Answer padding: 0 24px 24px 24px
- Animation: Height transition 0.3s ease

Icon States:
- Closed: ▶ (or chevron-right)
- Open: ▼ (or chevron-down)
- Size: 20px
- Color: Primary-600
- Position: Absolute right 24px
```

---

## Section 8: Final CTA (Full-Width)

### Layout
```
┌─────────────────────────────────────────────────────────────┐
│                                                               │
│                   CENTERED CONTENT                            │
│                                                               │
│              H2: Ready to Transform Your Listing?             │
│                                                               │
│         Upload your first photo absolutely free—              │
│                see the magic yourself                         │
│                                                               │
│              [LARGE CTA BUTTON: Try It Free]                  │
│                  (No Credit Card Required)                    │
│                                                               │
│    ───────────────────────────────────────────────────       │
│                                                               │
│   [Icon] 5,000+    [Icon] 100,000+    [Icon] 4.9/5          │
│    Agents           Rooms Staged        Rating               │
│                                                               │
└─────────────────────────────────────────────────────────────┘
                   Background: Gradient or Image
                   Height: 400px
```

### Specifications:
```
Section Background:
- Option 1: Gradient (Primary-900 to Primary-600)
- Option 2: Background image with dark overlay
- Text color: White

CTA Button:
- Width: 320px
- Height: 64px
- Font-size: 18px bold
- Background: White
- Text color: Primary-900
- Shadow: 0 8px 24px rgba(0,0,0,0.2)
- Hover: Scale(1.05)

Trust Stats:
- Layout: 3 columns, equal width
- Icon: 40px, White
- Number: 32px bold, White
- Label: 14px, White opacity 80%
- Spacing: 48px gaps
```

---

## Footer

### Layout
```
┌─────────────────────────────────────────────────────────────┐
│                                                               │
│  [LOGO]                                                       │
│                                                               │
│  Product        Company        Resources        Legal         │
│  • Features     • About        • Blog           • Terms       │
│  • Pricing      • Team         • Help Center    • Privacy     │
│  • Gallery      • Careers      • Contact        • Cookies     │
│  • API          • Press        • FAQ                          │
│                                                               │
│  ───────────────────────────────────────────────────────────│
│                                                               │
│  [Social Icons: LinkedIn Instagram Twitter Facebook]         │
│                                                               │
│  © 2026 Virtual Staging Co. All rights reserved.             │
│                                                               │
└─────────────────────────────────────────────────────────────┘
```

---

## Responsive Breakpoints

### Desktop Large (1440px+)
- Max container: 1280px
- All elements full size
- 3-column layouts

### Desktop (1024px - 1439px)
- Max container: 960px
- Slightly reduced spacing
- 3-column layouts maintained

### Tablet (768px - 1023px)
- Full-width container with 40px margins
- 2-column layouts
- Reduced font sizes (H1: 48px)

### Mobile (375px - 767px)
- Full-width with 20px margins
- Single column layouts
- Stacked navigation
- Reduced spacing (XL: 40px, XXL: 64px)
- H1: 36px, H2: 32px

---

## Interaction States

### Buttons
```
Default:
- Background: Accent-600
- Text: White
- Shadow: 0 4px 12px rgba(49,130,206,0.3)

Hover:
- Background: Accent-500
- Transform: Scale(1.02) TranslateY(-2px)
- Shadow: 0 8px 20px rgba(49,130,206,0.4)

Active:
- Transform: Scale(0.98)
- Shadow: 0 2px 8px rgba(49,130,206,0.3)

Disabled:
- Background: Gray-300
- Text: Gray-500
- Cursor: not-allowed
- No shadow
```

### Cards
```
Default:
- Shadow: 0 2px 8px rgba(0,0,0,0.08)
- Transform: none

Hover:
- Shadow: 0 8px 24px rgba(0,0,0,0.12)
- Transform: TranslateY(-4px)
- Transition: all 0.3s ease

Click/Active:
- Border: 2px solid Accent-500
- Shadow: 0 4px 16px rgba(49,130,206,0.2)
```

### Links
```
Default:
- Color: Accent-600
- Text-decoration: none

Hover:
- Color: Accent-700
- Text-decoration: underline

Visited:
- Color: Accent-800

Focus:
- Outline: 2px solid Accent-400
- Outline-offset: 2px
```

---

## Accessibility Specifications

### Color Contrast
- All text: Minimum 4.5:1 ratio
- Large text (18px+): Minimum 3:1 ratio
- Interactive elements: Clear focus states

### Keyboard Navigation
- Tab order: Logical flow top to bottom
- Focus indicators: Visible on all interactive elements
- Skip links: "Skip to main content"

### Screen Readers
- Alt text: All images (descriptive, concise)
- ARIA labels: Complex interactions
- Semantic HTML: Proper heading hierarchy
- Form labels: Explicit associations

### Motion
- Respect prefers-reduced-motion
- Provide pause controls for auto-play
- No flashing content > 3 times per second

---

## Performance Optimization

### Image Strategy
- Hero: WebP format, 1200×800px max
- Gallery: Lazy loading, 800×600px
- Thumbnails: 400×300px
- Retina: @2x versions for displays > 2x density

### Loading Priority
1. Hero section (above fold)
2. Critical CSS inline
3. Defer non-critical JavaScript
4. Lazy load images below fold
5. Preconnect to external fonts

### File Sizes
- Hero image: < 300KB
- Gallery images: < 150KB each
- Total CSS: < 50KB
- Critical CSS: < 10KB
- Total JS (initial): < 100KB

This comprehensive wireframe guide gives you exact specifications for implementing the Virtual Home Staging landing page design!