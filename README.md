<p align="center">
	<img src="./Images/logo.png" alt="Photography Website logo" width="92" height="92" />
</p>

<h1 align="center">Photography Website</h1>

<p align="center"><i>Static photography landing page built with HTML and CSS, featuring a full-screen background image and a CSS-only sliding sidebar menu.</i></p>

<p align="center">
	<img src="https://img.shields.io/badge/TYPE-STATIC%20SITE-8B5CF6?style=for-the-badge&labelColor=4C1D95" alt="Static site" />
	<img src="https://img.shields.io/badge/HTML-5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
	<img src="https://img.shields.io/badge/CSS-3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
	<img src="https://img.shields.io/badge/STYLE-SIDEBAR%20UI-14B8A6?style=for-the-badge&labelColor=0F766E" alt="Sidebar UI" />
	<img src="https://img.shields.io/badge/FEATURE-FULLSCREEN%20HERO-DB2777?style=for-the-badge&labelColor=BE185D" alt="Fullscreen hero" />
	<img src="https://img.shields.io/badge/DEPLOYMENT-STATIC%20HOSTING-22C55E?style=for-the-badge&labelColor=15803D" alt="Static hosting" />
	<img src="https://img.shields.io/badge/ICONS-FONT%20AWESOME-F59E0B?style=for-the-badge&labelColor=92400E" alt="Font Awesome" />
	<img src="https://img.shields.io/badge/FONTS-GOOGLE%20POPPINS-3B82F6?style=for-the-badge&labelColor=1D4ED8" alt="Google Poppins" />
	<img src="https://img.shields.io/badge/💡-PORTFOLIO%20LANDING%20PAGE-111827?style=for-the-badge&labelColor=1F2937" alt="Portfolio landing page" />
</p>

## Table of Contents

- [🚀 Project intro](#project-intro)
- [📁 Project structure](#project-structure)
- [⭐ Differentiators](#differentiators)
- [🔧 Features](#features)
	- [Flow diagram](#flow-diagram)
	- [Interaction behavior](#interaction-behavior)
- [🧰 Tech stack](#tech-stack)
- [⚙️ Install methods](#install-methods)
- [🔐 Environment variables](#environment-variables)
- [📜 Available scripts](#available-scripts)
- [🚀 Deployment notes](#deployment-notes)
- [🤝 Contributing](#contributing)
- [📄 License](#license)

## 🚀 Project intro

This project is a simple static photography website built with HTML and CSS. It uses a full-screen background image, a left-side sliding menu, and icon-based navigation to create a focused landing-page experience without any JavaScript, backend, or database layer.

## 📁 Project structure

```txt
Photography-Website/
├── index.html
├── README.md
├── css/
│   └── style.css
└── Images/
    ├── logo.png
    └── photo.jpg
```

## ⭐ Differentiators

- CSS-only sidebar toggle driven by a hidden checkbox and label controls
- Full-screen photography hero background for an immediate visual focus
- Lightweight single-page layout with no build step or framework overhead
- Font Awesome icons and Google Fonts loaded from CDNs for simple presentation styling

## 🔧 Features

### Core features

| Feature | Status | Notes |
| --- | --- | --- |
| Full-screen landing page | ✅ Current | The main hero area fills the viewport with a photography background image. |
| Sliding sidebar menu | ✅ Current | A left-side menu opens and closes with smooth CSS transitions. |
| Navigation-style menu items | ✅ Current | Gallery, Shortcuts, Exhibits, Events, Store, Contact, and Feedback are shown as menu entries. |
| Social media icons | ✅ Current | Facebook, Twitter, Instagram, and YouTube icons appear in the sidebar footer area. |
| Responsive viewport setup | ✅ Current | The page includes the standard mobile viewport meta tag. |

### 🌊 Flow diagram

The Mermaid flow below shows the main interaction path for the page, from loading the landing screen through opening the sidebar and selecting menu actions.

```mermaid
flowchart TD
	A[Visitor] --> B[/Open index.html/]
	B --> C[See full-screen photography hero]
	C --> D{Open sidebar?}

	D -- Yes --> E[Click hamburger icon]
	E --> F[Sidebar slides in]
	F --> G[View menu items and social icons]
	G --> H{Close sidebar?}
	H -- Yes --> I[Click close icon]
	I --> C

	D -- No --> J[Continue viewing the hero page]
```

### Interaction behavior

- The hamburger icon opens the sidebar by toggling a hidden checkbox.
- The close icon hides the sidebar with the same CSS toggle behavior.
- The menu items are present as placeholder links (`#`) inside a single-page layout.
- The social icons are displayed in the sidebar footer area for visual polish.

## 🧰 Tech stack

- **Markup:** HTML5
- **Styling:** CSS3
- **Icons:** Font Awesome 6.4
- **Typography:** Google Fonts (Poppins)
- **Runtime:** Browser-only static page

## ⚙️ Install methods

### 📦 Open locally

Prerequisites:

- A modern web browser

1. Clone or download this repository.
2. Open the project folder.
3. Open `index.html` directly in your browser to view the site.

If you prefer a local server, you can also serve the folder with any static file server or a VS Code Live Server extension.

## 🔐 Environment variables

No environment variables are required for this project.

Notes:

- All layout and behavior are handled in `index.html` and `css/style.css`.
- Font Awesome and Google Fonts are loaded from external CDNs, so the page needs internet access for those assets.

## 📜 Available scripts

This repository does not define any npm, yarn, or build scripts.

Useful manual actions:

- Open `index.html` directly for a quick preview.
- Use any static server if you want a local hosted experience during editing.

## 🚀 Deployment notes

- This project can be deployed as static files on any host that serves HTML, CSS, and image assets.
- Make sure the `css/` and `Images/` folders are included in the deployment output.
- GitHub Pages, Netlify, Vercel static hosting, or standard web servers can all serve this project as-is.

## 🤝 Contributing

- Fork the repository and create a feature branch.
- Keep pull requests focused and include verification steps.
- Avoid committing secrets or unnecessary generated files.

## 📄 License

No license file is currently included in this repository.
