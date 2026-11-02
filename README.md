# Personal Website — Santiago M. Pinto (`www.santiagompinto.com`)

This folder (`C:\Users\E1SMP01\Dropbox\Personal\My Personal Website`) is the live source repository for **https://www.santiagompinto.com**, hosted on GitHub Pages via [`smpinto/smpinto.github.io`](https://github.com/smpinto/smpinto.github.io).

---

## Quick Guide: How to Update Your Website

Because this folder is directly connected to your GitHub repository (`origin/main`), you no longer need to manually drag-and-drop files onto GitHub's website.

### Option 1: Using Your AI Assistant (Antigravity, Claude Code, or Codex) — Recommended
1. Open `C:\Users\E1SMP01\Dropbox\Personal\My Personal Website` in the IDE.
2. Tell the assistant what you want to update, for example:
   - *"Check my Richmond Fed profile (`https://www.richmondfed.org/research/people/pinto`) and Google Scholar (`https://scholar.google.com/citations?view_op=list_works&hl=en&user=TOT0F80AAAAJ&sortby=pubdate`) for any new publications and add them to `research.html`."*
   - *"I placed an updated `CV_SMP.pdf` in the folder — commit and push it to my website."*
   - *"Update the bio text on `index.html` and push the changes."*
3. The assistant will edit the files locally, commit, and run `git push origin main`.
4. Wait **1–2 minutes** for GitHub Pages to rebuild, then open `https://www.santiagompinto.com` and press **`Ctrl + F5`** to refresh.

### Option 2: Editing Files Yourself
1. Edit the HTML/CSS files directly in this folder (`index.html`, `research.html`, `cv.html`, `other-stuff.html`, `style.css`) or replace `CV_SMP.pdf`.
2. Double-click any `.html` file in File Explorer to preview your changes locally in your browser.
3. Ask the assistant to *"commit and push my website changes"*, or run in the terminal:
   ```powershell
   git pull --autostash origin main
   git add index.html research.html cv.html other-stuff.html style.css main.js CV_SMP.pdf
   git commit -m "Update website content"
   git push origin main
   ```

> **Tip:** Prefer making edits in this local folder rather than using the pencil icon on `github.com`. If you ever make a quick edit on `github.com`, run `git pull` (or tell the assistant) at the start of your next session so your local files stay in sync.

---

## Site Structure

| File / Folder | Purpose |
| :--- | :--- |
| `index.html` | Home page (bio, photo, contact details) |
| `research.html` | Publications, working papers, books/chapters, presentations & podcasts, ongoing research (organized as collapsible dropdown categories with expandable abstracts) |
| `cv.html` | Curriculum Vitae page |
| `CV_SMP.pdf` | Downloadable Curriculum Vitae PDF |
| `other-stuff.html` | Additional links and resources |
| `style.css` | Site-wide styling and layout |
| `main.js` | Mobile navigation menu and dynamic footer year |
| `public/` | Additional downloadable PDFs and static assets |
| `CNAME` | **Required by GitHub Pages** — binds custom domain `www.santiagompinto.com` (do not delete) |

---

## Reference: Domain & Hosting Setup (GoDaddy + GitHub Pages)

- **GitHub Repository:** `https://github.com/smpinto/smpinto.github.io` (branch: `main`, Public)
- **Custom Domain:** `www.santiagompinto.com` (stored in `CNAME`)
- **GoDaddy DNS Records:**
  - `A` records (`@`): `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
  - `CNAME` record (`www`): `smpinto.github.io`
