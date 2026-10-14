# Anam Husain Portfolio

Static site. One `index.html` with its images and CV alongside it. No build step. Hosted on Cloudflare (Workers), deployed from this GitHub repo.

## Deploy to Cloudflare Pages via GitHub

1. Create a new GitHub repo (e.g. `anam-portfolio`) and push this folder to it.
2. In Cloudflare, go to Workers & Pages > Create > Pages > Connect to Git, and pick the repo.
3. Build settings: Framework preset `None`, build command empty, output directory `/`.
4. Deploy. The site goes live at `<project>.pages.dev`.
5. Optional: add a custom domain under the project's Custom domains tab.

## Editing content

- Client strip: the `CLIENTS` list at the top of the `<script>` block.
- Case studies: the cards are plain HTML inside `<div class="grid" id="grid">`. Each card's gallery images are listed in `CASES` in the script, in the same order as the cards.
- FAQs: plain HTML inside `<div id="qas">`. Copy a `.qa` block to add one.
- Stats: edit both `data-n` and the visible number in each `.odo` (e.g. `data-n="25"` and `25`).
- Bio, experience rows and skills are plain HTML in their sections.

## Before sharing widely

- Share preview: once the final domain is live, change `og:image` in the `<head>` to the full URL (`https://<domain>/og-image.jpg`) and add `og:url` and a canonical link.
- Call button: swap the `mailto:` for a Cal.com or Calendly link once she has one.

## Swapping images

- Hero: `anam-portrait.webp`
- Link preview (WhatsApp, LinkedIn): `og-image.jpg`, 1200x630
- About portrait: `backcourt-chairs.webp` (swap for a photo of Anam)
- Call card avatar: `anam-portrait.webp` (cropped to her face)
- CV download: `Anam_Husain_CV.pdf`
