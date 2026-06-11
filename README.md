# JAMILLA — Architecture & Street Photography

A self-hosted portfolio site in a single HTML file, featuring interactive
three.js scenes: a rotating turntable showcasing three Filipino-inflected
buildings (residence, apartment, storefront) and a capiz-shell window
turning in passing light.

## Running it

No build step, no dependencies to install.

- **Locally:** open `jamilla-3d.html` in any modern browser.
- **Hosted:** upload the file to any static host (Netlify, Cloudflare Pages,
  GitHub Pages, or your own server). Rename it `index.html` so it loads at
  your domain root.

An internet connection is required for three.js (loaded from a CDN), Google
Fonts, and the placeholder images.

## Interacting with it

- The hero turntable rotates to a new building every 9 seconds.
- **Tap/click** to advance, **swipe left/right** to turn in either direction.
- Moving the mouse adds parallax; scrolling lifts the camera away.

## Customizing

Everything lives in `jamilla-3d.html`:

- **Photos:** the project list near the bottom of the `<script>` section uses
  `picsum.photos` placeholder URLs. Replace them with paths to your own
  images (e.g. `images/concrete-hymn.jpg`) and commit the images alongside.
- **Project titles:** edit the `projects` array in the same place.
- **Colors:** the palette is defined once as CSS variables in `:root` at the
  top of the `<style>` block.
- **Contact details:** search for `hello@jamilla.photo` and the social links
  in the Contact section.

## Working offline / removing the CDN

Download `three.min.js` (r128), place it next to the HTML file, and change
the script tag to `<script src="three.min.js"></script>`.

## License

All rights reserved — see [LICENSE](LICENSE). This is a personal portfolio;
the code and photographs are not licensed for reuse.
