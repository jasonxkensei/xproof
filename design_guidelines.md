# ProofMint Design Guidelines

## Design Approach

**Selected Approach:** Design System (Utility-Focused) with Premium Trust Elements

**Justification:** ProofMint is a professional certification tool requiring credibility and ease of use. The interface must inspire trust while remaining accessible to non-technical users. Drawing from enterprise design patterns (Stripe's clarity, Linear's typography, Notion's clean interfaces) while maintaining a distinctive "proof-centric" identity.

**Core Principle:** "Professional legitimacy meets Web3 simplicity" - The interface should feel like a legal certification tool, not a crypto experiment.

## Color Palette

### Dark Mode (Primary)
- **Background Base:** 0 0% 8% (deep charcoal)
- **Surface:** 0 0% 12% (elevated cards)
- **Primary Brand:** 160 84% 39% (emerald - MultiversX inspired)
- **Text Primary:** 0 0% 98%
- **Text Secondary:** 0 0% 65%
- **Border Subtle:** 0 0% 18%
- **Success/Verified:** 142 76% 36% (green certification indicator)

### Light Mode
- **Background Base:** 0 0% 98%
- **Surface:** 0 0% 100%
- **Primary Brand:** 160 84% 39% (consistent emerald)
- **Text Primary:** 0 0% 10%
- **Text Secondary:** 0 0% 40%

**Accent Usage:** Emerald green used sparingly for CTAs, verification badges, and certification status indicators. No secondary accent colors to maintain professional focus.

## Typography

**Font Stack:**
- **Primary:** Space Grotesk (headings, navigation) - modern, distinctive, Web3-aligned
- **Secondary:** Inter (body, forms, data) - clean, highly legible, professional

**Scale:**
- **Hero Heading:** text-6xl font-bold (60px) - landing page impact
- **Section Headings:** text-3xl font-semibold (30px)
- **Card Titles:** text-xl font-medium (20px)
- **Body Text:** text-base (16px) - optimal readability
- **Metadata/Labels:** text-sm text-secondary (14px)
- **Micro Copy:** text-xs (12px) - timestamps, hash displays

## Layout System

**Spacing Primitives:** Use Tailwind units of 4, 6, 8, 12, 16, 24 (p-4, gap-6, my-8, py-12, etc.)

**Container Strategy:**
- **Full-width sections:** w-full with inner max-w-7xl mx-auto px-6
- **Content areas:** max-w-6xl mx-auto
- **Dashboard content:** max-w-5xl
- **Forms:** max-w-2xl

**Grid Patterns:**
- **Features:** grid-cols-1 md:grid-cols-3 gap-8
- **Dashboard cards:** grid-cols-1 lg:grid-cols-2 gap-6
- **Certification history:** Single column with horizontal card layout

## Component Library

### Navigation
- **Top Bar:** Sticky header with logo left, nav center, CTA/user menu right
- **Logo:** "ProofMint" wordmark with seal icon, emerald accent on hover
- **Nav Links:** Clean text links with subtle underline on hover
- **CTA Button:** Primary emerald button "Start Free Trial"

### Core UI Elements

**Upload Zone:**
- Large dashed border box with emerald accent on drag-over
- Center-aligned icon (document with shield/checkmark)
- "Drop your file here or click to browse" text
- Supported formats displayed below
- Progress bar with emerald fill during upload

**Certification Cards (Dashboard):**
- White/dark surface with subtle border
- Left: File type icon with emerald background
- Center: Filename, date, hash preview (truncated with tooltip)
- Right: Status badge + action menu (download certificate, view proof)
- Transaction link with external icon

**Proof Verification Display:**
- Hero section with large verification seal icon
- Filename display (non-downloadable)
- Hash shown in monospace font with copy button
- Timestamp with calendar icon
- Prominent "View on MultiversX Explorer" button
- Certificate download CTA

**Pricing Cards:**
- Three-column layout (Free, Pro, Business)
- Emerald highlight on recommended plan
- Clear feature list with checkmarks
- Pricing displayed prominently
- "Start Plan" CTA button
- Enterprise as separate contact card

### Forms
- Clean input fields with emerald focus rings
- Labels above inputs, help text below
- File upload with drag-drop zone
- Author name/signature input with character count
- Submit buttons in emerald with loading states

### Data Display
- **Transaction Hashes:** Monospace font, truncated with expand/copy
- **Timestamps:** Relative time with absolute tooltip
- **Status Badges:** Pill-shaped with icon (Verified, Pending, Failed)
- **QR Codes:** Generated dynamically, placed on certificates and public proof pages

### Overlays
- **Modals:** Centered with backdrop blur, max-w-lg
- **Toast Notifications:** Top-right, emerald for success, red for errors
- **Certificate Preview:** Modal with PDF viewer before download

## Landing Page Strategy

**Hero Section (80vh):**
- Split layout: Left side with heading, tagline, CTA; Right side with animated certification flow visualization
- Heading: "Certify what you create. In one click."
- Subheading: "Blockchain-secured proof of ownership. No coding required."
- Primary CTA: "Certify Your First File Free" (emerald)
- Trust indicator: "Powered by MultiversX Truth Machine" with logo

**How It Works (3 Steps):**
- Horizontal timeline with numbered circles
- Upload → Hash → Certify workflow
- Visual icons for each step
- Brief explanatory text

**Benefits Grid:**
- Three columns: 🔒 Immutable Proof | ⚡ Instant Certification | 🧾 Public Verification
- Each with icon, heading, description

**Use Cases:**
- Target audience showcase: Designers, Lawyers, Musicians, Agencies
- Card layout with profession icon and specific use case

**Pricing Preview:**
- Simplified tier comparison
- "View All Plans" link to dedicated pricing page

**Trust Section:**
- "Built on MultiversX" branding
- Blockchain verification explanation
- Security reassurance

**Footer:**
- Dark background with emerald accents
- Quick links, API documentation, social media
- Newsletter signup: "Get updates on blockchain certification"

## Images

**Hero Image:** Abstract visualization of blockchain verification - geometric patterns forming a certification seal, emerald accents on dark background. Right side of hero split layout.

**How It Works Illustrations:** Three sequential isometric illustrations showing file upload, hash computation, and blockchain certification process.

**Use Case Images:** Professional stock photos of target users (designer at desk, lawyer reviewing documents, musician with headphones) - authentic, diverse, modern workplace settings.

## Animations

**Minimal and Purposeful:**
- Upload zone: Subtle bounce on drag-over
- Certification complete: Checkmark animation (1 second)
- Transaction confirmation: Pulse effect on verification badge
- Page transitions: Smooth fade (300ms)

**No Distracting Effects:** No parallax scrolling, no floating elements, no constant motion.