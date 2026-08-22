# Valeria Guevara — Power Vinyasa Teacher

A single-page personal site: plain HTML/CSS/JS, no build step, no dependencies beyond Google Fonts.

## Structure

```
.
├── index.html    # all page content
├── styles.css    # design system + layout (pink/beige theme)
├── script.js     # reserved for future interactivity
└── README.md
```

## Run it locally

Open `index.html` directly in a browser, or serve it:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy to GitHub Pages

1. Push these files to a new repo's `main` branch:
   ```bash
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
2. On GitHub: **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`.
4. Save — the site goes live at `https://<your-username>.github.io/<repo-name>/`.

## Customizing

- **Name, bio, class/workshop copy** — edit directly in `index.html`, it's plain markup.
- **Colors** — all tokens live at the top of `styles.css` in `:root` (`--sand`, `--rose`, `--wine`, etc.).
- **Prices / session lengths** — in the `#privates` section of `index.html`.
- **Booking** — "Inquire about privates" and the header CTA are `mailto:` links; swap for a real scheduling tool (Calendly, Acuity, etc.) when ready.
- **Photo** — the pink "VG" circle in `#about` is a placeholder monogram. Replace `.monogram` in the HTML with an `<img>` tag once you have a headshot, and adjust `.monogram` CSS to `object-fit: cover`.
