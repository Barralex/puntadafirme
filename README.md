# Sewing Atelier

**Venezuelan tailoring · Solymar, Ciudad de la Costa, Uruguay**

Landing page for a seamstress's atelier: alterations, uniforms, children's clothing, and the party dress that needs one last fix. Cloth, thread, and patience.

***

The roots of this workshop run three countries deep, and the vision arrived complete; fitting it on a page was the easy half. An online store, a booking calendar, a price list, a contact form: each was argued through and set aside, because each put a step between a person holding a garment and an answer, and none would earn back what it cost to keep alive. What is left is the craft itself, and one way to reach it.

***

A single static page: no build step, no dependencies, nothing to install. HTML, two typefaces, and [Leaflet](https://leafletjs.com) for the coverage map over Ciudad de la Costa. The dress form, the icons, and the 24-48 h seal are inline SVG, so they stay sharp at any size and cost no extra request.

```
index.html      the page
assets/         the two sewing machines
```

Published at `https://puntadafirme.com/`. The social preview tags and `CNAME` both carry that domain; change them together if it ever moves.

To update, edit `index.html` and:

```bash
git add . && git commit -m "Update" && git push
```

<p align="center"><sub>co-assisted by <b>Claude Opus 5</b></sub></p>
