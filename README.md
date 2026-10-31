# LUMINAER Website Guide

## Live website

- Website: <https://luminaer.vercel.app>
- Source repository: <https://github.com/chaitanyasaiganeshmanda-oss/luminaer>
- Production branch: `main`
- Hosting: Vercel

## Website features

- Responsive LUMINAER landing page with a portable-kit illustration.
- Dark and light appearance toggle. On a first visit, the site follows the device preference; after a visitor chooses a theme, the choice is saved in that browser.
- Navigation links open separate page views for Concept, The Kit, Prototype, Checklist, Help, FAQ, and Feedback. Each view has its own shareable URL, for example <https://luminaer.vercel.app/?page=kit>.
- Interactive checklist progress is saved in the visitor's browser.
- Feedback form submits through FormSubmit to the recipient configured in the HTML. Email delivery may require FormSubmit activation.

## Project files

- `index.html` — active website. The page content, styles, and browser scripts are included here.
- `style.css` and `script.js` — older standalone source files; the active page does not load these files.
- `LUMINAER-website-source (1).zip` — archived source copy.
- `README.md` — this guide.

## Preview locally

This is a static HTML site and has no build step. From the repository folder, run:

```powershell
python -m http.server 8000
```

Then open <http://localhost:8000/>. Keep the terminal window open while previewing. Stop the server with `Ctrl+C`.

## Save or restore a backup

On GitHub, open the repository and choose **Code → Download ZIP**. To restore an earlier page, use the repository's commit history to recover `index.html` from the desired version.

## Publish updates

The Vercel project is connected to this repository. Changes committed to `main` trigger a production deployment. In Vercel, wait for the deployment to show **Ready**, then check <https://luminaer.vercel.app>. The site is configured as a plain static HTML project with the repository root as its deployment directory.

## External assets and services

- The prototype image is loaded from a Google Drive thumbnail. The image must remain publicly accessible or be replaced with a stable image URL.
- The feedback form relies on FormSubmit and the configured recipient address.
