# 📈 Even Money

A small, self-contained browser game that teaches the math of risk, leverage, and compounding. Start with **$100** and try to reach **$1,000,000**.

Each round you pick a move, then a hidden card numbered 2–10 is revealed. Even or odd decides whether you win.

## How to play

Choose one of four moves (click, or press keys **1–4**):

| Move | Win | Loss |
| --- | --- | --- |
| **Go Long** | Even → 2× your money | Odd → 0.5× |
| **Go Short** | Odd → 2× your money | Even → 0.5× |
| **Lever Up** | Even → 4× your money | Odd → $0 |
| **Hold** | No change | No change |

Every move advances the clock by three months. Hit **$1,000,000** to win (you'll see how many years it took); hit **$0** and you're out. Use the **Repeat** box to rapid-deal many rounds at once.

## Running it

It's a single static `index.html` with no dependencies or build step. Just open the file in a browser, or host it on any static host (see below).

## Hosting on GitHub Pages

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
4. Select branch **`main`** and folder **`/ (root)`**, then **Save**.
5. Wait ~1 minute; your game will be live at `https://<username>.github.io/even-money-game/`.

## License

[MIT](LICENSE) — see the [game specification](GAME_SPEC.md) for the original design notes.
