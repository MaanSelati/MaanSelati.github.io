# Maan Selati — Resume Website

This folder is already a git repository with your site committed and ready to push.

## What's inside
- `index.html` — your resume site (light/minimal theme)
- `Maan-Selati-Resume.pdf` — your resume, linked from the site's "Download Resume" buttons
- `.git/` — a local git repo, already initialized with your name as the commit author, with your files already committed on the `main` branch

## What's left to do (only steps that need YOUR GitHub login)

1. Create a new **empty** repository on GitHub:
   - Go to https://github.com/new
   - Name it `<your-username>.github.io` (replace with your actual GitHub username) for the shortest possible URL, or any other name if a project subpage URL (`https://<username>.github.io/<repo-name>/`) is fine.
   - Leave "Add a README" and "Add .gitignore" **unchecked** — this folder already has everything.
   - Click Create repository.

2. Open a terminal **in this folder** (the one this README is in) and run:
   ```
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
   When prompted for a password, GitHub requires a Personal Access Token instead of your actual password:
   - Go to https://github.com/settings/tokens → "Generate new token (classic)" → check the `repo` scope → Generate, then paste that token as the password when git asks.
   - Or install [GitHub CLI](https://cli.github.com/) and run `gh auth login` once beforehand — after that, `git push` will just work with no token needed.

3. Turn on GitHub Pages:
   - In your new repo on GitHub, go to Settings → Pages.
   - Under "Build and deployment", set Source to "Deploy from a branch", branch `main`, folder `/ (root)`, then Save.
   - Wait a minute or two — your site goes live at:
     - `https://<your-username>.github.io/` (if the repo is named `<your-username>.github.io`)
     - `https://<your-username>.github.io/<repo-name>/` (otherwise)

## Making future edits
Edit `index.html` directly (it's plain HTML/CSS/JS, no build step), then from this folder:
```
git add .
git commit -m "update site"
git push
```
GitHub Pages redeploys automatically within about a minute of each push.
