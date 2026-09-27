# Nova Visual Platform

> **See Beyond the Feed** — An intentional visual discovery, curation, and creator economy platform designed for visual directors, photographers, architects, and discerning curators.

---

## 🌟 Overview

**Nova Visual Platform** is an immersive, high-fidelity visual social ecosystem built as a modern alternative to traditional algorithmic dopamine loops. Designed around architectural minimalism and visual purity, Nova combines thematic world discovery, multi-faceted collection curation, creator sovereignty, direct monetization, and visual lineage tracking into a seamless, zero-dependency Single-Page Application (SPA).

Built with pure vanilla web technologies (HTML5, CSS3, and modern JavaScript), Nova runs entirely in the browser with persistent client-side state storage, high-resolution visual rendering, client-side EXIF GPS extraction, real-time interactive discussions, and an integrated Creator Studio equipped with dynamic SVG analytics.

---

## ✨ Features

### 1. Intentional Visual Discovery & Feed Modes
- **Thematic Visual Worlds**: 8 distinct creative domains mapped by aesthetic harmony:
  - Architecture *(Liminal spaces, concrete brutalism, geometric light)*
  - Photography *(Monochrome street, nocturnal Tokyo, 35mm analog grain)*
  - Travel *(Terracotta deserts, subarctic Scandinavian fjords, solitary destinations)*
  - Design *(Bauhaus typography, stoneware ceramics, industrial CNC forms)*
  - Fashion *(Architectural draping, technical outerwear, sculptural silhouettes)*
  - AI Art *(Latent topology, synthetic minerals, procedural biology)*
  - Nature *(Bioluminescent flora, basalt columns, glacial melt patterns)*
  - Technology *(Quantum lattices, fiber optic refraction, frosted hardware)*
- **Multi-Faceted Feed Filtering**: Switch between **For You**, **Following**, **Fresh**, **Trending**, and **Nearby** streams.
- **Interactive Visual Cards**: High-resolution immersive card presentation with reaction appreciation, discussion counts, collection clipping, quick sharing, and direct creator tipping.
- **"Inspired By" Visual Lineage**: Relational graph connections tracing contemporary artistic responses, derivative works, and creative lineage.

### 2. Dedicated Search & Faceted Exploration
- Real-time client-side search across **Visuals**, **Creators**, and **Collections**.
- One-click trending topic tags (`#Architecture`, `#Tokyo`, `#Portraits`, `#Minimalism`, `#Design`, etc.).
- Informative zero-result states with smart search term recommendations.
- Global keyboard navigation shortcut (`/` to focus search, `Escape` to dismiss overlays).

### 3. Visual Collections & Collaborative Worlds
- Organize visual studies into thematic collections with privacy controls (**Public**, **Private**).
- Support for **Collaborative Worlds** allowing multiple curators to co-curate collections.
- Inline collection creation and single-click asset assignment.

### 4. Create Studio & Upload Engine
- Side-by-side live card preview updated in real-time as metadata is entered.
- Drag-and-drop / file upload dropzone with automated visual title extraction from image filenames.
- **Client-Side EXIF GPS Parser**: Automatically inspects uploaded JPEG binary headers and parses GPS coordinate metadata for accurate location suggestions without server-side processing.
- Discipline categorization, location context, collection assignment, and monetization flags (tipping, subscriber exclusivity).

### 5. Creator Studio & Analytics Dashboard
- Comprehensive creator performance metrics:
  - Total Visual Views & monthly growth attribution.
  - Engagement resonance percentage.
  - Available and pending wallet balances.
  - Active subscriber counts.
- **Pure SVG Audience Impression Chart**: Interactive time-series area chart with timeframe filters (**7D**, **30D**, **90D**).
- **Pure SVG Revenue Diversification Donut**: Visual breakdown across Brand Collabs, Monthly Subscriptions, Direct Tips, and Paid Collections.
- Top-performing visual rankings with view-to-discussion metrics.

