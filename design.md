# Design Specification: Building Singapore's Quantum-Safe Future

This document details the layout, visual design, and content architecture for the static web page **"Building Singapore's Quantum-Safe Future"**. The page is designed to highlight Singapore's transition and initiatives in safeguarding digital infrastructure against future quantum computer threats.

---

## 1. Visual Theme & Color Palette

The main visual theme is **Futuristic, High-Tech, and Secure**, utilizing a crisp, modern **light theme with a deep purple and violet aesthetic** that matches the advanced feel of quantum computing and cryptography.

### Color Codes
- **Background / Primary Light**: `#f8f9fc` (Clean off-white slate)
- **Secondary Light / Section Backgrounds**: `#ffffff` (Pure White)
- **Main Theme Accent**: `#6929c4` (Deep Purple Accent)
- **Secondary Theme Accent / Highlights**: `#8a3ffc` (Vibrant Quantum Purple)
- **Subtle Highlight / Hover states**: `#f1ecfe` (Soft Purple Mist)
- **Text Primary**: `#161616` (Deep Charcoal Black for superior readability)
- **Text Secondary**: `#525252` (Slate Gray)
- **Card Background (Glassmorphism)**: `rgba(255, 255, 255, 0.75)` with border `rgba(105, 41, 196, 0.15)` and `backdrop-filter: blur(12px)`

### Typography
- **Headings**: Modern sans-serif with wide tracking (e.g., IBM Plex Sans, Inter, or system-ui)
- **Hero Title**: Bold weight (800), gradient fill transitioning from Purple-Blue to Lavender-Cyan.

---

## 2. Layout Structure (Single-Page)

The page will be structured as a responsive, modern single-page web portal. It contains the following main sections:

### Header / Navigation Bar
- **Logo / Brand**: "Singapore Quantum-Safe Portal" (With a stylized quantum-lock icon)
- **Navigation Links**: Overview, Key Pillars, Roadmap, Assessment, Resources
- **CTA Button**: "Get Assessment" (Sleek purple outline button with glowing hover effect)

### Hero Section (The Core Requirement)
- **Background Image**: `ibm_quantum_safe_4k_hero_05.png` as a full-viewport background with `background-attachment: fixed` or high-resolution cover layout.
- **Overlay**: A deep purple radial/linear gradient overlay (`linear-gradient(180deg, rgba(12, 5, 26, 0.4) 0%, rgba(12, 5, 26, 0.95) 100%)`) to guarantee excellent readability of text.
- **Content Block (Glassmorphism Glass Card)**:
  - **Pre-title**: "QUANTUM-SAFE SECURITY INITIATIVE" (Small caps, letter-spaced, soft lavender)
  - **Main Title**: "Building Singapore's Quantum-Safe Future" (Sleek, futuristic, prominent)
  - **Description**: "Preparing our nation’s critical infrastructure, financial networks, and public institutions for the post-quantum era with state-of-the-art cryptographic resilience."
  - **Primary CTA**: "Explore the Roadmap" (Solid purple background, smooth transition, glowing shadow)
  - **Secondary CTA**: "Read Whitepaper" (Translucent border button)

### Section 1: The Threat & The Mission (Briefing)
- Split grid layout:
  - **Left**: A narrative on "Why Quantum-Safe?" explaining Shor's algorithm and the threat to RSA/ECC.
  - **Right**: An interactive-looking metrics block (e.g., "Quantum Advantage Countdown", "1024-bit Vulnerability Level", "Target Transition: 2026-2030").

### Section 2: Core Strategic Pillar - Post-Quantum Cryptography (PQC)
A 3-part detailed focus on Singapore's software-based cryptographic transition:
1. **PQC Algorithm Transition**: Replacing vulnerable public-key suites (RSA/ECC) with NIST-vetted lattice-based cryptographic algorithms (such as ML-KEM for key establishment and ML-DSA for digital signatures).
2. **Cryptographic Agility**: Designing application architectures and protocols to dynamically hot-swap encryption suites without full infrastructure refactoring.
3. **PQC Discovery & Inventory Audits**: Proactively identifying, cataloging, and testing legacy asymmetric key vulnerabilities across databases, cloud, and edge systems.

### Section 3: Singapore's Cryptographic Transition Roadmap (Interactive Timeline)
A vertical or horizontal timeline highlighting key milestones aligned with the CSA Singapore Quantum-Safe Handbook:
- **Phase 1: Pilot & Collaboration (2024 - 2026)**: Actively launching pilot systems, testing and deploying PQC implementations with tier-1 telecom providers and trial partners.
- **Milestone 2: 31 March 2027 (Migration Blueprint Deadline)**: Target deadline for Critical Information Infrastructure (CII) owners to submit a comprehensive, multi-year quantum-safe migration plan to the Cyber Security Agency of Singapore (CSA).
- **Milestone 3: 1 January 2028 (Sovereign Readiness Mandate)**: All newly procured and implemented computer systems with a digital component must support quantum-safe technologies or be certified as quantum-safe ready.
- **Milestone 4: 31 December 2031 (Full Cryptographic Transition)**: Final target deadline to complete full quantum-safe migration across all CII systems, resulting in the complete retirement of vulnerable public-key cryptography (e.g., RSA, standard ECC) in active use.

### Section 4: Strategic Engagement & Collaboration (Coming Soon)
- Public pathway allowing Singapore organizations to verify readiness, attend executive briefings, join technical workshops, and collaborate on sandbox systems.
- Interested organizations can register via Microsoft Forms: `https://forms.cloud.microsoft/r/kVjashmpfn?origin=lprLink` to request briefings, workshops, pilot collaboration, or early sandbox access.

### Footer
- High-quality, minimalist footer featuring:
  - Explanatory note on Singapore's position in quantum tech.
  - Centered copyright section with a thin top border.

---

## 3. Implementation Details & Assets

- **Framework**: No complex frameworks. Pure HTML5, modern Tailwind CSS via CDN, and vanilla JavaScript.
- **Icons**: SVG icons embedded directly into the HTML to prevent external dependency failures and ensure lightning-fast rendering.
- **Fonts**: Pre-fetched from Google Fonts (Inter & JetBrains Mono for tech-themed items).
- **Responsive Web Design**:
  - Mobile-first approach using Tailwind classes (`md:grid-cols-3`, `px-6 lg:px-12`, etc.).
  - Navigation menu collapses into a responsive hamburger menu on smaller screens.
