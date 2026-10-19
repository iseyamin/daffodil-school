# 🏫 Daffodil School – Landing Page

A responsive, single-page landing website for a kids' school, built with **pure HTML5 + CSS3** (no frameworks, no JavaScript yet).

---

## 📑 Table of Contents

- [✨ Features](#-features)
- [🛠️ Tech Stack](#️-tech-stack)
- [📁 Project Structure](#-project-structure)
- [🧱 HTML Analysis](#-html-analysis)
- [🎨 CSS Analysis](#-css-analysis)
- [📱 Responsive Design](#-responsive-design)
- [⚠️ Issues Found & Fixes](#️-issues-found--fixes)
- [🚀 Future Improvements](#-future-improvements)
- [▶️ How to Run](#️-how-to-run)

---

## ✨ Features

- 🧭 Navigation bar with logo, links, hamburger button and a *Contact* button
- 🦸 Hero banner with colorful headline, subtitle and *Enroll Now* call-to-action
- 📚 "Standard Curriculum" section with 3 cards (Kinder, Elementary, Middle)
- ◀️▶️ Slider arrow buttons (UI only)
- 📰 "Our Stories" blog section (1 large story + 4 small cards)
- 🦶 Footer with school info, quick links and social icons
- 📱 Mobile layout via a media query at `576px`

---

## 🛠️ Tech Stack

| Technology | Usage |
|-----------|-------|
| 🟠 HTML5 | Semantic structure (`header`, `nav`, `main`, `section`, `footer`) |
| 🔵 CSS3 | Flexbox, Grid, media queries, gradients, shadows |
| 🔤 Google Fonts | **Quicksand** typeface |

---

## 📁 Project Structure

```
📦 daffodil-school
 ┣ 📜 index.html
 ┣ 📂 styles
 ┃ ┗ 📜 dis.css
 ┗ 📂 assets
   ┣ 🖼️ dis-new-1676290938.webp   (logo)
   ┣ 🖼️ hero-kids.png
   ┣ 🖼️ kinder.png / elementary.png / middle.png
   ┣ 🖼️ story-1.png … story-5.png
   ┣ 🖼️ bg.png
   ┗ 🖼️ logo.png, fb.png, google+.png, twitter.png, dribble.png
```

---

## 🧱 HTML Analysis

### 🔹 Page skeleton

```
<body>
 ├─ <header>
 │   ├─ <nav>      → logo, menu button, links, Contact button
 │   └─ .banner    → hero text + hero image
 ├─ <main>
 │   ├─ section.curriculumn   → 3 cards + slider arrows
 │   └─ section.stories-part  → story1 (big) + story2 (grid of 4)
 └─ <footer>       → info | about links | social icons
```

### 🔹 Section breakdown

| Section | Class | Purpose |
|---------|-------|---------|
| 🧭 Navbar | `.nav-bar` | Logo + links + CTA |
| 🦸 Banner | `.banner` | Headline, subtitle, *Enroll Now* |
| 📚 Curriculum | `.curriculumn`, `.c-cards`, `.c-card` | Program cards |
| ◀️▶️ Slider | `.slides`, `.slide` | Circular prev/next buttons |
| 📰 Stories | `.stories`, `.story1`, `.story2-card` | Blog previews |
| 🦶 Footer | `.last`, `.info`, `.about`, `.contact` | Info and links |

### 🔹 Good practices ✅

- ✅ Semantic tags (`header`, `nav`, `main`, `section`, `footer`)
- ✅ `lang="en"` and viewport meta tag set
- ✅ Meaningful `alt` on curriculum images
- ✅ Reusable utility classes (`display-flex`, `color-*`)
- ✅ Helpful Emmet comment left in the code

---

## 🎨 CSS Analysis

### 🎨 Color palette

| Variable-like class | Hex | Used for |
|---------------------|-----|----------|
| `.color-black` | `#111111` | Headings, dark button |
| `.color-yell` | `#FEA301` | Primary buttons, accents |
| `.color-sky` | `#01ACFD` | Links, footer background |
| `.color-sky2` | `#05D4DF` | Links, "Read more" |
| `.color-beg` | `#5D58EF` | Purple accent |

### 🔤 Typography

- Font: **Quicksand** (weights 300–700)
- Base weight set to `700` on `body` (everything is bold unless overridden)
- Sizes use `rem`: titles `3rem`, banner `3.5rem`, body text `1–1.25rem`

### 🧩 Layout techniques

| Technique | Where |
|-----------|-------|
| 📦 **Flexbox** | Navbar, banner, cards, footer, slider |
| 🔲 **CSS Grid** | `.story2` (2-column grid of small cards) |
| 🌈 **Gradients** | Stories background, card background |
| 🌑 **Box-shadow (inset)** | Curriculum cards |
| 🔘 **Rounded corners** | Buttons (`12px`, `48px`), cards (`16–19px`), slider (`50%`) |

### 🧰 Reusable classes

- `.display-flex` → `display: flex`
- `.btn-primary` / `.btn-sec` → button styles
- `.sec-title` → section headings
- `.color-*` → text colors

---

## 📱 Responsive Design

Breakpoint: `@media (max-width: 576px)`

| Element | Desktop 🖥️ | Mobile 📱 |
|---------|-----------|-----------|
| Nav links / Contact button | Visible | Hidden |
| Hamburger `☰` | Hidden | Visible |
| Banner | Row (text + image) | Column-reverse, centered |
| Curriculum cards | Row | Column |
| Slider arrows | Visible | Hidden |
| Big story (`.story1`) | Visible | Hidden |
| Small stories | 2-column grid | Smaller cards, centered |
| Footer | Row | Column |

---


## 🚀 Future Improvements

- 🔧 Add JavaScript for the mobile menu (`toggleMenu()`) and the curriculum slider
- 🎨 Introduce CSS variables (`:root`) for colors and spacing
- 📐 Add a tablet breakpoint (`~768px–992px`)
- ♿ Improve accessibility (alt text, ARIA labels, focus styles, color contrast)
- 🔍 Add SEO meta tags (`description`, Open Graph) and a descriptive `<title>`
- 🖼️ Add `loading="lazy"` to below-the-fold images
- 🧹 Rename classes consistently (BEM, e.g. `card__title`)
- 📬 Build a real Contact/Enroll form

---

## ▶️ How to Run

1. 📥 Clone or download the project
2. 📂 Make sure the `assets/` and `styles/` folders are in place
3. 🌐 Open `index.html` in any modern browser

```bash
# Optional: run a local server
npx serve .
```

---

## 👤 Author

Made with IS Eyamin for learning HTML & CSS.

## 📄 License

Free to use for learning purposes.
