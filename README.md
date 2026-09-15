# Puntada Firme

**Venezuelan tailoring · Solymar, Ciudad de la Costa, Uruguay**

Landing page for a seamstress's atelier: alterations, uniforms, children's clothing, and the party dress that needs one last fix. Cloth, thread, and patience.

***

The roots of this workshop run three countries deep, and the vision arrived complete; fitting it on a page was the easy half. An online store, a booking calendar, a price list, a contact form: each was argued through and set aside, because each put a step between a person holding a garment and an answer, and none would earn back what it cost to keep alive. What is left is the craft itself, and one way to reach it.

***

A single static page: no build step, no dependencies, nothing to install. HTML, three typefaces, and [Leaflet](https://leafletjs.com) for the coverage map over Ciudad de la Costa. The icons, the flag, and the 24-48 h seal are inline SVG, so they stay sharp at any size and cost no extra request.

```
index.html                     the page
assets/                        images
.github/scripts/check.py       checks the page before it goes out
.github/workflows/deploy.yml   publishes to GitHub Pages
```

The hero photos (`hero-*.webp`) are CC0 from [rawpixel](https://www.rawpixel.com): free for commercial use, no attribution required. The current machine (`maquina-actual.jpg`) is by [storebukkebruse](https://www.flickr.com/photos/8536261@N07/13937583028) under [CC BY 2.0](https://creativecommons.org/licenses/by/2.0/), credited in the footer.

Published at `https://puntadafirme.com/`. The social preview tags and `CNAME` both carry that domain; change them together if it ever moves.

To update, edit `index.html` and:

```bash
git add . && git commit -m "fix(landing): short description" && git push
```

Every push to `main` runs `check.py` first: broken markup, a missing file, or a bad social preview tag stops the deploy and the live site stays as it was.

Commits follow `type(scope): short message`, e.g. `feat(landing): add reviews`, `fix(deploy): ...`, `docs(readme): ...`.

<p align="center"><sub>co-assisted by <b>Claude Opus 5</b></sub></p>
