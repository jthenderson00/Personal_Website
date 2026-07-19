# Jay Henderson — Personal Website

A dependency-free static portfolio for Jay Henderson, focused on IT support, infrastructure, systems administration, and automation work.

## Live site

The site is published with GitHub Pages from the repository's default branch:

`https://jthenderson00.github.io/Personal_Website/`

## Files

- `index.html` — complete responsive portfolio, styles, and minimal navigation JavaScript
- `favicon.svg` — scalable JH favicon
- `favicon.ico` — legacy browser fallback already present in the repository

## Design goals

- Recruiter-friendly overview with a clear contact path
- Current, defensible project descriptions instead of unsupported metrics
- Responsive layout with keyboard-accessible navigation
- No build system or package dependencies
- Relative asset paths so GitHub Pages project-site hosting works correctly
- No external JavaScript or CSS dependencies

## Deployment

GitHub Pages serves the repository as a project site under `/Personal_Website/`. Asset references must remain relative, for example:

```html
<link rel="icon" href="./favicon.svg">
```

Avoid root-relative paths such as `/favicon.svg`, which point to the root of `jthenderson00.github.io` instead of this project directory.

## Local preview

From the repository directory:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000/`.
