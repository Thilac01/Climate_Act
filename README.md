# 🌍 ClimAct — SDG 13: Climate Action

<div align="center">

![ClimAct Banner](https://images.unsplash.com/photo-1470071459604-3b5ec3a7fe05?w=900&q=80)

**An interactive, educational web platform dedicated to UN Sustainable Development Goal 13: Climate Action.**

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](LICENSE)

*Built by students at the University of Westminster · © 2026*

</div>

---

## 📖 Table of Contents

- [About the Project](#-about-the-project)
- [Live Demo](#-live-demo)
- [Features](#-features)
- [Project Structure](#-project-structure)
- [Pages Overview](#-pages-overview)
- [Technical Details](#-technical-details)
- [Getting Started](#-getting-started)
- [Team](#-team)
- [Validation & Accessibility](#-validation--accessibility)
- [License](#-license)

---

## 🌱 About the Project

**ClimAct** is a fully static, client-side website built to raise awareness and inspire action around **UN SDG 13: Climate Action**. Developed collaboratively by a team of four students, it combines educational content, interactive tools, and a clean, accessible design to make climate literacy engaging for everyone.

The site explores four key pillars of climate action:
- 🌞 Renewable Energy
- 🚌 Sustainable Transport
- 🥦 Sustainable Food & Agriculture
- 🏠 Green Living at Home

---

## 🔗 Live Demo

> Open `splash.html` in any modern browser to launch the site. No server or build step required.

```
ClimAct/
└── splash.html  ← Start here
```

---

## ✨ Features

### ⚡ Action Impact Simulator (`ais.html`)
An interactive decision tool that lets users select from **8 real-world climate actions** and calculates a cumulative impact score in real time.

- **Dynamic visual feedback** — page background and panels transition through Red → Orange → Green based on score.
- **Instant scoring** — each choice updates the display immediately.
- Encourages users to reflect on the environmental weight of everyday decisions.

### 🖼️ Interactive Media Gallery (`gallery.html`)
A JavaScript-powered photo grid showcasing climate-related photography.

- **Live customisation** — users can change modal background colour, text colour, and font family in real time.
- Smooth animations and hover effects throughout.

### 📬 Feedback & Community Hub (`feedback.html`)
A two-part community engagement page.

- **Programme Directory** — a scrollable list of local climate initiatives (e.g. *Zero Waste Challenge*).
- **Feedback Form** — full client-side validation: required field checks, a 500-character live counter, and error messaging.

### 📚 Deep-Dive Content Pages (`content_ST1–4.html`)
Four in-depth articles on core sustainability topics, each researched and written by a dedicated team member.

### 👤 User Profile Page (`profile.html`)
A personalisation page where users can manage their preferences and track their engagement.

---

## 📂 Project Structure

```
Climate_Act/
│
├── 📄 splash.html              # Entry splash screen (auto-redirects to home)
├── 📄 home.html                # Main landing page with mission cards & gallery
├── 📄 sitemap.html             # Full site navigation directory
│
├── ── Interactive Tools ──
├── 📄 ais.html                 # Action Impact Simulator
├── 📄 gallery.html             # Photo gallery with customisation
├── 📄 feedback.html            # Community hub & feedback form
├── 📄 profile.html             # User profile page
├── 📄 team.html                # Meet the development team
│
├── ── Content Pages ──
├── 📄 content_ST1.html         # Renewable Energy Solutions
├── 📄 content_ST2.html         # Sustainable Transport
├── 📄 content_ST3.html         # Sustainable Food & Agriculture
├── 📄 content_ST4.html         # Green Living at Home
│
├── ── Developer Pages ──
├── 📄 pageEditor_ST1.html      # Technical editor notes — Student 1
├── 📄 pageEditor_ST2.html      # Technical editor notes — Student 2
├── 📄 pageEditor_ST3.html      # Technical editor notes — Student 3
├── 📄 pageEditor_ST4.html      # Technical editor notes — Student 4
│
├── ── Validation Reports ──
├── 📄 validation_ST1.html      # HTML/CSS validation report — Student 1
├── 📄 validation_ST2.html      # HTML/CSS validation report — Student 2
├── 📄 validation_ST3.html      # HTML/CSS validation report — Student 3
├── 📄 validation_ST4.html      # HTML/CSS validation report — Student 4
│
└── 🎨 style.css                # Global shared design system
```

---

## 📄 Pages Overview

| Page | File | Description | Author |
|---|---|---|---|
| Splash Screen | `splash.html` | Animated intro with auto-redirect | Shared |
| Home | `home.html` | Mission cards, hero, content gallery | Student 1 |
| Action Simulator | `ais.html` | Interactive climate impact calculator | Shared |
| Gallery | `gallery.html` | Customisable photo gallery | Shared |
| Feedback | `feedback.html` | Community directory + validated form | Shared |
| Profile | `profile.html` | User personalisation | Shared |
| Team | `team.html` | Team introduction page | Shared |
| Sitemap | `sitemap.html` | Full site navigation map | Shared |
| Renewable Energy | `content_ST1.html` | Solar, wind & hydro power | Student 1 |
| Sustainable Transport | `content_ST2.html` | EVs, cycling & public transport | Student 2 |
| Food & Agriculture | `content_ST3.html` | Plant-based diets, sustainable farming | Student 3 |
| Green Living | `content_ST4.html` | Home energy & water efficiency | Student 4 |

---

## 🛠️ Technical Details

### Design System (`style.css`)
The entire site shares a single, unified design system built with **CSS Custom Properties (variables)**:

```css
/* Example from style.css */
:root {
  --primary:        #2E7D32;   /* Forest green */
  --secondary:      #FF9800;   /* Warm amber */
  --radius-lg:      12px;
  --shadow-md:      0 4px 12px rgba(0,0,0,0.1);
}
```

This ensures visual consistency across all 20+ pages with minimal repetition.

### Layout
- **CSS Grid** and **Flexbox** are used throughout for responsive, multi-column layouts.
- Breakpoints cover **mobile** (≤ 480px), **tablet** (≤ 768px), and **desktop** (> 768px).

### JavaScript Interactivity
All JavaScript is vanilla (no frameworks or libraries). Key interactive features include:

| Feature | Technique |
|---|---|
| AIS impact scoring | DOM manipulation + conditional class toggling |
| Gallery modal customisation | Live CSS property updates via `element.style` |
| Feedback form validation | `addEventListener` + regex validation patterns |
| Mobile hamburger menu | `classList.toggle` on nav element |
| Hero animations | CSS `@keyframes` with JS class triggers |

### Images
All photography is sourced from **[Unsplash](https://unsplash.com)** (royalty-free), loaded via CDN URL references. No local image assets are required.

### Accessibility
- Semantic HTML5 elements (`<header>`, `<main>`, `<nav>`, `<section>`, `<footer>`)
- `aria-label` attributes on all interactive controls
- Keyboard navigation supported throughout
- Colour contrast ratios compliant with WCAG 2.1 AA standards

---

## 🚀 Getting Started

ClimAct requires **no installation, build tool, or server**. It runs entirely in the browser.

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/Thilac01/Climate_Act.git
   ```

2. **Navigate to the folder**
   ```bash
   cd Climate_Act
   ```

3. **Open the entry point**

   Simply open `splash.html` in any modern browser:
   ```bash
   # macOS
   open splash.html

   # Windows
   start splash.html

   # Linux
   xdg-open splash.html
   ```

   Or open it directly via **File → Open** in your browser.

### Browser Compatibility

| Browser | Supported |
|---|---|
| Chrome 90+ | ✅ |
| Firefox 88+ | ✅ |
| Safari 14+ | ✅ |
| Edge 90+ | ✅ |

> **Note:** An internet connection is recommended for loading Unsplash images. The site's layout and functionality work fully offline; only remote images will not display.

---

## 👥 Team

The ClimAct website was built collaboratively by four students at the **University of Westminster** as part of a web development module focused on the UN SDGs.

| Student | Name | Pages Owned | Editor Report | Validation |
|---|---|---|---|---|
| Student 1 | Alex Johnson | `home.html`, `content_ST1.html` | `pageEditor_ST1.html` | `validation_ST1.html` |
| Student 2 | Maria Garcia | `content_ST2.html` | `pageEditor_ST2.html` | `validation_ST2.html` |
| Student 3 | James Chen | `content_ST3.html` | `pageEditor_ST3.html` | `validation_ST3.html` |
| Student 4 | Sarah Williams | `content_ST4.html` | `pageEditor_ST4.html` | `validation_ST4.html` |

Each team member maintained a **Page Editor** (`pageEditor_STn.html`) documenting their design decisions and a **Validation Report** (`validation_STn.html`) confirming HTML/CSS compliance.

---

## ✅ Validation & Accessibility

All pages in this project have been validated using the **W3C Markup Validation Service** and **W3C CSS Validator**. Results are documented in the individual `validation_STn.html` reports.

- **HTML:** Valid HTML5, no critical errors
- **CSS:** Valid CSS3 with vendor prefixes where required
- **Accessibility:** Tested against WCAG 2.1 Level AA guidelines

---

## 📜 License

This project was created for **educational purposes** at the University of Westminster. Content is original and images are sourced from Unsplash under the [Unsplash License](https://unsplash.com/license).

```
© 2026 ClimAct | SDG 13: Climate Action | University of Westminster
```

---

<div align="center">

🌿 *"The greatest threat to our planet is the belief that someone else will save it."* — Robert Swan

**[⬆ Back to Top](#-climact--sdg-13-climate-action)**

</div>
