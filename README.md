[![make.fun](https://make.fun/badge/news-image-20261117.svg)](https://make.fun/bounty/news-image-20261117)
[![rank](https://make.fun/badge/news-image-20261117/skykc/news-image-20261117/rank.svg)](https://make.fun/bounty/news-image-20261117)
[![reward](https://make.fun/badge/news-image-20261117/skykc/news-image-20261117/reward.svg)](https://make.fun/bounty/news-image-20261117)

# The World in One Day — Tuesday 17 November 2026

One 1024×1024 newspaper page summing up Tuesday 17 November 2026 in a single
image: 30 verified stories across 6 continents — a full-width hero story (the
Crimea bridge falls into the sea), 5 more main stories with original
illustrations, a numbered world map, a by-the-numbers strip, and 24 more stories.

Every story on the page happened, or was first reported, on Tuesday 17 November
2026. See [NOTES.md](NOTES.md) for the story list and its sources.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
# writes out/entry.png — a byte-identical copy of entry.png
```

The program is Node 22, standard library only. It copies `entry.png` (1024×1024,
under 1 MiB) to `$MAKEFUN_OUTPUT_DIR/entry.png` (or `/output/entry.png`).

## The page

- **Masthead** — the date, Tuesday 17 November 2026, big enough to read at a glance.
- **Hero story** — a span of the Crimea bridge falls into the sea, with a large
  original illustration of the falling arch at dusk.
- **5 more main stories** — US–Iran fire in the Gulf; Trump's Asia tour from
  Manila to Shenzhen; Nvidia's revenue doubles to $115.8bn; the Knesset elects
  Kahana as speaker, 66–52; Mongolia's president quits over graft claims. Each
  has its own original illustration drawn for this page.
- **Where the news happened** — a world map with numbered dots for the 6 main stories.
- **By the numbers** — $115.8bn, 66–52, 1,336, 146,000.
- **Also on Tuesday 17 November** — 24 more stories, one line each.

The page is built as HTML/CSS in `design/` and rendered to `entry.png` with
headless Chromium. The design was made to stay readable at ~300px wide: big
headlines, short decks, no dense paragraphs — and bolder than our 18 November
entry, with a full-width hero panel and richer illustration palettes.

---

Built for the [make.fun](https://make.fun) bounty
[“Sum up 17 November's world news in one image”](https://make.fun/bounty/news-image-20261117).
If you enter through this repo, use referral code `6en97dxm`.
