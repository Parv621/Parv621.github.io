# Personal website template

A single-page personal/academic site, adapted from [sushrutkr.github.io](https://sushrutkr.github.io/).
Plain HTML/CSS/JS, no build step, dark/light theme toggle built in.

## What's here

- `index.html` — the entire site (structure, styles, and script are all in this one file)
- `images/photo.jpg` — a placeholder headshot; swap it for your own (keep the filename or update the `<img>` `src` in `index.html`)

Every section that needs your information is marked with `[bracketed placeholder text]` and,
in most places, an HTML comment starting `<!-- TO CUSTOMIZE: ... -->` explaining what to do.
Search the file for `[` to find every spot that still needs editing.

## Sections to fill in

1. **`<title>`** and Google Analytics block (top of `<head>`) — your name/tagline, and your own GA ID if you use one (otherwise leave it commented out)
2. **Hero** — name, photo, one-line bio, current role, GitHub/Scholar/email links
3. **About** — five bio paragraphs and five headline stat tiles
4. **Experience** — one timeline entry per role (copy/paste the block to add more)
5. **Technical Stack** — four skill categories, rename and fill as fits your field
6. **Open Source** — up to three project cards linking to your repos
7. **Research Highlights** — up to three larger write-ups, each with an image/video placeholder
8. **Selected Publications** — one row per paper, plus a link to your Google Scholar profile
9. **Contact / footer** — your name, affiliation, and email (the email is split into `u`/`d` variables near the bottom of the script to keep it off scrapers)

## Deploying to GitHub Pages

1. On GitHub, create a new **empty** repository (no README/gitignore/license) named
   `yourusername.github.io` if you want it at the root of your GitHub Pages domain,
   or any name if you're fine with `yourusername.github.io/reponame`.
2. Push this folder to that repository (see the steps your assistant gave you, or run
   the commands below from a computer with git installed):

   ```bash
   git remote add origin https://github.com/yourusername/yourusername.github.io.git
   git branch -M main
   git push -u origin main
   ```

3. In the repo's **Settings → Pages**, set the source to the `main` branch, root folder.
4. Your site will be live at `https://yourusername.github.io/` (or
   `https://yourusername.github.io/reponame/`) within a minute or two.

## Local preview

No build step needed — open `index.html` directly in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

then visit `http://localhost:8000`.
