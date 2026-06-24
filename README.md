# Myriad Markets Trading Bot

**🌐 Language / 语言 / Язык:** [English](README.md) · [简体中文](README.zh-CN.md) · [Русский](README.ru.md)

![Status](https://img.shields.io/badge/status-🟢_live-2ea44f?style=flat-square)
[![Engine](https://img.shields.io/badge/engine-shared_core-6e40c9?style=flat-square)](https://github.com/HarrierOnChain/Prediction-Markets-Trading-Bot-Toolkits)
[![Rust](https://img.shields.io/badge/rust-1.70+-orange.svg?style=flat-square&logo=rust)](https://www.rust-lang.org/)
[![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](LICENSE)
[![CI](https://github.com/HarrierOnChain/Myriad-Markets/actions/workflows/ci.yml/badge.svg)](https://github.com/HarrierOnChain/Myriad-Markets/actions/workflows/ci.yml)

> Automated **Myriad Markets trading bot** — Crypto. Part of the [Prediction Market Toolkits](https://github.com/HarrierOnChain/Prediction-Markets-Trading-Bot-Toolkits) suite: one execution core, one risk layer, every venue.

**Myriad Markets** is **live in production today.**

---

## Live on Myriad Markets

<div align="center">

<img width="820" alt="Myriad Markets trading bot TUI" src="https://github.com/user-attachments/assets/b6c51ba1-14c6-4582-858c-e9441516dd1d" />
<img width="820" alt="Myriad Markets trading bot TUI" src="https://github.com/user-attachments/assets/66d9cb72-e14a-414f-93e5-600fb1d3f49f" />

<sub>The shared TUI running against Myriad Markets — live positions, P&L, and circuit-breaker state. <!-- TODO: swap in Myriad Markets-specific captures --></sub>

</div>

---

## Strategies on Myriad Markets

These bots run on Myriad Markets through a single venue adapter on the shared engine — same risk controls, same TUI, full dry-run support.

| Strategy |
|----------|
| 📊 **Orderbook Imbalance** — the signal *is* the order book, no external feeds |
| 🎯 **Directional Arbitrage** — arb base (Up + Down < $1), tilted toward the side with more edge |

> Want a strategy not listed here on Myriad Markets? Adapter coverage is demand-driven — [ask](https://t.me/HarrierOnChain).

---

## Quickstart

Clone, drop in your keys, and run — the TUI lets you pick a strategy.

```bash
git clone https://github.com/HarrierOnChain/Myriad-Markets.git
cd Myriad-Markets
cp config.example.yaml config.yaml   # add your keys
cargo run --release                  # launch the TUI
# headless: cargo run --release -- run copy-trading
```

---

## One engine, every venue

This repo is the **Myriad Markets** entry point. The execution core, risk layer, and all 20+ venue adapters live in the main toolkit:

### 👉 **[Prediction-Markets-Trading-Bot-Toolkits](https://github.com/HarrierOnChain/Prediction-Markets-Trading-Bot-Toolkits)** — the full suite

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
| **Full toolkit** | [Prediction-Markets-Trading-Bot-Toolkits](https://github.com/HarrierOnChain/Prediction-Markets-Trading-Bot-Toolkits) |
| **Telegram** | [@HarrierOnChain](https://t.me/HarrierOnChain) |
| **Discussions** | [GitHub Discussions](https://github.com/HarrierOnChain/Prediction-Markets-Trading-Bot-Toolkits/discussions) |

*Response time is typically within a few hours.*

---

## Related venues

[Kalshi](https://github.com/HarrierOnChain/Kalshi) · [Polymarket](https://github.com/HarrierOnChain/Polymarket) · [Augur](https://github.com/HarrierOnChain/Augur) · [Azuro](https://github.com/HarrierOnChain/Azuro)

> Browse the full venue directory in the [main toolkit →](https://github.com/HarrierOnChain/Prediction-Markets-Trading-Bot-Toolkits#venue-coverage)

---

## Disclaimer

> Trading prediction markets involves real financial risk. This software is provided as-is, without warranty. It is not financial advice. Always test with `enable_trading: false` before deploying real capital. Ensure compliance with Myriad Markets's terms of service and your local regulations.

---

<div align="center">

**Myriad Markets trading bot · built on the [Prediction Market Toolkits](https://github.com/HarrierOnChain/Prediction-Markets-Trading-Bot-Toolkits) engine**

[![Telegram](https://img.shields.io/badge/Telegram-@HarrierOnChain-26A5E4?style=flat-square&logo=telegram)](https://t.me/HarrierOnChain)

</div>
