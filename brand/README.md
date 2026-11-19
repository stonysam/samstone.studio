# Sam Stone Studio design system

The live version, with component previews, fonts and downloadable logos, is the "Sam Stone Studio design system" artifact: https://claude.ai/artifact/8pF4dEgCMNtDyAdCuU5jzA. This doc is a text copy for chats in this project. In this repo, the logos are in `logos/`, the fonts in `fonts/`, and `tokens.css` is generated from `tokens.json` for use in any page.

Sam Stone Studio is the trading name of Sam Stone, an independent product builder based in South Bohemia, Czech Republic. The studio turns founders' ideas into working products, built with AI. This system records the brand as it is used on samstone.studio and on Instagram (@samstone.studio): colours, type, logo, a few components and the voice.

## Using this system

- Use token names, never raw hex values, in new work. The colour tokens have a light and a dark theme; light is the default.
- Fonts are Manrope (display) and Newsreader (body). Serve them from your own files, as samstone.studio does, not from Google Fonts: loading them from Google sends visitors' IP addresses to Google.
- Use the logo files in Logos. Never retype the wordmark in another font or redraw the avatar.
- One page, one bold element. The site's is the "Decisions before code" panel in the hero.

## Voice

The studio is one person, and the writing says so.

- **First person singular.** "I", never "we". Hire Sam and you get Sam; when a project needs more people, he brings them in and says who they are.
- **Plain and specific.** Short sentences, everyday words. Name the problem, the outcome and the next step.
- **Honest about how the work is done.** "I direct AI coding tools; I don't hand-write every line." Present it as a strength, not a confession.
- **No hype.** No "cutting-edge", no "world's first", no emoji, no "I hope this finds you well".
- **Past tense for past roles.** Say what was led and delivered, not how another company is doing now.
- **Pricing on request.** Never print a price or an estimate.
- **Sentence case** for every heading, button and label. The only uppercase text is the eyebrow style.

| Write | Not |
|---|---|
| You have the vision. I'll build the product. | We deliver cutting-edge digital solutions. |
| I direct AI coding tools to do it, backed by eight years leading product at Swarm. | Our AI-powered team leverages deep expertise. |
| Tell me what you're trying to get done. | Get in touch to unlock your potential! |
| A few lines is enough to start. | Book a free discovery call today. |

## Colour

The palette is navy and blue on a pale blue-white ground, with one accent per view.

| Token | Role |
|---|---|
| `ground` | Page background |
| `surface` | Cards and tiles, always with a `line` border |
| `ink` | Text, and the background of inverted panels |
| `muted` | Secondary text |
| `accent` | Links, the primary button, highlighted headline text, numbers, "Studio" in the wordmark |
| `accent-soft` | Soft panels such as the stats band |
| `line` | Hairlines and borders |
| `brand-navy`, `brand-blue` | Fixed brand colours for the logo and Instagram |
| `on-navy`, `on-navy-accent`, `on-navy-soft` | Text on `brand-navy` |

Rules:

- **Borders, not shadows.** Sections and rows are separated by `line` hairlines; nothing casts a shadow.
- **Accent marks one thing.** The second sentence of a headline, a number, a link. Never a single word in the middle of a sentence.
- **Inverted panels use `ink`** as the background with `ground` text, so they flip to a light panel in the dark theme.
- **`brand-blue` is the logo's colour**: the avatar, the favicon and the occasional Instagram cover slide. Not for text.
- **Instagram uses the on-navy set** on `brand-navy`. The first posts used #a9d0f5 for the small samstone.studio label; new work uses `on-navy-soft`.

## Type

Heavy Manrope headings carry the studio's voice; a Newsreader serif carries the first-person reading text.

- **Manrope** (`display`): headings at 800 with tight letter-spacing, buttons at 700, meta text at 500, and "Studio" in the wordmark at 400.
- **Newsreader** (`body`): reading text at 400, with italic for rare emphasis and 500 where a little more weight helps.
- Headings use balanced line breaks. Body text stays under the `measure` token (about 36em).
- The hero style scales from 72px down to 40px on phones; section headings from 40px down to 28px.

## Logo

Two marks, both drawn from Manrope ExtraBold and kept as outlined vector files in Logos.

- **Wordmark:** "Sam Stone" at 800 and "Studio" at 400. The light version (`ink` and `accent`) sits on `ground` or white. The dark version (`on-navy` and `on-navy-accent`) sits on `brand-navy`.
- **Avatar:** a white "S." on a `brand-blue` circle. For Instagram, LinkedIn, the favicon and email.
- **Clear space:** keep at least the height of the capital S clear around the wordmark.
- **Minimum size:** the wordmark at 120px wide; the avatar down to 16px.
- **Don't** recolour either mark, stretch it, add effects, set the wordmark in another font, or put the light wordmark on navy.

## Layout

- A left-aligned editorial page, content up to `content-width`, sections separated by `line` hairlines with `space-9` padding.
- A section opens with a two-column head: the heading on the left (5 parts), a `muted` intro on the right (7 parts). Below 900px wide everything stacks into one column.
- Cards sit in a grid of three at `space-5` gaps and become one column on phones.
- Every control is at least 44px tall and shows a 3px `accent` focus ring.

