# XR4HRI website

Website of the XR4HRI workshop series (Extended Reality for Human-Robot Interaction), formerly VAM-HRI (2018–2025).

Plain HTML and CSS, no build step. GitHub Pages serves the files as they are (`.nojekyll` disables Jekyll).

## Structure

```
index.html            Series overview: about, topics, all editions, contact
hri2027/index.html    Current edition (update once the proposal is accepted)
ismar2026/index.html  XR4HRI @ ISMAR 2026 (migrated from Google Sites)
assets/css/style.css  Shared styles (light and dark mode)
assets/fonts/         Archivo, self-hosted (SIL Open Font License, see OFL.txt)
assets/img/           Favicon and images
```

The fonts are self-hosted on purpose: embedding Google Fonts directly transfers visitors' IP addresses to Google, which is a GDPR issue for sites run from the EU.

## Deploy on GitHub Pages

1. Create a GitHub organization `xr4hri` (or use an existing one) and a repository named `xr4hri.github.io`.
2. Push the contents of this folder to the `main` branch.
3. In the repository settings under Pages, choose "Deploy from a branch", branch `main`, folder `/ (root)`.
4. The site is then available at https://xr4hri.github.io/.

## Adding a new edition

1. Copy the folder of the most recent edition, e.g. `hri2027/` to `hri2028/`.
2. Update the title, meta description, facts, and content.
3. Mark the page as current in its navigation (`aria-current="page"`) and add it to the navigation of the other pages.
4. Add a row to the editions table in `index.html` and update the "Next" block.

## Open TODOs

Search the files for `TODO`:
- Discord invite and mailing list link on the home page
- GitHub organization name in the footer link
- Exact day and time of the ISMAR 2026 workshop
- HRI 2027: replace the status note with the call for papers once accepted

## Archive

Pages of the VAM-HRI editions 2018–2025 stay at https://vam-hri.github.io/previous/ and are linked from the editions table. Consider adding a note on vam-hri.github.io that points to this site.
