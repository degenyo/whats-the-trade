# What's the Trade

A Claude skill that turns any piece of news into an actionable trade thesis.

Feed it a headline, tweet, article, rumor, or policy announcement — it gives you back:

- **The Trade** — the actionable move, stated with conviction
- **Tickers** — specific assets that benefit, get hurt, and second-order plays
- **Narrative** — what bigger thesis this plugs into
- **Timeframe & Conviction** — is this a now trade or a building trend, and how confident

## Why

Every trader sees news and thinks "okay but what's the trade." This packages that thought process into a reusable tool. It's opinionated by design — no hedge-everything disclaimers, no "investors should consider" corporate speak. Just: here's the trade, here's why, here's how to play it.

## Example

**Input:**
> Matt Shumer posts "Something Big Is Happening" — viral thread comparing AI's current moment to early COVID, says he's no longer needed for the technical work of his job

**Output:**
> 🎯 **The Trade:** Long AI infrastructure and tooling. This is the "normie awakening" moment — position ahead of enterprise adoption spend that follows awareness.
>
> 📊 **Tickers:** Bullish $NVDA, $MSFT, $PLTR. Bearish $UPWK, $FVRR, Indian IT. Second-order: $CRWD (more AI code = more attack surface), $RENDER/$AKT (decentralized compute).
>
> 📖 **Narrative:** "AI is eating software" — the perception flip from overhyped to underhyped reprices the entire sector.
>
> ⏱️ **Conviction:** Medium. Narrative accelerant, not fundamental catalyst. Invalidation: visible AI plateau in next 6 months.

## Install

This is a [Claude skill](https://docs.anthropic.com). To use it:

1. Clone this repo
2. Place the `whats-the-trade` folder in your Claude skills directory
3. Start pasting news

## Structure

```
whats-the-trade/
├── SKILL.md                          # Core skill instructions
├── README.md                         # You're here
└── references/
    ├── narratives.md                 # Narrative-to-ticker mapping (update this)
    ├── trade-framework.md            # 5-layer analysis engine
    └── news-categories.md            # News classifier with trigger words
```

## Customization

The **`references/narratives.md`** file is the one you'll want to keep updated. It maps narratives to tickers — as markets evolve, new tokens launch, and narratives shift, update the mappings. Everything else is structural and shouldn't need frequent changes.

## License

MIT — do whatever you want with it.
