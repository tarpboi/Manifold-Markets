# Manifold Markets Trading Bot

[![Engine](https://img.shields.io/badge/engine-shared_core-6e40c9?style=flat-square)](https://github.com/tarpboi/Prediction-Markets-Trading-Bot-Toolkits)
[![Rust](https://img.shields.io/badge/rust-1.70+-orange.svg?style=flat-square&logo=rust)](https://www.rust-lang.org/)
[![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](LICENSE)
[![CI](https://github.com/tarpboi/Manifold-Markets/actions/workflows/ci.yml/badge.svg)](https://github.com/tarpboi/Manifold-Markets/actions/workflows/ci.yml)

> **Manifold Markets trading bot** — Play-money. Part of the [Prediction Market Toolkits](https://github.com/tarpboi/Prediction-Markets-Trading-Bot-Toolkits) suite: one execution core, one risk layer, every venue.

**Manifold Markets** is mapped to the shared engine, but its adapter isn't wired yet. This repo holds venue metadata; the trading code lives in the main toolkit, which executes on Polymarket today.

> Backtest / research sandbox.

---

## Strategies on Manifold Markets

These are the strategies mapped to Manifold Markets. They run here once its adapter is wired — same risk controls, same TUI, full dry-run support.

| Strategy |
|----------|
| 🎯 **Directional Arbitrage** — arb base (Up + Down < $1), tilted toward the side with more edge |

> Want a strategy not listed here on Manifold Markets? Adapter coverage is demand-driven — [ask](https://t.me/tarpboi).

---

## Quickstart

The trading code lives in the main toolkit. Clone it, add your keys, and start in dry-run. It runs against Polymarket today.

```bash
git clone https://github.com/tarpboi/Prediction-Markets-Trading-Bot-Toolkits.git
cd Prediction-Markets-Trading-Bot-Toolkits
cp config.yaml.example config.yaml        # add your keys
cargo run --release -- run copy-trading   # dry-run: enable_trading is false by default
```

---

## One engine, every venue

The execution core and risk layer live in the main toolkit:

### 👉 **[Prediction-Markets-Trading-Bot-Toolkits](https://github.com/tarpboi/Prediction-Markets-Trading-Bot-Toolkits)** — the full suite

| | |
|---|---|
| **Order execution** | < 100ms end-to-end |
| **Event processing** | < 1ms per event |
| **Safety** | Circuit breaker · depth guard · dry-run · trade floor |
| **Venues** | 21 venues mapped |

Adding a venue means writing **one adapter** — not rebuilding a bot.

---

## Get access

| Platform | Link |
|----------|------|
| **Full toolkit** | [Prediction-Markets-Trading-Bot-Toolkits](https://github.com/tarpboi/Prediction-Markets-Trading-Bot-Toolkits) |
| **Telegram** | [@tarpboi](https://t.me/tarpboi) |
| **Discussions** | [GitHub Discussions](https://github.com/tarpboi/Prediction-Markets-Trading-Bot-Toolkits/discussions) |

*Response time is typically within a few hours.*

---

## Related venues

[Crypto.com Predictions](https://github.com/tarpboi/Crypto.com-Predictions) · [Hedgehog Markets](https://github.com/tarpboi/Hedgehog-Markets) · [Kalshi](https://github.com/tarpboi/Kalshi) · [Myriad Markets](https://github.com/tarpboi/Myriad-Markets)

> Browse the full venue directory in the [main toolkit →](https://github.com/tarpboi/Prediction-Markets-Trading-Bot-Toolkits#venue-coverage)

---

## Disclaimer

> Trading prediction markets involves real financial risk. This software is provided as-is, without warranty. It is not financial advice. Always test with `enable_trading: false` before deploying real capital. Ensure compliance with Manifold Markets's terms of service and your local regulations.

---

<div align="center">

**Manifold Markets trading bot · built on the [Prediction Market Toolkits](https://github.com/tarpboi/Prediction-Markets-Trading-Bot-Toolkits) engine**

[![Telegram](https://img.shields.io/badge/Telegram-@tarpboi-26A5E4?style=flat-square&logo=telegram)](https://t.me/tarpboi)

</div>
