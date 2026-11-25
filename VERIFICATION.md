# VERIFICATION — news-image-20261124 v4 (hero-led revision)

Built: 25 Nov 2026, ~20:40–21:00 WIB. Builder session: this build session
(subagent task news-image-20261124 v4, parent job makefun-watch).

## Output

- Program: `main.py` (Python 3.13, Pillow draw; no network at grading; falls
  back to copying the bundled `entry.png` if Pillow is unavailable)
- Image: `entry.png`, 1024x1024 RGB PNG
- Bytes: **493,298** (target >= 430 KB / 440,320 B and <= 1 MiB — PASS)
- SHA-256 (2 runs, byte-identical): **30333e010ff3efe8cf7825328ae506427b2f030152eb5cc34c5c25cf06fd41f7**
- Run time: ~0.6 s per run (limit 60 s — PASS)
- 300 px downscale check: masthead, date, hero headline, art panel and
  markets band all legible at ~300 px; briefs read as a dense newspaper
  index, as intended.

## Counts

- News items: **40** (1 lead + 3 featured + 36 briefs) — target >= 35 PASS
- Regions: **8** — Middle East, North America, Europe, Asia-Pacific,
  Africa, Latin America, Markets, Science/Culture/Sport/Media — target
  >= 7 PASS
- Date on image: "TUESDAY, 24 NOVEMBER 2026" (verified: 24 Nov 2026 is a
  Tuesday)

## Lead story

**TWO TANKERS HIT BY MINES IN THE STRAIT OF HORMUZ** (Middle East)

- Iran's Revolutionary Guards Navy said two oil tankers struck naval mines
  and caught fire early on Tuesday, 24 Nov 2026 (statement carried by
  Iranian state media; Reuters: could not independently verify).
- UKMTO Warning 219-26: three vessels struck by unknown projectiles while
  transiting eastbound at 00:25 UAE time, 24 Nov; all crew accounted for.
- JMIC keeps the Strait threat level "severe"; traffic 65% below pre-war
  levels; 227 vessels at anchor east of the strait.
- Sources: Reuters (25 Nov), OilPrice, UKMTO via Dubai Press, JMIC via
  Dubai Standard.

## Featured stories

1. MARKETS — "DOW CLOSES ABOVE 50,000": Dow 50,018.70 +0.85%; Nasdaq
   -1.48%; Nvidia -5.86% to $155.38 (Dow Jones / Morningstar 24 Nov;
   Argus).
2. ASIA-PACIFIC — "CHINA LAUNCHES SHENZHOU-24": Pakistani astronaut
   Zeeshan Ali, first foreign flyer to Tiangong (AP 24 Nov; Straits Times).
3. EUROPE — "UKRAINE HITS TWO SAMARA REFINERIES": hours after Putin calls
   retaliation "inevitable" (Financial Times via Daily Digest 24 Nov).

## Briefs (36) — sources, all 24 Nov 2026

- Middle East (7): Aden/Houthis 60 km (Daily Summary Of); Riyadh tower,
  11 wounded (Daily Summary Of); Katz chemical weapons (AP/Breitbart);
  Al-Amari raid + 3 killed in Gaza (Arab News 24 Nov 06:00 GMT); Oxfam
  "toxic land" (Horizon); 41 killed in Saudi strikes (RNA News); Iran
  rules out talks, 7 conditions (Horizon).
- North America (7): Trump "probably doable" (Breitbart); US tariffs on
  China/EU (AP); consumer confidence 103.3 vs 91.9 (Dow Jones/Conference
  Board); Pentagon rebukes Canada (AP); Abrego Garcia to Spain (Daily
  Digest); measles 9th death, 46 counties (Horizon); Coast Guard boards
  2 ships (Breitbart).
- Europe (5): Russian strike kills 2, wounds 48 (AP); Ukraine drones hit
  Russian ship off Libya (AP); German business sentiment up (Dow Jones);
  Anmer break-in, 2 held (News Media House); GTA VI hacker freed (Breitbart).
- Asia-Pacific (7): N. Korea shuts Swiss office (AP); Solomons pick
  Australia (AP); Nepal quake 5.6, no deaths (NEMRC via Jagran Josh);
  Hanoi blast kills 6 (Reuters); China sentences spy to death (AP);
  Hasina returns Dec 16 (Breitbart); China eases export curbs (Dow Jones).
- Africa (2): Tripoli questions Kyiv (Horizon); RSF drones hit Khartoum
  (RNA News).
- Latin America (4): 25 hostages in Cartagena (Daily Summary Of/AP);
  Mexico tries "El Chapo Isidro" (Horizon); Maduro birthday in jail
  (Breitbart); Flavio Bolsonaro summoned (Breitbart).
- Science/Culture/Sport/Media (4): record quasar, 630m years after Big
  Bang (AP); Pope's diary "gates of hell" (AP); Arsenal held by Dortmund
  (News Media House); AP editor Ellen Nimmons dies at 78 (AP).
- Markets strip: Dow 50,018.70 +0.85%, S&P 500 7,201.09 -0.50%, Nasdaq
  23,733.54 -1.48%, WTI $82.05 +2.4%, Gold $3,556 -2.6% (Daily Digest /
  Argus, 24 Nov closes).

Excluded on purpose: items dated Monday 23 Nov (ICJ Rohingya affirmation,
Guterres AI-framework call, Nvidia Huang reinstatement) — only the 24 Nov
market reaction to the Huang return is used.

## Kit check

- Local kit: `news-image-20261124-kit-extract`, bundle_sha256
  `4b5efc94df5f7f13825c507da56ccbb2c28bfefaa6d9e78930db672cc4b17c10`.
- Fresh download from https://make.fun/c/news-image-20261124/kit on
  25 Nov 2026: same bundle_sha256, same pricing_rev, same scorer
  program — kit level unchanged, no refresh needed.

## Iteration note (v4 vs v1/v3)

v1 (R1 rank 852/7302) and v3 (R3 rank 3158/14561) used the same dense
3-column recipe; rank worsened as the field grew 7302 -> 14561. v4 pivots
to a hero-led front page: one dominant lead story with illustration,
larger headline typography, three featured stories, then a dense briefs
index — same verified facts, clearer hierarchy and thumbnail legibility.
