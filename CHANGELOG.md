# LeChiffre — release notes

Product changes for the Android app, the web app, the signal server (Cloudflare Worker), and the Telegram bot.
Source code, server addresses, keys, and member data are not in this repository. Every P/L figure is for a **0.1 lot**.

## 10 October 2026

### Telegram bot — worker 1.12.1 → 1.12.3
- **Pair picker.** First visit: **XAUUSD · Gold** and **BTCUSD · Bitcoin** (an “Other pairs” button appears only once other pairs are switched on).
- After a pick, the pair menu: Signals · Results · price · USD news · Open app · Change pair · language.
- **1.12.2:** one **🔁 Change pair → <next>** button on every menu cycles XAUUSD → BTCUSD → XAUUSD. The choice is saved per chat and the menu is edited in place.
- **1.12.3:** once a pair is known, the main menu shows only the Change pair button.
- Signals: the public feed for that pair, with the members-only signals of the delay window counted as locked. Results: daily results for that pair. Price: TradingView, with a fallback source. BTCUSD is marked “open 24/7”.
- Commands: `/pair`, `/xauusd`, `/btcusd`, `/gold`, `/btc`. `/results`, `/signals`, `/price`, `/news` follow the last pair.
- The bot menu is served by the Cloudflare Worker (Telegram webhook).

### App 1.0.23 · web 1.0.23-web
- No more pair tab bar. The pair in the Signals and Results heading is the switcher: **‹ XAUUSD ›**. Arrows or a tap on the name switch XAUUSD ↔ BTCUSD.
- **Notify me** shows one pair’s grid at a time with the same switcher. Same rows (1M … 4H, 1H included, Other), same switches, same news toggles.
- Screens: [`assets/app-v1.0.23/`](assets/app-v1.0.23/).

### App 1.0.22 · web 1.0.22-web · worker 1.12.0 — two pairs
- **XAUUSD and BTCUSD** live. Feed, running trades, Today, Performance, history, Results, live price, and the TradingView / MT5 buttons all follow the selected pair.
- **1H** timeframe tab: All, 1M, 3M, 5M, 15M, 30M, 1H, 4H on Signals, Results, and Notify me.
- **Performance** table: **Today** · Week · Month · All history. Today = since 00:00 on the member’s device, per pair.
- **Notify me**: one grid per pair, Pre-entry · Signal · Result for each timeframe. BTCUSD alerts start once the member opens Notify me on 1.0.22 or later. Older apps keep their XAUUSD alerts as before.
- Notification titles carry the pair: “Preentry on BTCUSD 1 min TF”, “Buy XAUUSD 5 min TF”, “Result Win BTCUSD 15 min TF”.
- Away summary grouped by pair.
- BTCUSD P/L on a 0.1 lot = 0.1 BTC.

### App 1.0.21 · worker 1.11.0
- Enabling notifications now checks that banners really show, with step-by-step help for Windows, Mac, Android, and iPhone.
- **Away summary:** with the app in the background, the tab hidden, or logged out, one summary on return instead of every alert.
- iPhone: in-app guide to add LeChiffre to the Home Screen and allow its notifications.

### Worker 1.10.11
- 1-minute history kept in full, like every other timeframe. 1M daily summaries from 30 July to 10 September 2026 restored from the Telegram channel export.

### App 1.0.20 · worker 1.10.10
- **Notify me grid:** for each timeframe, three switches, Pre-entry · Signal · Result. Tap a timeframe or a column title to switch a whole row or column. News 30 min / 5 min before under the grid.
- Notification titles always name the timeframe.
- Web watermark: member’s name and code, members only.

Past performance does not guarantee future results. This is not financial advice.
