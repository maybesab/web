# Sabrina May, portfolio site

Static site. No build step, no dependencies. Every page is plain HTML with
inline CSS and JS, so you can drop this straight onto GitHub Pages.

## What is in here

    index.html          Home: hero, case studies, case board, contact
    about.html          About
    Design.html         Tinker: web, design interventions, graphic, fabrication, doodles
    resume.html         Resume viewer (password gated)
    favicon.png
    cases/              One HTML file per case study
      case.css          Shared case-study stylesheet
      favicon.png
      img/              Case study images and video
      assets/           Downloadable PDFs
    img/
      board/            Case board logos
      golive/           Go Live FigJam process artifacts

## Deploying to GitHub Pages

From this folder:

    git init
    git add .
    git commit -m "Portfolio update"
    git branch -M main
    git remote add origin https://github.com/<your-username>/<your-repo>.git
    git push -u origin main

Then in the repository: Settings, Pages, Source = Deploy from a branch,
Branch = main, folder = / (root). Save.

If the repository already exists locally, replace the files and:

    git add -A
    git commit -m "Portfolio update"
    git push

## One thing to add yourself

resume.html looks for a file named `resume.pdf` next to it. That file is not
in this bundle. Drop your PDF in at the root as `resume.pdf` and the viewer
picks it up automatically. Without it the page shows a placeholder instead of
breaking.

## Notes

Case pages link out to three live builds that are hosted separately:

    Go Live Companion   https://maybesab.github.io/Go-Live-/
    MPEP Study Tool     https://jd1407-code.github.io/MPEP/
    ATLA element quiz   https://maybesab.github.io/ATLA/

Fonts load from Google Fonts, so the site needs a network connection to look
right. Everything else is local.