## Components

Live previews are under Components.

- **Button**: the primary action and its plain-link partner.
- **Card**: a service or feature tile, with a highlighted variant for the lead offer.
- **Stat**: a big number with a label, and the stats band that holds several.
- **Decision ledger**: the inverted "Decisions before code" panel.
- **Instagram post**: the 1080 × 1350 post template.

## Instagram

- Posts are 1080 × 1350 (4:5). When uploading, choose "Original" in Instagram's crop menu; it defaults to square.
- Keep text inside the `post-margin` (96px). The profile grid shows posts cropped to 3:4.
- Ground is `brand-navy`; an occasional cover slide uses `brand-blue`. The headline is `post-headline` in `on-navy`, with its second half in `on-navy-accent`.
- The "S." mark sits top left and samstone.studio top right; the wordmark or an email address closes the post at the bottom.
- In a carousel, every slide takes the first slide's shape.

## Files

- `fonts/`: Manrope 400, 500, 700 and 800; Newsreader 400, 400 italic and 500. Latin and Central European characters (Czech included), under the SIL Open Font License (licence files alongside).
- Logos: `wordmark-light.svg`, `wordmark-dark.svg` and `avatar.svg`, plus PNG versions for places that don't take SVG (`avatar-1080.png` for profile pictures, the 1200px wordmarks for email signatures and documents).

## Token values

### Colour

| Token | Light | Dark | Use |
|---|---|---|---|
| `ground` | #f4f8fc | #0a1b30 | Page background: the pale blue-white ground of samstone.studio. |
| `surface` | #ffffff | #10294a | Cards and tiles on ground, always with a line border. |
| `ink` | #0e2744 | #eaf2fa | Headings and body text on ground or surface. Also the background of inverted panels (decision ledger, contact block), so they flip to light in the dark theme. |
| `muted` | #4a5b70 | #a3b6cb | Secondary text: section intros, role lines, stat labels, footnotes. Passes 4.5:1 on ground, surface and accent-soft in both themes. |
| `accent` | #1f5fa8 | #8dbdec | Links, the primary button, the second sentence of a headline, stat numbers, eyebrow labels, and "Studio" in the wordmark. |
| `accent-soft` | #dce8f5 | #173a63 | Soft panels: the stats band and the "How I actually work" note. Text on it is ink, muted or accent. |
| `line` | #c9d7e6 | #24446b | Hairlines between sections and rows, and card borders. Borders, not shadows. |
| `brand-navy` | #0e2744 | #0e2744 | Fixed navy that does not change with theme: Instagram post grounds and the background for the dark wordmark. Same value as ink in the light theme. |
| `brand-blue` | #2f6fb5 | #2f6fb5 | Logo blue: the avatar circle, the favicon and occasional Instagram cover slides. White text on it is 5.2:1. Never for body text. |
| `on-navy` | #f4f8fc | #f4f8fc | Main text on brand-navy: Instagram headlines, "Sam Stone" in the dark wordmark. |
| `on-navy-accent` | #8dbdec | #8dbdec | Accent on brand-navy: the second half of an Instagram headline, "Studio" in the dark wordmark, the dot in the post mark. |
| `on-navy-soft` | #dce8f5 | #dce8f5 | Secondary text on brand-navy: Instagram sublines and the samstone.studio label. |

### Type

| Style | Font | Size / line height | Weight | Tracking |
|---|---|---|---|---|
| `hero` | Manrope | 72px / 1.02 | 800 | -0.04em |
| `section` | Manrope | 40px / 1.08 | 800 | -0.03em |
| `title` | Manrope | 21px / 1.2 | 800 | -0.02em |
| `wordmark` | Manrope | 22px / 1 | 800 | -0.03em |
| `stat` | Manrope | 32px / 1 | 800 | -0.04em |
| `ui` | Manrope | 16px / 1.25 | 700 | 0 |
| `meta` | Manrope | 14px / 1.4 | 500 | 0 |
| `eyebrow` | Manrope | 12px / 1.3 | 700 | 0.1em |
| `lede` | Newsreader | 22px / 1.45 | 400 | 0 |
| `body` | Newsreader | 19px / 1.55 | 400 | 0 |
| `body-small` | Newsreader | 17px / 1.55 | 400 | 0 |
| `post-headline` | Manrope | 112px / 1.02 | 800 | -0.045em |
| `post-subline` | Manrope | 38px / 1.3 | 500 | 0 |

### Spacing, radius and layout

- Spacing: `space-1` 4px, `space-2` 8px, `space-3` 12px, `space-4` 16px, `space-5` 24px, `space-6` 28px, `space-7` 44px, `space-8` 56px, `space-9` 72px
- Radius: `radius-sm` 4px, `radius-md` 8px, `radius-lg` 12px, `radius-xl` 16px, `radius-full` 9999px
- Layout: `content-width` 1120px, `measure` 36em, `post-width` 1080px, `post-height` 1350px, `post-margin` 96px