### 6. Creator Monetization & Treasury Wallet
- **Patron Tipping**: Direct creator appreciation with preset (`₹50`, `₹100`, `₹250`, `₹500`) and custom amounts, complete with personal notes.
- **Studio Circle Subscriptions**: Recurring creator memberships granting exclusive access to high-res archives, behind-the-scenes studies, and distinctive glowing patron badges.
- **Creator Treasury Wallet**: Live balance tracking with simulated instant bank withdrawals (UPI / IMPS).
- **Brand Marketplace**: Commercial campaign directory with detailed briefs (budgets, deadlines, requirements, deliverables) and creative proposal submission workflows.

### 7. Real-Time Chat & Activity Center
- **Direct Messaging**: In-app messenger with active conversation threads, unread message badges, and simulated contextual creator replies.
- **Notification Center**: Real-time notifications categorized into **Social**, **Creator**, and **Earnings**, with unread status indicators and mark-all-read controls.

### 8. User Identity & Persona Switching
- Multi-persona simulation system:
  - **Renu Sri** — Verified Creator (Tokyo, Japan)
  - **Alex Rivera** — Visual Collector (San Francisco, USA)
  - **Aether Studio** — Official Brand & Hardware Studio (Berlin, Germany)
  - **Guest Mode** — Unauthenticated read-only browsing mode with sign-in prompts
- Comprehensive user profiles with follower and following statistics bars and interactive user list modals.
- Obsidian Dark (`--bg-primary: #080A0F`) and Lumina Light mode themes.
- Client-side session persistence via browser `localStorage`.

---

## 🛠️ Technology Stack

| Layer | Technology | Details |
| :--- | :--- | :--- |
| **Markup** | HTML5 | Semantic architecture (`<nav>`, `<aside>`, `<main>`, `<header>`, `<footer>`, `<dialog>`, `<svg>`) |
| **Styling** | CSS3 | CSS Custom Properties (Theme tokens), CSS Grid, Flexbox, Glassmorphism backdrop filters |
| **Logic** | Vanilla JavaScript (ES6+) | Modern asynchronous event-driven architecture, zero external dependencies |
| **Router** | Client-Side Hash Router | SPA navigation (`#/home`, `#/discover`, `#/search`, `#/visual/:id`, etc.) |
| **State Storage** | `localStorage` API | Reactive persistent state store (`nova_state_v1`, `nova_session_user_id`) |
| **Binary Parser** | ArrayBuffer & DataView | Client-side EXIF APP1 parser for JPEG GPS coordinates extraction |
| **Visual Assets** | Inline SVG & Unsplash | Optimized vector iconography, linear gradients, and curated CDN photography |

---

## 📋 Prerequisites

To run Nova Visual Platform, all you need is a modern web browser:
- Google Chrome (version 90+)
- Mozilla Firefox (version 88+)
- Microsoft Edge (version 90+)
- Apple Safari (version 14+)

*No Node.js, Python, package managers, or compilers are required for running the application.*

---

## 🚀 Installation & Run Commands

### Method 1: Direct File Execution (Quickest)
Simply double-click `index.html` (or `Nova-Visual-Platform.html`) to open the platform directly in your default browser.

```bash
# On Windows (PowerShell)
Start-Process .\index.html

# On macOS
open index.html

# On Linux
xdg-open index.html
```

---

### Method 2: Local HTTP Server (Recommended)

Running through a local web server provides the smoothest performance and ensures standard browser security policies for local storage and image rendering.

#### Using Python 3:
```bash
# Start a local HTTP server on port 8000
python -m http.server 8000

# Open http://localhost:8000 in your browser
```

#### Using Node.js (`npx serve`):
```bash
# Serve the repository root
npx serve .

# Open the displayed localhost URL (typically http://localhost:3000)
```

#### Using VS Code Live Server:
1. Open the `Nova-Visual-Platform` folder in VS Code.
2. Right-click `index.html` and select **"Open with Live Server"**.

