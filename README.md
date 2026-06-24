# DeFi Risk Aggregator

A neutral aggregator of DeFi risk intelligence. It collects what the major risk feeds publish about the top Ethereum DeFi protocols and shows each feed's verdict verbatim, side by side. It produces no rating or score of its own. Where feeds disagree, you see the disagreement; where a feed is silent, the gap stays visible.

## Run it

One self-contained HTML file. No build step, no dependencies.

- Open `index.html` in any browser, or
- Serve the folder and open it: `python3 -m http.server` then visit http://localhost:8000

## What's inside

- One ring per protocol. Each slice is a single feed's verdict, coloured on that feed's own scale. The centre stays empty, because there is no overall score.
- A full protocol-by-feed matrix. Every cell is labelled covered, partial, or not yet covered, so the gaps show up as data instead of disappearing into an average.
- A methodology page that explains the no-composite-score rule.

In this prototype the feed verdicts are real and each one links to its public source; TVL is live from DefiLlama.

## Why no score of our own

No single feed should be the last word on something this important. Putting the feeds side by side, without averaging them, is the whole point. The no-score rule is a project commitment, not a default we can quietly change.

## License

AGPL-3.0 (see `LICENSE`). Read the code, trace any number back to the source it links to, and run the whole thing yourself.
