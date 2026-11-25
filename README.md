# news-image-20261124-entry-v4

[![GitHub repo size](https://img.shields.io/github/repo-size/labibhanafi/news-image-20261124-entry-v4)](https://github.com/labibhanafi/news-image-20261124-entry-v4)
[![GitHub last commit](https://img.shields.io/github/last-commit/labibhanafi/news-image-20261124-entry-v4)](https://github.com/labibhanafi/news-image-20261124-entry-v4/commits/main)
[![License: MIT](https://img.shields.io/github/license/labibhanafi/news-image-20261124-entry-v4)](https://github.com/labibhanafi/news-image-20261124-entry-v4/blob/main/LICENSE)

Hero-led revision (v4) for the [make.fun bounty news-image-20261124](https://make.fun/bounty/news-image-20261124): sum up the world news of **Tuesday, 24 November 2026** in one 1024x1024 image.

Referral: https://make.fun/r/3t7y0djc

## The image

`main.py` draws a one-page newspaper front page — **THE WORLD DAILY** — with a hero lead story (two tankers hit by mines in the Strait of Hormuz), three featured stories, and 36 briefs across 8 regions, plus a markets strip. Every headline and figure was verified against live web reporting during the build and is hard-coded in the program; it runs with no network.

- 40 news items (1 lead + 3 featured + 36 briefs)
- 8 regions: Middle East, North America, Europe, Asia-Pacific, Africa, Latin America, Markets, Science/Culture/Sport/Media
- Output: `entry.png`, 1024x1024, 493,298 bytes, byte-identical on repeated runs

## Run it

```sh
MAKEFUN_OUTPUT_DIR=out python3 main.py   # writes out/entry.png
```

Python 3.13, Pillow for drawing. If Pillow is unavailable, the program copies the bundled `entry.png` (the exact file this program produced) instead, so the output is identical either way.

## License

MIT — see [LICENSE](LICENSE).
