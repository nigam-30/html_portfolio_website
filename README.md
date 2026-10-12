# Personal Portfolio Website — HTML5 & CSS3 Conversion

**Student Name:** Nigam Mehta  
**Discipline:** Electronics Engineering (VLSI Design & Technology)  
**Institution:** Shah & Anchor Kutchhi Engineering College (SAKEC), Mumbai  
**Project Track:** EWB Courses | HTML & CSS Internship Project  
**Submission Deadline:** 16 October 2026  

---

## 1. Project Description (Internship Form Submission)

> A pixel-accurate, submission-ready personal portfolio website engineered exclusively using semantic HTML5 and modern CSS3 with zero JavaScript dependencies. The website showcases digital hardware, VLSI microarchitecture, FPGA prototyping, and systems engineering projects through a high-precision semiconductor aesthetic featuring a wafer-substrate micro-grid, chip-bezel cards, and responsive editorial typography. Built with fluid CSS Flexbox and Grid architectures, it delivers complete cross-device responsiveness across mobile, tablet, and desktop viewports with smooth navigation anchors, accessible interactive disclosures, and custom CSS-only light/dark theme support.

---

## 2. How to Open the Website Locally

You can open and test the website using any modern web browser (Google Chrome, Microsoft Edge, Mozilla Firefox, Safari) without needing any build tools, package managers, or server installations:

### Option A: Direct File Launch (Simplest)
1. Navigate to the `Nigam_HTML_CSS_Portfolio` folder.
2. Double-click `index.html` (or right-click and choose **Open with > Google Chrome** / **Microsoft Edge**).
3. The portfolio will load with all styles, fonts, images, and anchors immediately active.

