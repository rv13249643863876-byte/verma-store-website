# Aapka Family Store – Verma Store, Mangolpuri

A responsive, frontend-only website for **Verma Store**, a neighbourhood general store, stationery and photocopy shop in X Block, Mangolpuri (Delhi). Customers can browse the shop's items, search them instantly, build a basket and send the list to the shop on WhatsApp.

> Frontend only. No backend, no database, no API keys.

**Live link:** _add your GitHub Pages link here_

## What it does

- **Instant item search** – type "aata", "pen" or "lamination" in the search bar and matching items appear right away, with an **Add** button and a quantity stepper. Works with Hindi and English spellings, and tolerates small typos.
- **Category browsing** – 9 categories (daily essentials, dairy and snacks, stationery, ice creams, photocopy, printout, lamination and more) opening into tap-to-add item lists.
- **Basket** – add, change quantity or remove items. The basket is saved in the browser (`localStorage`), so it survives a page reload.
- **Order on WhatsApp** – the basket is turned into a ready-made message and opened through a `wa.me` link. There is also a copy-list option and a "previous list" to reorder quickly.
- **Live open / closed status** – calculated from the shop's daily timings in Indian Standard Time.
- **Profile** – a small saved profile (also in `localStorage`).
- **3D hero** – an animated shop scene built with three.js.
- **Mobile first** – designed for phones (safe-area aware, large tap targets), also works on desktop.

## Tech stack

| Area | Used |
| --- | --- |
| Structure, styling, logic | HTML, CSS, vanilla JavaScript (single `index.html`) |
| 3D scene | [three.js](https://threejs.org/) r128, loaded from cdnjs |
| Fonts | Google Fonts (Baloo 2, Nunito Sans) |
| Storage | Browser `localStorage` |
| Ordering | WhatsApp `wa.me` deep link |

## How to run

1. Download or clone this repository.
2. Open `index.html` in any modern browser. No build step or install is needed.

An internet connection is needed for the first load (three.js and fonts come from a CDN). If they cannot load, the rest of the site still works.

Optional local server:

```bash
python -m http.server 8000
# then open http://localhost:8000
```

## Project structure

```
.
├── index.html   # the whole site: markup, styles and scripts
└── README.md
```

## Development notes

_Edit this section so it is true for you._

- Idea and use case: a real shop I know, built so customers can send their list without calling.
- I built this with the help of an AI assistant (Claude). _Write here which parts you did yourself, for example the content, the item lists, testing, and the changes you asked for, and what you learned._
- Tested on a phone-sized and a desktop-sized browser window.

## Contact (shop)

X Block, Mangolpuri, near Sanjay Gandhi Memorial Hospital, Delhi.
