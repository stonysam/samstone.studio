# samstone.studio

Website and brand files for Sam Stone Studio.

| Folder | What's in it |
|---|---|
| `site/` | The website, as deployed at https://samstone.studio. Plain HTML, CSS and self-hosted fonts; no build step. |
| `brand/` | The design system: brand book (`README.md`), tokens (`tokens.json`, `tokens.css`), logos and fonts. The live version, with component previews, is the "Sam Stone Studio design system" artifact in Claude. |

## Updating the website

1. Edit the files in `site/`.
2. In Cloudflare, go to Workers & Pages → `small-water-1df4` → New deployment.
3. Upload the contents of `site/` (or a zip with `index.html` at its root).

The site is served from Cloudflare Workers (static assets only) at samstone.studio and www.samstone.studio.

## Fonts

Manrope and Newsreader, both under the SIL Open Font License 1.1. The licence files are next to the font files. The site loads its fonts from its own folder, not from Google Fonts.
