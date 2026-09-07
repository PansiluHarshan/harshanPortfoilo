# Deploying this portfolio to GitHub Pages

## File structure (already set up)
```
your-repo/
├── index.html
└── assets/
    └── profile-photo.jpg   ← your photo, already in place
```

## Push to GitHub
1. Create a new repository at github.com (public, no README needed — you already have this file)
2. In the repo, click **Add file → Upload files**
3. Drag in `index.html` and the `assets` folder (with `profile-photo.jpg` inside)
4. Commit the changes

## Enable GitHub Pages
1. Repo → **Settings** → **Pages**
2. Source: `Deploy from a branch`
3. Branch: `main`, folder: `/ (root)`
4. Save — live in a minute or two at `https://<your-username>.github.io/<your-repo>/`

## Before going fully live
- Update the GitHub link in the footer (currently a placeholder `#`)
- Check the photo crop at different screen widths — if it looks off, adjust
  `object-position` in the `.hero-photo-panel img` CSS rule inside `index.html`

No build step, no dependencies — `index.html` is the entire site.
