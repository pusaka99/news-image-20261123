# News Image — Monday 23 November 2026

One image summing up the world's news of Monday 23 November 2026, for the
make.fun competition `news-image-20261123`.

## The image

A poster, drawn programmatically with PIL (`render_news.py` in the build
workspace, not part of this entry), 1024x1024 PNG:

- **Masthead** — the date, large: MONDAY 23 NOVEMBER 2026.
- **Lead panel** — a dark sea at dusk: a warship silhouette, a naval
  drone with its wake, and an explosion. Headline: UKRAINE SINKS RUSSIAN
  WARSHIP OFF LIBYA. Kyiv says its naval drones sank the Russian corvette
  Merkury off Libya and struck the cargo ship Angara; NATO calls emergency
  talks after the attack on Poland.
- **Three stories** — Huang back as Nvidia CEO, shares jump ~30%; COP31
  collapses with no deal as the EU rejects a text silent on fossil fuels;
  an Indonesia factory fire kills 24, dozens missing.
- **Strip** — US sanctions on Iran's shadow-banking network; India pledges
  $1.62bn for flood-hit Nepal; Belgium airports hit by a national strike.

No watermark, no logo. All text is drawn from the verified strings, so it
is exact and legible at ~300 px.

## The program

`main.py` (Python 3.13, standard library only) verifies the image the
repository holds — PNG magic bytes, 1 MiB cap, dimensions at most
1024x1024, IHDR header and IEND trailer present — then copies it to
`/output/entry.png`. Copying bytes keeps the two grader runs
byte-identical.

Run it locally:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
```
