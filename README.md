# The CIDOC CRM Periodic Table: Documentation You Can Test

Slides for the talk at **Sci-K 2026** (6th International Workshop on Scientific Knowledge: Representation, Discovery, and Assessment), ISWC 2026, Bari, 26 October 2026. Planned at 11:35 for a 12-minute slot plus 3 minutes of questions.

Remo Grillo · University of Bologna · I Tatti, The Harvard University Center for Italian Renaissance Studies

- Live tool: [remogrillo.github.io/cidoc-crm_periodic_table](https://remogrillo.github.io/cidoc-crm_periodic_table/)
- Code: [github.com/RemoGrillo/cidoc-crm_periodic_table](https://github.com/RemoGrillo/cidoc-crm_periodic_table) · archived release: [doi.org/10.5281/zenodo.21821748](https://doi.org/10.5281/zenodo.21821748)

## Keys

| Key | Action |
|---|---|
| → / Space / click right | next step |
| ← / click left | previous step |
| P | presenter window: notes on top, current and next step below, each with a countdown bar for the slide's planned time; kept in sync, keys work in both windows |
| N | speaker notes and timer in the slides window |
| F | fullscreen |
| B | jump to the bonus tracks |
| T | restart the talk clock |
| R | reload the live demo on the current slide (back to its deep link) |
| O | show the screenshots instead of the live demos (no network); press again to go back |
| E | on a live demo: expand it to the whole slide (again to go back); also the ⤢ button in the top row |
| − / + / 0 | on a live demo: zoom the tool out (more of it fits) or in; 0 resets; also the − / + buttons in the top row |

On slide 2, the street names in the first entry are links: click one to open its entry, then follow the next. Clicking the scrolling manual stops or restarts it.

The deck is a single HTML file and its fonts are bundled, so it works offline. Only the three live demos (slides 10, 11, 12, and bonus 6) need the network: they load the real tool in an iframe. If the wifi fails, press O and the demos show screenshots of the same states. `#12.2` in the URL opens slide 12 at step 2. `?print` stacks every slide at its last step, with screenshots in place of the demos: print it to PDF from the browser.

## The live demos

- **A click inside a demo gives the keyboard to the tool.** Move the mouse off the demo and the slides take the keys back within half a second; the presenter window always drives the slides.
- Demo 1 (slide 10) opens `?ont=crm,crminf,crmdig,crmsci&code=S5`. Scroll the table, then show I1 Argumentation among the superclasses and the J2 row in the Properties tab.
- Demo 2 (slide 11) has no deep link for the triple builder, so the clicks are live: Explore → Experiment → domain S4 → property O8 → range (6 of 131 classes left) → S15.
- Demo 3 (slide 12) changes deep link at each step (or with its buttons): `S5,I2` → `S13,D9` → `D11,S13`. **Tick "hide loose paths" after each load**: the counts on the slide (1 and 3 sound chains) and in the paper hold only with that box ticked. Without it the tool lists 20, 6 and 8 direct paths, mostly loose.
- Every iframe load counts as page views in the tool's Google Analytics, rehearsals included. Presenter thumbnails and print mode show screenshots and load nothing.

## Sources

The numbers come from the paper (CEUR-WS Vol-4291). Slide 2: street data © OpenStreetMap contributors (ODbL), Overpass API, 25 October 2026; one entry per named street (355); the route is the shortest walk on that network (3.3 km), and the directions are read off it. Slide 3: Vermeer, *Young Woman with a Water Pitcher* (ca. 1662), The Metropolitan Museum of Art, open access (CC0), full resolution 3437 × 3866; operations, pigments and examinations are generic examples, not a record of this painting; page counts from the PDFs published on cidoc-crm.org (CRM 7.1.3: 234, CRMsci 3.2: 78, CRMdig 5.0: 35, CRMinf 1.2.1: 68). The demo states and path results were checked on the deployed tool on 25 October 2026. Slide 15: the GA4 export of 4 August 2026 (`paper_scik2026/periodic table report.csv` in the tool repository): monthly users from the daily series, cities with five or more users located with Nominatim, land outline from Natural Earth 1:110m (public domain). Mendeleev: weights as in the 1871 table; gallium (Lecoq de Boisbaudran, 1875), scandium (Nilson, 1879), germanium (Winkler, 1886).

Base CSS, slide engine and presenter window are reused from the QRAKEN deck for GLOW'26.
