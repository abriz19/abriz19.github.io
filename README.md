# Abreham Dessu — Portfolio

Personal portfolio and CV for **Abreham Dessu**, Full Stack Software Engineer.

**Live site:** https://abriz19.github.io

Built with semantic HTML5 and hand-written CSS — no frameworks, no build step, no JavaScript.

## Files

| File | Purpose |
|------|---------|
| `index.html` | The portfolio site — hero, skills, experience timeline, projects, contact |
| `style.css` | All styling. Design tokens in `:root`, light + dark themes, responsive |
| `resume.md` | Master resume in Markdown — the readable source of truth |
| `resume.html` | Print-optimised A4 CV sheet; generates the PDF and doubles as a browser-viewable CV |
| `Abreham_Dessu_CV.pdf` | Downloadable CV, generated from `resume.html` |
| `og-image.png` | Social preview card (1200×630) for link sharing |

## Regenerating the CV PDF

After editing `resume.html`:

```bash
google-chrome --headless --disable-gpu --no-pdf-header-footer \
  --print-to-pdf=Abreham_Dessu_CV.pdf resume.html
```

Any Chromium-based browser works. Keep the output to two A4 pages.

## Local preview

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Notes

Resume content lives in three places — `resume.md`, `resume.html`, and the experience
timeline in `index.html`. Update all three when the content changes.
