# Manifold Markets Trading Bot

![Status](https://img.shields.io/badge/status-⚪_roadmap-555?style=flat-square)
[![Engine](https://img.shields.io/badge/engine-shared_core-6e40c9?style=flat-square)](https://github.com/tarpboi/Prediction-Markets-Trading-Bot-Toolkits)
[![Rust](https://img.shields.io/badge/rust-1.70+-orange.svg?style=flat-square&logo=rust)](https://www.rust-lang.org/)
[![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](LICENSE)
[![CI](https://github.com/tarpboi/Manifold-Markets/actions/workflows/ci.yml/badge.svg)](https://github.com/tarpboi/Manifold-Markets/actions/workflows/ci.yml)

> Automated **Manifold Markets trading bot** — Play-money. Part of the [Prediction Market Toolkits](https://github.com/tarpboi/Prediction-Markets-Trading-Bot-Toolkits) suite: one execution core, one risk layer, every venue.

**Manifold Markets** is **live in production today.**

> Backtest / research sandbox.

---

## Strategies on Manifold Markets

These bots run on Manifold Markets through a single venue adapter on the shared engine — same risk controls, same TUI, full dry-run support.

| Strategy |
|----------|
| 🎯 **Directional Arbitrage** — arb base (Up + Down < $1), tilted toward the side with more edge |

> Want a strategy not listed here on Manifold Markets? Adapter coverage is demand-driven — [ask](https://t.me/tarpboi).

---

## Quickstart

Clone, drop in your keys, and run — the TUI lets you pick a strategy.

```bash
git clone https://github.com/tarpboi/Manifold-Markets.git
cd Manifold-Markets
cp config.example.yaml config.yaml   # add your keys
cargo run --release                  # launch the TUI
# headless: cargo run --release -- run copy-trading
```

---

## One engine, every venue

This repo is the **Manifold Markets** entry point. The execution core, risk layer, and all 20+ venue adapters live in the main toolkit:

### 👉 **[Prediction-Markets-Trading-Bot-Toolkits](https://github.com/tarpboi/Prediction-Markets-Trading-Bot-Toolkits)** — the full suite

| | |
|---|---|
| **Order execution** | < 100ms end-to-end |
| **Event processing** | < 1ms per event |
| **Safety** | Circuit breaker · depth guard · dry-run · trade floor |
| **Venues** | 7 live today · 20+ venues |

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
