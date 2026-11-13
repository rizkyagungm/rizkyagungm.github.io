# Rizky Agung Mahendra — Digital Marketing Portfolio

Responsive one-page portfolio built with semantic HTML5, Tailwind CSS Play CDN, custom CSS, and vanilla JavaScript.

## Run locally

1. Extract the ZIP.
2. Keep `index.html` and the `images/` folder together.
3. Open `index.html` in a modern browser. A local server also works, for example `npx http-server .`.

## Update photos and campaign images

The images are stored in the `images/` folder:

| File | Location | Recommended content |
|---|---|---|
| `hero-portrait.svg` | Main hero image | Your professional portrait, vertical 4:5 |
| `campaign-automotive.svg` | Gallery item 1 | Daihatsu campaign creative or an approved ads screenshot |
| `campaign-coffee.svg` | Gallery item 2 | Janji Jiwa social post or campaign creative |
| `campaign-furniture.svg` | Gallery item 3 | Decoblanca campaign creative |

To use a JPG/PNG/WebP, copy it into `images/`, then update the corresponding `src` in `index.html`. For gallery images, update both the button's `data-lightbox-src` and the thumbnail's `<img src>` to the same path. The large modal uses `data-lightbox-src`; the grid thumbnail uses `<img src>`.

For example, if you add `images/rizky.jpg`, change the hero image from:

```html
<img class="hero-image" src="images/hero-portrait.svg" ...>
```

to:

```html
<img class="hero-image" src="images/rizky.jpg" alt="Rizky Agung Mahendra" ...>
```

## Included features

- Responsive desktop sidebar and mobile navigation drawer
- Dark/light mode with saved preference
- Smooth section navigation and active-section indication
- Subtle scroll reveal with reduced-motion support
- Back-to-top control and sticky contact bar
- Image modal opens over the current scroll position; close button, Escape, and backdrop click dismiss it
- Desktop custom cursor, disabled on touch screens and for reduced-motion preference

## Before deployment

- Use your own approved portrait and campaign creatives in the `images/` folder.
- Confirm contact details and campaign figures before publishing.
- Tailwind Play CDN is used for convenient static use. For a high-traffic deployment, compile Tailwind locally and serve the resulting CSS as a static asset.