### Option B: Local Static Server (Recommended for local PDFs and media)
If you prefer running a lightweight local HTTP server:
- **Using Python 3:**
  ```bash
  cd Nigam_HTML_CSS_Portfolio
  python -m http.server 3000
  ```
  Then visit [http://localhost:3000](http://localhost:3000) in your browser.
- **Using VS Code Live Server:**
  Open the folder in Visual Studio Code, right-click `index.html`, and select **Open with Live Server**.

---

## 3. Project Directory Structure

```
Nigam_HTML_CSS_Portfolio/
├── index.html                   # Semantic HTML5 document (zero JavaScript)
├── style.css                    # Modern CSS3 stylesheet with design tokens & media queries
├── Resume.pdf                   # Static downloadable engineering resume
├── resume.pdf                   # Case-insensitive compatibility symlink/copy
├── images/                      # Optimized image assets
│   ├── profile.jpg              # High-resolution profile photo
│   ├── certificates/            # Verified credentials & simulation certificates
│   └── projects/                # RTL schematics, Vivado waveforms & reports
├── reports/                     # Project technical reports & documentation
│   ├── Digital_data_monitor_Phase_1_report.pdf
│   ├── Digital_data_monitor_Phase_2_Report.pdf
│   ├── Pipelined_Processor_Project_Report.pdf
│   ├── Entropyx_Project_Report.pdf
│   ├── Credence-Core_Project_Report.pdf
│   ├── Rail_Nova_Project_Report.pdf
│   └── Telecom_Churn_Analysis_Report.pdf
└── README.md                    # Project documentation & compliance checklist
```

---

## 4. Internship Guideline Compliance Checklist

All requirements from `HTML_CSS_Internship_Project_Guide.pdf` are satisfied:

| Requirement | PDF Specification | Implementation Status | Notes |
|:---|:---|:---:|:---|
| **Technologies** | HTML5 and CSS3 only | ✅ Passed | 100% pure HTML & CSS. Zero JS, React, Tailwind, Bootstrap, or backend code. |
| **HTML5 Structure** | Valid doctype, html, head, body | ✅ Passed | Valid HTML5 with `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`. |
| **Meta & Viewport** | UTF-8 charset & viewport tag | ✅ Passed | `<meta charset="UTF-8">`, `<meta name="viewport" content="width=device-width, initial-scale=1.0">`. |
| **Header / Nav** | Name/logo & links to all sections | ✅ Passed | Sticky header with NM logo, links to `#about`, `#work`, `#skills`, `#experience`, `#contact`. |
| **Hero / Home** | Name, role, intro & CTA button | ✅ Passed | Dominant heading, value statement, tech pillars, "View Projects" and "GitHub" buttons. |
| **About Me** | Biography, education, career focus | ✅ Passed | Editorial narrative, SAKEC B.Tech education banner, and Core Focus hardware matrix. |
| **Skills Section** | ≥ 5 skills as labels, chips, or cards | ✅ Passed | 20 categorized skills across Hardware, EDA & Workflows, Software & Compute. |
| **Projects Section**| ≥ 2 project cards with title, description, tech stack | ✅ Passed | 6 projects including featured FPGA hardware IP (DEMU) and 5 full-stack/systems projects. |
| **Contact Section** | Email & profile links | ✅ Passed | Direct email, mailto CTA, LinkedIn, GitHub, Resume download, and engineering telemetry. |
| **Footer** | Copyright line & student name | ✅ Passed | `© 2026 Nigam Mehta · Built with HTML5 & CSS3`, brand mark, and back-to-top anchor. |
| **Separate CSS** | `style.css` linked from HTML | ✅ Passed | External stylesheet `style.css` linked in `<head>`. |
| **CSS Variables** | Color tokens & design system | ✅ Passed | Custom properties for background, cards, text, accents, borders, and shadows. |
| **Flexbox & Grid** | Modern CSS layout engines | ✅ Passed | Grid used for projects, skills, and about sections; Flexbox for header, hero, and cards. |
| **Responsive Design** | Usable on mobile (360/390px), tablet (768px), desktop (1440/1920px) | ✅ Passed | Fully tested across all viewports; zero horizontal overflow. |
| **Hover & Focus** | Hover and focus states on links/buttons | ✅ Passed | Interactive hover transitions, focus outlines, and card elevation effects. |

---

## 5. Original Interactive Features & CSS-Only Adaptations

To strictly adhere to the internship constraint requiring **zero JavaScript**, the following dynamic behaviors were faithfully recreated using clean, accessible HTML5 and CSS3 mechanisms:

1. **Mobile Navigation Drawer:**
   - *Original:* React `useState(isOpen)` + Framer Motion animated drawer.
   - *HTML/CSS Adaptation:* Built using a pure CSS hidden checkbox toggle (`#mobile-menu-toggle`) with accessible SVG hamburger / close triggers and responsive drawer display.
2. **Light / Dark Mode Switcher:**
   - *Original:* Next.js React Context (`ThemeContext`) with `localStorage`.
   - *HTML/CSS Adaptation:* Powered by a CSS checkbox toggle (`#theme-toggle`) leveraging `:root:has(#theme-toggle:checked)` to dynamically switch CSS custom variables between light (#F7F8FA) and dark (#07090D) themes.
3. **Experience & Certifications Disclosure Accordions:**
   - *Original:* React state button toggling array slices (`showAll ? items : items.slice(0, 4)`).
   - *HTML/CSS Adaptation:* Implemented with native HTML5 `<details>` and `<summary>` elements styled with CSS to render the exact `+ 5 Earlier Internships` and `+ 11 More Certifications` buttons.
4. **Certificate Image Preview Lightbox:**
   - *Original:* Framer Motion modal dialog with backdrop blur.
   - *HTML/CSS Adaptation:* Recreated using pure CSS `:target` pseudo-class modals (`#cert-modal-1` through `#cert-modal-8`). Clicking "Preview" opens the modal; clicking the backdrop or close button returns to `#certifications`.
5. **Direct Contact & Telemetry:**
   - *Original:* React state form with custom copy button and telemetry card.
   - *HTML/CSS Adaptation:* Streamlined direct email channel (`mailto:mehtanigam3024@gmail.com`), social action buttons (GitHub, LinkedIn, Resume download), and engineering telemetry metadata.

---

## 6. Summary of Visual Fidelity & Differences

- **Layout & Section Order:** 100% identical to the original live website (Header → Hero → About → Selected Work → Skills → Experience Timeline → Certifications → Open Source Repositories → Contact → Footer).
- **Typography & Font Hierarchy:** Identical pairing of Google Fonts *Inter* for editorial copy and *JetBrains Mono* for engineering identifiers, technical specs, and dates.
- **Color Palette & Visual Details:** Exact hexadecimal matches for substrate background (`#F7F8FA`), wafer grid lines, hairline borders (`rgba(0, 0, 0, 0.08)`), cyan accent (`#007EA7`), emerald status indicator (`#10b981`), and dark button styles.
- **Silicon Reticle Markers:** Recreated purely in CSS with hairline border corner reticles on the profile frame.
- **Hardware Spec Metrics:** Featured project card displays identical 4-column metric boxes for Clock, Timing Slack, Core Logic, and Bus Interconnect.
- **Visual Differences:** None. The visual reconstruction is indistinguishable from the live website at matching viewport widths.
