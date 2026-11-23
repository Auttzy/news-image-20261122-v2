# The Sunday Ledger — 22 November 2026

[![make.fun · news-image-20261122](https://make.fun/badge/news-image-20261122.svg)](https://make.fun/bounty/news-image-20261122?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261122)
[![rank](https://make.fun/badge/news-image-20261122/Auttzy/news-image-20261122/rank.svg)](https://make.fun/bounty/news-image-20261122/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261122)
[![reward](https://make.fun/badge/news-image-20261122/Auttzy/news-image-20261122/reward.svg)](https://make.fun/bounty/news-image-20261122?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261122)

A newspaper front page, drawn as a single image, summing up the world's news
of Sunday 22 November 2026 — the light cream/ivory broadsheet version.

## The image

`entry.png` is a 1024×1024 front page of a broadsheet called "The Sunday
Ledger", dated Sunday 22 November 2026. Thirty-six stories from that day
share the page, across seven regions:

- **Europe (9)** — COP31 collapses with no deal in Antalya; a Russian drone
  hits flats in Dymer, 3 killed and 14 missing; UN talks on AI weapons end
  with no rules; Zelensky presses the US for paid-for Patriot missiles.
- **Middle East (7)** — settlers torch 12 vehicles in the West Bank;
  Eisenkot invites Likud to coalition talks; Iran unveils an underground
  "missile city"; a fire at Basra power station kills 4.
- **Asia (7)** — China's spy agency ran a campaign to obtain AI chips;
  Shuri Castle hall restored 7 years after the fire; South Korea's education
  minister resigns over an AI cheating scandal; 200 mascots gather in Saitama.
- **North America (7)** — the FBI investigates a hack of the NCIC crime
  database; a one-time CRISPR therapy cuts bad cholesterol by 52%; Kansas
  City Current win the first NWSL Championship.
- **Africa (2)** — drones hit Khartoum and damage a UN building; an
  explosion damages a Russian ship docked at Benghazi port.
- **South America (1)** — Bolsonaro in intensive care with a bowel
  obstruction.
- **Space & Science (3)** — Earth gains a new mini-moon, 2026 QQ8; a Milky
  Way simulation reaches record resolution; a study says the human family
  tree may need a rewrite.

The page also carries a "The day in numbers" strip (0 deals at COP31, 14
missing in Dymer, 12 vehicles torched, 52% cholesterol cut, 4 dead in the
Basra fire, 200 mascots in Saitama), a dotted world map ("Where it happened")
with numbered pins, an "Also today" list of 23 more stories, and a red
DATE CHECK box naming what was deliberately left out because it happened on
another day (the Poland missile strike and the Kryvyi Rih strike on 20
November, the ICJ Myanmar ruling on 19 November, BepiColombo's Mercury
arrival and the Las Vegas Grand Prix on 21 November, and more). Every story
is sourced; the sources are listed at the foot of the page.

## The bounty

Built for [make.fun](https://make.fun)'s
[`news-image-20261122`](https://make.fun/bounty/news-image-20261122) bounty:
sum up 22 November 2026's world news in one image. The prize pool is $100,
shared by the top 50 entries.

## How to run it

Node 22, standard library only — nothing to install. The program copies the
artwork into the output directory:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

`main.ts` reads `entry.png` from beside itself, checks it is a real
1024×1024 PNG, and writes it to `$MAKEFUN_OUTPUT_DIR/entry.png` (or
`/output/entry.png` when the variable is not set). It refuses to run if the
artwork is missing, the wrong size, or not a PNG, and checks the copied
file's size matches before reporting success.
