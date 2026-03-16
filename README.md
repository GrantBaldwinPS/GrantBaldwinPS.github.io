# E. Grant Baldwin — Personal Academic Website

Built with [Quarto](https://quarto.org/).

## Structure

```
.
├── _quarto.yml       # Site config: navbar, theme, footer
├── custom.scss       # All custom styling
├── index.qmd         # Bio & CV page (home)
├── research.qmd      # Publications & working papers
├── teaching.qmd      # Teaching history
├── 404.qmd           # 404 page
└── files/
    ├── cv.pdf        # Your CV PDF (already included)
    └── img/
        └── headshot.jpg   # ← ADD YOUR PHOTO HERE
```

## Setup

1. **Install Quarto**: https://quarto.org/docs/get-started/
2. **Add your headshot**: Replace `files/img/headshot.jpg` with your photo
3. **Preview locally**:
   ```r
   # In R, from the project directory:
   quarto::quarto_preview()
   ```
   Or from terminal:
   ```bash
   quarto preview
   ```
4. **Render the site**:
   ```r
   quarto::quarto_render()
   ```

## Deploying

### Quarto Pub (easiest, free)
```bash
quarto publish quarto-pub
```

### Netlify (recommended for custom domain)
```bash
quarto publish netlify
```

### GitHub Pages
```bash
quarto publish gh-pages
```

## Customizing

- **Colors/fonts**: Edit `custom.scss` — the top `/*-- scss:defaults --*/` section has all the key variables
- **Navbar links**: Edit `_quarto.yml` under `website.navbar`
- **Add a blog**: Create a `blog/` directory with `posts/` subdirectory, add `listing` to a new `blog.qmd`
- **Add social icons**: Update the navbar `right` section in `_quarto.yml`

## Color Palette

| Variable | Value | Use |
|---|---|---|
| Navbar bg | `#1a1a2e` | Deep navy |
| Gold accent | `#e8c97a` | Active links, section borders |
| Link color | `#8b1a1a` | Body links |

