# Khush Makhija Portfolio

This repository contains the static one-page CV/portfolio website for `khushmakhija.me`.

The site uses plain HTML, CSS, and a small amount of JavaScript. It can be deployed directly with GitHub Pages and does not require a build step.

## Project Structure

```text
.
├── index.html
├── style.css
├── assets/
├── CNAME
└── README.md
```

Add your CV PDF to the `assets/` folder. The current download link in `index.html` points to:

```text
assets/Khush_Makhija_CV.pdf
```

If your PDF has a different name, update the `href` in the Download CV button.

## Preview Locally With VS Code Live Server

1. Open this repository in VS Code.
2. Install the `Live Server` extension if it is not already installed.
3. Right-click `index.html`.
4. Select `Open with Live Server`.
5. Your browser will open a local preview, usually at `http://127.0.0.1:5500/`.

## Commit and Push Changes

After editing the website, run:

```bash
git status
git add index.html style.css README.md CNAME assets/
git commit -m "Update portfolio website"
git push
```

## Enable GitHub Pages

1. Open the repository on GitHub.
2. Go to `Settings`.
3. Open `Pages`.
4. Under `Build and deployment`, choose `Deploy from a branch`.
5. Select the `main` branch and the `/root` folder.
6. Save the settings.

GitHub Pages will publish the site after the first deployment finishes.

## Connect the Custom Domain

The `CNAME` file already contains:

```text
khushmakhija.me
```

In the GitHub Pages settings:

1. Enter `khushmakhija.me` as the custom domain.
2. Save the domain.
3. Enable `Enforce HTTPS` after GitHub verifies the domain.

At your domain provider, configure DNS records for GitHub Pages. For an apex domain such as `khushmakhija.me`, add GitHub Pages `A` records. You can also add a `www` subdomain with a `CNAME` record pointing to `khushmakhija.github.io`.

GitHub's current Pages DNS documentation is the best source for the exact DNS values if they change.
