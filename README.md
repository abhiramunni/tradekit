# TradeKit — Your Trading Journal & Risk Desk

Every trade teaches. Write it down.

TradeKit is a private, single-file web app for keeping a trading journal: log each trade, see your real win rate, profit factor and average R, watch your equity curve grow, and size every position from the risk you choose — never from a feeling.

**Live:** https://abhiramunni.github.io/tradekit/

## What it does

- **Trade ledger** — log trades with date, symbol, direction (long/short), entry, exit, size in lots, stop-loss, target and one honest line about why you took it. Leave the exit blank and a trade stays open; close it from its detail drawer later.
- **Honest stats** — net P&L, win rate, profit factor, average R, average win/loss and current streak, all worked out from the trades you log. No numbers are typed by hand.
- **Equity curve** — a canvas chart of your running total after each closed trade.
- **Position-size calculator** — enter account size, risk % per trade, entry, stop and target; the desk returns how much you risk, the size in lots (and ounces for gold — 1 lot = 100 oz), and the reward-to-risk ratio, in plain words.
- **Today's discipline check** — six pre-trade checks (trend checked, stop set before entry, risk ≤ 1%, trading the plan, reason written down, stop never moved away) plus a daily journal note, saved per day.
- **Six plain-language guides** — risk first, one setup at a time, writing the why, Sunday review, losses as tuition, never risking money you need.
- **Private by design** — everything lives in your browser's localStorage. Nothing is uploaded anywhere. Sample trades are marked and removable in one tap; erase-all is two taps.

## What it is not

TradeKit is a journal, not advice. It never tells you what to buy or sell, never shows a signal, and never predicts a price. P&L is worked out from the prices you type — always check it against your broker.

## How to use it

1. Open the live link (or open `index.html` locally).
2. Skim the 3-step tour.
3. Remove the sample trades from the footer once you have logged your own.
4. Before each trade, tick the discipline checks; after each trade, log it in ten seconds.
5. Every Sunday, read your notes and ask: did I follow my plan?

## Tech

- One self-contained `index.html` — no backend, no signup, no build step.
- Vanilla HTML/CSS/JS, Fraunces + Inter, localStorage only.
- Two AI-generated warm-editorial photographs (trading desk hero, journal flat-lay) with a slow Ken Burns drift.
- Warm editorial palette (ivory paper, espresso ink, bronze/gold, terracotta) with a full-screen cinematic intro and tap-to-skip.

## Run the checks

```bash
node qa-test.js   # headless jsdom assertions (76 checks)
```

## License

MIT — use it, fork it, make it yours.
