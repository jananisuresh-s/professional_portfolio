# Janani S — Portfolio

A dark-themed, single-page portfolio built with plain HTML, CSS, and JavaScript (no frameworks, no build step). Includes dedicated detail pages for each project.

## Files

```
index.html                        Main page (About, Skills, Projects, Education, Contact)
project-brain-tumor.html          Brain Tumor Detection — project detail page
project-smart-rooftop.html        Smart Rooftop System — project detail page
project-line-following-robot.html Line-Following Robot — project detail page
style.css                         All styling (colors, layout, animations)
script.js                         Scroll animations (skill bars + section reveals)
Janani_S_Resume.pdf               Resume, linked from the nav bar and footer
README.md                         This file
```

All files must stay in the same folder — the pages link to each other and to the stylesheet/script using relative paths (e.g. `href="style.css"`, `href="project-brain-tumor.html"`). If you move one file without the others, those links break.

## Viewing it locally

Just open `index.html` in a browser. Everything runs client-side, no server or build step needed.

## Publishing to GitHub Pages

1. **If you're replacing your existing portfolio repo** (`jananisuresh-s.github.io/portfolio-website` or similar):
   - Delete the old files from the repo (or clear the folder locally before copying these in), so nothing conflicts.
   - Copy all 7 files from this zip into the repo folder.
   - Commit and push:
     ```
     git add .
     git commit -m "Redesign portfolio"
     git push
     ```
   - GitHub Pages will rebuild automatically — give it a minute or two, then check your existing Pages URL.

2. **If you're starting a fresh repo:**
   - Create a new repo on GitHub. If you want it at `https://jananisuresh-s.github.io`, the repo must be named exactly `jananisuresh-s.github.io`. Otherwise, name it anything and it'll be served at `https://jananisuresh-s.github.io/<repo-name>`.
   - Upload all 7 files (GitHub's web UI "Add file → Upload files" works fine for this, or `git add . && git commit -m "Initial portfolio" && git push`).
   - Go to the repo's **Settings → Pages**, set the source branch to `main` (or `master`) and folder to `/root`, then save.
   - Your site will be live at the URL GitHub shows on that same settings page within a few minutes.

## Before you publish — double check

- Resume PDF is current (swap `Janani_S_Resume.pdf` for an updated version if needed, keeping the same filename, or update the filename in `index.html`'s two resume links if you rename it).
- Smart Rooftop System project page has a placeholder line under "My role" — fill in your actual contribution before this goes live.
- All contact links (email, GitHub, LinkedIn) are already wired to your real accounts.

## Customizing

- Colors live as CSS variables at the top of `style.css` (`:root { --bg, --primary, --accent, ... }`) — change them there and they apply everywhere.
- Skill bar percentages are inline `style="--fill:XX%"` on each `.skill-bar-fill` div in `index.html` — adjust freely as your skills grow.

## Live Demo

https://jananisuresh-s.github.io/professional_portfolio/
