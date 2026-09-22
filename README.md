# LeChiffre — TradingView portfolio

Public portfolio for **Elie Minassian** ([e-mination](https://github.com/e-mination)): a rule-based **XAUUSD** method, a **Pine Script** indicator on TradingView, the **5M LeChiffre** Telegram channel, and the site [lechiffre.online](https://lechiffre.online/).

This repository is the static site. It is the author’s own work — the indicator, the channel, and the website — documented with screenshots. It is not a backtest archive and it is not financial advice.

## Links

| | |
| --- | --- |
| Method site | [https://lechiffre.online/](https://lechiffre.online/) |
| GitHub Pages | [https://e-mination.github.io/lechiffre-trading/](https://e-mination.github.io/lechiffre-trading/) |
| Author | Elie Minassian · [minassianelie@gmail.com](mailto:minassianelie@gmail.com) |
| GitHub | [github.com/e-mination](https://github.com/e-mination) |

The GitHub repository homepage is already set to [lechiffre.online](https://lechiffre.online/). The Pages URL above is this portfolio, published from the `main` branch root.

## What’s on the site

- **Hero** — LeChiffre as a rule-based XAUUSD method, with links to the product site, the Pine indicator, and the Telegram channel.
- **TradingView / Pine Script** — the XAUUSD 5-minute chart: entries, session shading (including London), a Forex Factory news table, and WIN tags.
- **Telegram** — example messages from **5M LeChiffre**: pre-entry, confirmed entry (entry / take profit / stop), the result, and the daily summary.
- **Website** — what [lechiffre.online](https://lechiffre.online/) is for.
- **Note** — not financial advice. Figures are one example day visible in the screenshots, not a multi-month audit.

A second page, [`gallery.html`](gallery.html), shows both screenshots larger.

## Example day in the screenshots

The Telegram screenshot is from **22 September 2026**. The daily summary card on that image reads:

- Asset **XAUUSD**, timeframe **5**
- **10** wins, **2** losses, **12** trades, **83.3%** win rate
- Net PnL **414.09**

One confirmed signal in the same thread:

- **BUY** XAUUSD (5), signal time **22/09/2026 06:30 GMT+3**, exit **06:40 GMT+3**
- Entry **4344.649**, take profit **4347.778**, stop **4341.520**, risk/reward **1**
- Result card: **TRADE WON**, realized PnL **31.29**

The chart screenshot is the same method on TradingView (Gold Spot / U.S. Dollar, 5-minute, OANDA): buy and sell entries, WIN labels, session shading, and the news table. Do not treat either image as audited performance.

## Preview locally

From the repository root:

```bash
python3 -m http.server 8080
```

Open [http://127.0.0.1:8080/](http://127.0.0.1:8080/). Paths are relative, so the same files work on GitHub project Pages (`/lechiffre-trading/`) without a build step.

## GitHub Pages

The site is plain HTML, CSS, and images at the repository root. [`.nojekyll`](.nojekyll) is present so GitHub Pages serves the files as-is.

Pages is configured to deploy from a branch:

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
assets/             Chart screenshot, Telegram screenshot, favicon
LICENSE             MIT, for this site’s source
```

## Screenshots

| File | What it is |
| --- | --- |
| `assets/tradingview-indicator-xauusd.png` | LeChiffre Pine indicator on XAUUSD, 5-minute |
| `assets/telegram-5m-lechiffre.png` | 5M LeChiffre channel: summary, pre-entry, entry, result |

The images are portfolio evidence of the author’s indicator and channel. They are not stock photos.

## License and contact

Source of this site (HTML, CSS, SVG) is released under the [MIT License](LICENSE).

**Elie Minassian** — [minassianelie@gmail.com](mailto:minassianelie@gmail.com) — [github.com/e-mination](https://github.com/e-mination)
