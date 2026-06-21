# AR Studio APP

Clean upload-ready static package generated from the Google Stitch export `stitch_b_socio_ar_studio.zip`.

## What is included

- Root `index.html`: production landing page from `b_socio_ar_studio_production_landing_page/code.html`.
- `screens.html`: visual index for all 83 exported HTML screens.
- Original exported screen folders with `code.html` and `screen.png` preserved.
- Original Stitch markdown guides preserved.
- Static hosting files for Netlify, Vercel, and GitHub Pages.

## Upload

### Netlify drag-and-drop
Upload this whole folder. No build command is required.

### Vercel
Import this folder/repository as a static project. No install or build command is required.

### GitHub
Push the complete folder contents. Do not add `node_modules`, `.next`, `.env*`, or logs.

## Local preview

Open `index.html` in a browser for the production landing page, or open `screens.html` to browse all exported screens.

## Notes

The exported pages rely on public CDN resources such as Tailwind, Google Fonts, Material Symbols, and Stitch-generated image URLs, so a live internet connection is needed for the exact visual result.
