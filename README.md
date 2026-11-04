# Wu Qiongyi — Personal Website

A single-page, dependency-free personal website (HTML + CSS + a little JS), ready for GitHub Pages.

## Preview locally

Open `index.html` in a browser, or run a tiny local server:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Deploy on GitHub Pages

1. Create a new repository on GitHub. For the address `https://<username>.github.io`, name it `<username>.github.io`. Any other name gives `https://<username>.github.io/<repo-name>/`.
2. Push this folder:

   ```bash
   git init
   git add .
   git commit -m "Personal website"
   git branch -M main
   git remote add origin https://github.com/<username>/<repo-name>.git
   git push -u origin main
   ```

3. On GitHub, go to **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, then select `main` and `/ (root)`, and click **Save**.
4. After a minute or two the site will be live at the address shown on that page.

## Editing

All content is in `index.html`. Each section is marked with a comment (`HERO`, `ABOUT`, `PROJECTS`, `EXPERIENCE`, `EDUCATION`, `SKILLS`, `CONTACT`). Colours are set as CSS variables at the top of the `<style>` block (`--accent` is the main teal).
