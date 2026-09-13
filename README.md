# Zulari Valderrama · Sewing Atelier

**Venezuelan tailoring · Solymar, Ciudad de la Costa, Uruguay**

Landing page for a seamstress's atelier: alterations, uniforms, children's clothing, and the party dress that needs one last fix. Every enquiry ends on WhatsApp, so the whole page is built to get there in a single tap.

***

## Client work

Designed and built by [Luis Barral](https://barralex.github.io) for Zulari Valderrama. The atelier owns the brand, the copy, and the photographs; this repository holds the code.

***

A single static page: no build step, no dependencies, nothing to install. HTML, two typefaces, and [Leaflet](https://leafletjs.com) for the coverage map over Ciudad de la Costa. The dress form, the icons, and the 24-48h seal are inline SVG, so they stay sharp at any size and cost no extra request.

```
index.html      the page
assets/         the two sewing machines
```

The page is in Spanish because its readers are.

Social preview tags point at `https://barralex.github.io/zulari-atelier-page/`. Change that base if the atelier moves to a domain of its own.

To update, edit `index.html` and:

```bash
git add . && git commit -m "Update" && git push
```

## Contact

- Atelier: [WhatsApp](https://wa.me/59899485236)
- Development: luis.enrique.barral@hotmail.com

<p align="center"><sub>co-assisted by <b>Claude Opus 5</b></sub></p>
