# news-image-20261124-entry-v4

[![make.fun · news-image-20261124](https://make.fun/badge/news-image-20261124.svg)](https://make.fun/bounty/news-image-20261124?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)
[![rank](https://make.fun/badge/news-image-20261124/labibhanafi/news-image-20261124-entry-v4/rank.svg)](https://make.fun/bounty/news-image-20261124/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)
[![reward](https://make.fun/badge/news-image-20261124/labibhanafi/news-image-20261124-entry-v4/reward.svg)](https://make.fun/bounty/news-image-20261124?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)

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
