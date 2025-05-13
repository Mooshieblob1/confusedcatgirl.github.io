# confusedblorb.org

This is my socials website!  
Available at **[confusedblorb.org](https://confusedblorb.org/)**

---

## 🧠 Overview

A cozy, responsive personal landing site built with **SvelteKit** and **Tailwind CSS**, featuring a hand-crafted retro-futurist aesthetic and a soft blurred-glass layout.

This site serves as a public homepage for Blorb (a.k.a. confusedcatgirl), showcasing projects, contact links, and a few 3D-printed hobby works.

---

## ✨ Features

- ✅ **Single-page layout with anchor links**
- ✅ **Translucent blurred navbar and section boxes**
- ✅ **SvelteKit layout system with slot-based routing**
- ✅ `/tos` is a full separate route with consistent layout and styling
- ✅ Shared footer with attribution moved to layout (`About` section)
- ✅ Local navigation highlighting and smooth experience
- ✅ Optimized for both desktop and mobile displays
- ✅ No JavaScript frameworks beyond Svelte — lightweight and clean!

---

## 📁 Structure

```
src/
├── routes/
│   ├── +page.svelte        # Main homepage content (sections)
│   ├── tos/
│   │   └── +page.svelte    # Terms of Service route
│   └── +layout.svelte      # Shared layout (banner, nav, footer)
├── app.css                 # Tailwind + custom styles
└── app.html                # HTML entry template
```

---

## 🛠 Tech Stack

- **SvelteKit** — App framework
- **Tailwind CSS** (built-in integration)
- **HTML/CSS** — Fully responsive design
- **Deployed at**: [confusedblorb.org](https://confusedblorb.org)

---

## 📸 Credits

- Banner: [mooshieblob.com](https://www.mooshieblob.com/)
- Footer art: [Yuuki Tatsuya, 2011](https://danbooru.donmai.us/posts/1029426)

---

## 📜 License

Personal project, not open for redistribution.
