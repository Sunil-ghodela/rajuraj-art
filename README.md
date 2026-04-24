# RajuRaj art — landing page

Standalone brand site for **Raju Raj Manav** — handcrafted Himalayan miniatures from New Tehri, Uttarakhand.

## Preview locally (right now)

Just open the file in a browser. No build, no server, no install needed.

```
file:///home/vaibhav/AI/Jan-April.../RajuRajArt/index.html
```

Or from the file manager — double-click `index.html`. Tailwind loads from CDN, fonts from Google Fonts, images are local.

## Deploy free on Vercel (5 minutes)

**Easiest way — drag & drop:**

1. Go to [vercel.com](https://vercel.com) → sign up with GitHub or email (free).
2. Click "Add New… → Project" → "Browse all templates" → scroll down to "Other" → choose **"Static HTML"** OR just drag the entire `RajuRajArt` folder onto the deployment zone.
3. Vercel auto-detects, deploys, gives you a URL like `rajurajart.vercel.app`.
4. Done. Share that link.

**CLI alternative (if you prefer terminal):**

```bash
cd /home/vaibhav/AI/Jan-April.../RajuRajArt
npx vercel              # follow prompts, login once
npx vercel --prod       # promote to production
```

## What to customize before going live

Search for these in `index.html` and replace:

| Find | Replace with |
|------|--------------|
| `91XXXXXXXXXX` (appears 7 times) | Raju's or your WhatsApp number with country code, e.g. `919876543210` |
| Piece names ("The Village", "Lavender Peaks", etc.) | Whatever Raju wants to call them — Hindi names, place names, anything |
| Prices (`₹1,500`, `₹1,400`, etc.) | Final per-piece prices |
| Piece descriptions (italic line under each name) | Edit if Raju wants different language |
| The artist quote (English + Hindi blocks) | Refine if Raju gives a slightly different version on his voice note |

## File structure

```
RajuRajArt/
├── index.html          ← the entire site (single file)
├── README.md           ← this file
└── images/
    ├── village.jpeg            ← hero piece (with houses)
    ├── village-alt.jpeg
    ├── lavender-peaks.jpeg
    ├── lavender-peaks-alt.jpeg
    ├── mossy-peaks.jpeg
    ├── mossy-peaks-alt.jpeg
    ├── twin-caps.jpeg
    ├── twin-caps-alt.jpeg
    ├── first-snow.jpeg
    ├── first-snow-alt.jpeg
    ├── budding-peak.jpeg
    └── budding-peak-alt.jpeg
```

`-alt.jpeg` are the second-angle photos — not used yet on the page, but available for a future "view more angles" feature.

## Brand notes

- **Voice**: minimal. The artist's quote does the heavy lifting. No founder story, no charity framing. Standalone brand.
- **Palette**: snow white (`#f7f5f0`), moss deep (`#2f4a2a`), earth brown (`#5c4933`) — pulled from the art itself.
- **Typography**: Cormorant Garamond (serif, art-gallery feel) for headings + quote. Inter (clean sans) for body.
- **Mobile-first**: tested implicitly via Tailwind's responsive utilities. Hero is full-screen on phone.
- **Performance**: single HTML, no JS framework, CDN-only deps. Loads fast on weak network.

## What's NOT in v1 (deliberately, for later)

- Instagram embed (do this in week 2 once Insta is live)
- Process photos / making-of section (need fresh photos from Raju)
- Customer reviews / testimonials (need first orders first)
- Multi-page navigation (single page is enough at this scale)
- Analytics (add Vercel Analytics post-launch if needed)
- Form-based ordering (WhatsApp is the ordering mechanism)