---

## 🔨 Build Instructions

**No build step is required.**

Nova Visual Platform is architected as a complete, self-contained single-page web application. All styles, templates, datasets, and controllers are bundled into a cohesive architecture that executes directly in standard JavaScript runtimes.

---

## 📁 Project Structure

```
Nova-Visual-Platform/
├── .gitignore                  # Production Git ignore rules (OS, editors, env, dependencies)
├── README.md                   # Comprehensive project documentation
├── index.html                  # Main application entry point for static hosts & GitHub Pages
└── Nova-Visual-Platform.html   # Standalone platform bundle
```

### Key Components within the Application Bundle:
- **Design System (`<style>`):** CSS variable design tokens defining the Obsidian Dark and Lumina Light palettes, typography, glassmorphism, responsive breakpoints, and animations.
- **SVG Symbols & Filters:** Embedded scalable graphics for branding marks, directional navigation arrows, and gradient definitions.
- **Application Shell:** Responsive dual-layout featuring a fixed desktop sidebar, sticky blur header, and mobile bottom navigation bar.
- **Seeded Dataset (`INITIAL_DATA`):** 50 user profiles, 200 high-resolution visual studies, 30 curated collections, 120 discussions, commercial brand briefs, messages, notifications, and ledger entries.
- **Platform Application Engine:**
  - `initAppState()`: State hydrator with automated version migration and localStorage sync.
  - `renderCurrentRoute()`: Central hash-based router handling 26 unique view states.
  - `openModal()` / `closeModal()`: Modular accessible dialog manager.
  - `extractGpsFromExif()`: Binary ArrayBuffer / DataView parser for image EXIF metadata.
  - `showToast()`: Floating notification alert system.

---

## ⚙️ Configuration & Environment Notes

- **Persistent Client Storage**: Nova saves session data, profile customizations, uploaded visuals, reactions, and saved collections to `localStorage` under keys `nova_state_v1` and `nova_session_user_id`.
- **Resetting Demonstration Data**: To return the platform to its pristine initial seed state:
  - Open **Settings** (`#/settings`) from the user menu.
  - Scroll down to **Clear Demo Data** and click **"Reset Demo to Fresh Dataset"**.
  - Alternatively, run `localStorage.clear()` in your browser developer tools console and refresh.
- **Preconfigured Demo Personas**:
  - **Renu Sri (Creator)**: Verified Creator with active Creator Studio and Treasury Wallet.
  - **Alex Rivera (Personal)**: Minimalist collector and curator.
  - **Aether Studio (Brand)**: Official brand partner managing spatial design campaigns.
  - **Guest Mode**: Unauthenticated state with read-only feed browsing.
- **Security & Privacy Note**: All authentication, tipping, and payout mechanisms operate in demo sandbox mode. No real monetary transactions or external server transmissions take place.

---

## 🤝 Contribution Guidance

Contributions to enhance Nova Visual Platform are welcome! Follow these steps to contribute:

1. **Fork the Repository**:
   Click the **Fork** button at the top right of this page.
2. **Clone your Fork**:
   ```bash
   git clone https://github.com/renusrisai29/Nova-Visual-Platform.git
   cd Nova-Visual-Platform
   ```
3. **Create a Feature Branch**:
   ```bash
   git checkout -b feature/enhanced-visual-filters
   ```
4. **Make Your Changes**:
   Adhere to clean code practices, maintain semantic HTML structure, and test across both desktop and mobile viewports.
5. **Verify Compatibility**:
   Ensure both `index.html` and `Nova-Visual-Platform.html` remain in sync and run cleanly without console errors.
6. **Commit & Push**:
   ```bash
   git commit -m "Add enhanced visual filters to Discover feed"
   git push origin feature/enhanced-visual-filters
   ```
7. **Open a Pull Request**:
   Describe your changes, features added, and any design considerations.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

```
MIT License

Copyright (c) 2026 Nova Visual Platform

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
