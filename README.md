# Designed to Learn — Sinegugu Khumalo

A personal website built with plain HTML, CSS, and JS. No build step, no framework — every page is a standalone `.html` file that shares `style.css` and `script.js`.

## Pages
- `index.html` — home
- `about.html` — bio, background, skills
- `portfolio.html` — selected projects
- `blog.html` — blog index
- `blog-post-1.html`, `blog-post-2.html`, `blog-post-3.html` — starter posts (edit freely, add more the same way)
- `resume.html` — résumé, with a print/PDF button
- `contact.html` — contact details + a mailto-based contact form

## Host it on GitHub Pages (free)

1. Create a new **public** repository on GitHub — e.g. `personal-site`.
2. Upload all files in this folder to the repository root (drag-and-drop on github.com works, or use `git`):
```bash
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
```
3. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch `main`, folder `/ (root)`. Save.
4. GitHub will publish the site at `https://<your-username>.github.io/<repo-name>/` within a minute or two. That's your live link — no domain setup needed.

## Things to personalise before you share the link

- Replace the pink monogram badge (the `<svg>` in `index.html` and `about.html`) with a real photo — swap it for `<img src="photo.jpg" alt="Sinegugu Khumalo">` and drop `photo.jpg` in this folder.
- Swap the `#` placeholder LinkedIn URL (search-and-replace `sinegugu-khumalo` in the LinkedIn links) for your real profile link.
- The contact form submits via `mailto:`, which just opens the visitor's email client — fine for a start, but for real submissions, connect it to a free service like [Formspree](https://formspree.io) or [Netlify Forms](https://www.netlify.com/products/forms/) instead.
- Add more blog posts by duplicating `blog-post-3.html`, editing the content, and linking it from `blog.html`.

## Hiding a page from public view (for an examiner link)

GitHub Pages serves whatever's in the repo publicly — there's no built-in "private page" toggle. Two easy options:
- **Unlisted page:** create the page (e.g. `draft.html`) but don't link to it from any nav or other page. Anyone with the exact URL can view it; it won't appear in navigation or search. Share that direct link with your examiner, then link it into the nav later when it's ready to go public.
- **Private repo + GitHub Pages (paid tiers) or a password gate via a third-party static host** if you need real access control, not just an unlisted URL.
