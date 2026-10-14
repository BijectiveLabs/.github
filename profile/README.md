<p align="center">
  <a href="https://www.bijectivelabs.dev"><img src="https://raw.githubusercontent.com/BijectiveLabs/.github/main/profile/bijective_banner.png" alt="Bijective"></a>
</p>

<h3 align="center">The operating platform for crypto trading teams.</h3>

<p align="center"><em>You bring the strategy. We build everything it runs on.</em></p>

<p align="center">
  <a href="https://www.bijectivelabs.dev">Website</a> |
  <a href="https://www.bijectivelabs.dev/insights">Research</a> |
  <a href="https://www.bijectivelabs.dev/open-source">Open source</a> |
  <a href="https://docs.bijectivelabs.dev">Docs</a>
</p>

A trading team's edge is its strategy. Most of the work around it is not: risk limits, audit
evidence, monitoring, recovery, safe upgrades. That work takes months, and none of it finds alpha.

Bijective takes it off the team. It is a self-hosted platform that covers market data, execution,
portfolio control and an operator cockpit in one system, and runs on your own infrastructure.
Keys, strategies and data never leave it.

## The platform

| Part | What it does |
|---|---|
| Data engine | Market data from several venues, normalised into one consistent feed. A stream that goes quiet is flagged, not trusted. |
| Strategy engine | Where strategies are researched, tested and run: rules you write, or supervised AI agents that can only propose. |
| Control engine | Every order is checked against your limits before it reaches a venue. Risk never depends on execution. |
| Cockpit | Positions, orders, risk and health across venues, on one screen. |

One event record and one clock sit under all of it, so any moment can be reconstructed for audit
and any backtest replayed exactly.

## How it is built

- **It halts before it gambles with your capital.** When something is abnormal, the platform
  moves to a safe state instead of carrying on.
- **Silence is not health.** Every venue connection and data stream has an expected heartbeat.
  When it stops, that is an alarm.
- **Every order on record.** Every order and every refusal can be looked up and replayed later.
- **The real cost of a trade.** What execution cost against what was achievable, and a plain
  "not enough evidence" when the data cannot say.
- **Control stays with you.** The platform explains what it sees and recommends; it does not take
  execution authority you have not granted.

The platform is in active development, with early access by invitation. We commit to a design,
not an outcome: we reduce the risk within the platform's control and make failure survivable. We do
not claim to prevent every loss.

## Open source

[trading-research-agents](https://github.com/BijectiveLabs/trading-research-agents) is our
open-source package: autonomous trading agents for crypto, built on the same principle. Language
models propose a trade; fixed, tested rules compute the figures, size the position and decide
whether an order goes out. MIT license, [on PyPI](https://pypi.org/project/trading-research-agents/).
