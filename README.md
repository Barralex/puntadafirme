# Zulari Valderrama · Sewing Atelier

**Venezuelan tailoring · Solymar, Ciudad de la Costa, Uruguay**

Landing page for a seamstress's atelier: alterations, uniforms, children's clothing, and the party dress that needs one last fix. Every enquiry ends on WhatsApp, so the whole page is built to get there in a single tap.

***

## The brief

The starting point was a description of the work, not a specification: decades of trade, a clientele built by word of mouth, and a workshop where the conversation already happens on WhatsApp. Turning that into a page was mostly a matter of agreeing on what to leave out.

An online store, a booking calendar, a price list, and a contact form were each considered and set aside. Every one of them puts a step between a person holding a garment and an answer from the workshop. One channel survived, and the page repeats it wherever a visitor is likely to be ready.

What stayed, each section answers a question that already comes up in person:

- **Coverage map** — *"do you come to my neighbourhood?"* Drawn as an area rather than a pin, because the answer is a zone and its edges are open to discussion.
- **The two machines** — an inherited trade is the thing no competitor can copy, so it earns a section of its own instead of a line in an About.
- **24-48 h** — a turnaround the workshop can hold on a normal week. Stated once, plainly, and not repeated.
- **No prices** — every job is quoted from a photograph. That quote is the reason to write, so the page asks for the photograph instead of guessing at a number.

The copy is in Spanish and in the first person, for the same reason: the page should sound like the workshop, not like an agency.

***

A single static page: no build step, no dependencies, nothing to install. HTML, two typefaces, and [Leaflet](https://leafletjs.com) for the coverage map over Ciudad de la Costa. The dress form, the icons, and the 24-48 h seal are inline SVG, so they stay sharp at any size and cost no extra request.

```
index.html      the page
assets/         the two sewing machines
```

Social preview tags point at `https://barralex.github.io/zulari-atelier-page/`. Change that base if the atelier moves to a domain of its own.

To update, edit `index.html` and:

```bash
git add . && git commit -m "Update" && git push
```

<p align="center"><sub>co-assisted by <b>Claude Opus 5</b></sub></p>
