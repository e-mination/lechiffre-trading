# LeChiffre — TradingView portfolio

Public portfolio for **Elie Minassian** ([e-mination](https://github.com/e-mination)): a rule-based **XAUUSD** method, a **Pine Script** indicator on TradingView, the **5M LeChiffre** Telegram channel, and the site [lechiffre.online](https://lechiffre.online/).

This repository is the static site. It is the author’s own work — the indicator, the channel, and the website — documented with screenshots. The Strategy Tester images are example 30-day paper runs, not an audited live account, and this is not financial advice.

## Links

| | |
| --- | --- |
| Method site | [https://lechiffre.online/](https://lechiffre.online/) |
| GitHub Pages | [https://e-mination.github.io/lechiffre-trading/](https://e-mination.github.io/lechiffre-trading/) |
| Author | Elie Minassian · [minassianelie@gmail.com](mailto:minassianelie@gmail.com) |
| GitHub | [github.com/e-mination](https://github.com/e-mination) |

The GitHub repository homepage is already set to [lechiffre.online](https://lechiffre.online/). The Pages link above is the address for this portfolio once GitHub Pages is enabled from the `main` branch root.

## What’s on the site

- **Hero** — LeChiffre as a rule-based XAUUSD method, with links to the product site, the Pine indicator, and the Telegram channel.
- **TradingView / Pine Script** — the XAUUSD 5-minute chart: entries, session shading (including London), a Forex Factory news table, and WIN tags.
- **Strategy Tester** — paper examples of **LeChiffreXtelegram** on a $10,000 account: 1m, 3m, 5m, 15m, 30m, and 4H, for 7 days and 30 days where a screenshot is included. No 1-hour report. PnL shown for 0.1 lot size.
- **Telegram** — the 5M signal thread, plus best-day summaries for 1M, 3M, 5M, and Fifteen+. PnL shown for 0.1 lot size.
- **Website** — what [lechiffre.online](https://lechiffre.online/) is for.
- **Note** — not financial advice. Paper-test figures and the channel’s example day are not an audited live record.

A second page, [`gallery.html`](gallery.html), shows the screenshots larger.

## Example day in the screenshots

The Telegram screenshot is from **22 September 2026**. The daily summary card on that image reads:

- Asset **XAUUSD**, timeframe **5**
- **10** wins, **2** losses, **12** trades, **83.3%** win rate
- Net PnL **414.09**. PnL shown for 0.1 lot size.

One confirmed signal in the same thread:

- **BUY** XAUUSD (5), signal time **22/09/2026 06:30 GMT+3**, exit **06:40 GMT+3**
- Entry **4344.649**, take profit **4347.778**, stop **4341.520**, risk/reward **1**
- Result card: **TRADE WON**, realized PnL **31.29**. PnL shown for 0.1 lot size.

The chart screenshot is the same method on TradingView (Gold Spot / U.S. Dollar, 5-minute, OANDA): buy and sell entries, WIN labels, session shading, and the news table. Do not treat either image as audited performance.

## Telegram best-day reports

Positive example days only. Net PnL is for a **0.1 lot**. PnL shown for 0.1 lot size.

| Channel | Date | Win rate | Net PnL |
| --- | --- | --- | --- |
| 1M LeChiffre | 21/09/2026 | 65.5% (36 wins, 19 losses) | 414.08 |
| 3M LeChiffre | 18/09/2026 | 66.7% (10 wins, 5 losses) | 63.02 |
| 5M LeChiffre | 21/09/2026 | 66.7% (8 wins, 4 losses) | 143.03 |
| Fifteen+ LeChiffre | 21/09/2026 | 100% (4 wins, 0 losses) | 403.12 |

Images: `assets/telegram/`.

## Strategy Tester paper grid

TradingView Strategy Tester output for **LeChiffreXtelegram**, paper trading, **$10,000**. Windows are the last 7 days and the last 30 days. No 1-hour row, and no 5-minute 7-day screenshot in this set. The stronger 30-day runs are 1-minute, 3-minute, 5-minute, and 15-minute. Not an audited live brokerage account. PnL shown for 0.1 lot size.

| Timeframe | Last 7 days | Last 30 days |
| --- | --- | --- |
| 1-minute | +$2,168.61 (+21.69%), WR 61.64% (188/305), PF 1.834, DD 2.48% | +$6,292.17 (+62.92%), WR 60.93% (613/1006), PF 1.61, DD 3.55% |
| 3-minute | +$713.14 (+7.13%), WR 57.58% (57/99), PF 1.399, DD 4.09% | +$5,557.94 (+55.58%), WR 64.72% (233/360), PF 1.96, DD 2.84% |
| 5-minute | Not in this set | +$3,578.92 (+35.79%), WR 65.42% (140/214), PF 1.761, DD 3.24% |
| 15-minute | +$345.65 (+3.46%), WR 66.67% (14/21), PF 1.391, DD 4.15% | +$3,149.55 (+31.50%), WR 71.23% (52/73), PF 2.267, DD 2.77% |
| 30-minute | +$61.17 (+0.61%), WR 54.55% (6/11), PF 1.093, DD 5.63% | +$1,765.95 (+17.66%), WR 70.59% (24/34), PF 2.276, DD 4.84% |
| 4-hour | +$149.87 (+1.50%), DD 2.10%. Win rate and profit factor are not printed | +$1,478.75 (+14.79%), WR 75.00% (3/4), PF 3.349, DD 8.30% |

PnL shown for 0.1 lot size.

Screenshots: `assets/strategy/`.

## Preview locally

From the repository root:

```bash
python3 -m http.server 8080
```

Open [http://127.0.0.1:8080/](http://127.0.0.1:8080/). Paths are relative, so the same files work on GitHub project Pages (`/lechiffre-trading/`) without a build step.

## GitHub Pages

The site is plain HTML, CSS, and images at the repository root. [`.nojekyll`](.nojekyll) is present so GitHub Pages serves the files as-is.

Enable Pages from the repository root:

1. Repository **Settings → Pages**
2. **Build and deployment**: Deploy from a branch
3. Branch: **`main`**, folder: **`/ (root)`**
4. Save

After the first deploy finishes, the site is at:

**https://e-mination.github.io/lechiffre-trading/**

Do not add a `CNAME` for `lechiffre.online`. That domain already serves the method site. This repository is the portfolio on GitHub Pages.

## Repository layout

```
index.html          Portfolio
gallery.html        Screenshot gallery
css/styles.css      Styles
assets/             Chart, Strategy Tester grid, Telegram, favicon
assets/telegram/    Best-day channel summaries
assets/strategy/    Strategy Tester paper screenshots
LICENSE             MIT, for this site’s source
```

## Screenshots

| File | What it is |
| --- | --- |
| `assets/tradingview-indicator-xauusd.png` | LeChiffre Pine indicator on XAUUSD, 5-minute |
| `assets/strategy/` | Strategy Tester paper grid, 7-day and 30-day |
| `assets/strategy-30d-a.png` | Earlier crop of the 5-minute 30-day paper report |
| `assets/strategy-30d-b.png` | Earlier crop of the 15-minute 30-day paper report |
| `assets/telegram/` | Best-day summaries: 1M, 3M, 5M, Fifteen+ |
| `assets/telegram-5m-lechiffre.png` | 5M LeChiffre thread: pre-entry, entry, result, one daily summary |

The images are portfolio evidence of the author’s indicator and channel. They are not stock photos.

## License and contact

Source of this site (HTML, CSS, SVG) is released under the [MIT License](LICENSE).

**Elie Minassian** — [minassianelie@gmail.com](mailto:minassianelie@gmail.com) — [github.com/e-mination](https://github.com/e-mination)
