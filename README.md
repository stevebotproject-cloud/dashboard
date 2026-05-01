# STEVE — Autonomous Trading System Dashboard

Live dashboard for the STEVE trading system, powered by reinforcement learning (PPO/DQN).

## Architecture

- **VPS (Hostinger)** — OpenClaw container running Python agents
- **API** — HTTP endpoint inside container serving `steve_status.json`
- **GitHub Actions** — Fetches data every 5 minutes and commits to repo
- **GitHub Pages** — Serves the static dashboard

## Workspaces

| Workspace | Market | Broker | Status |
|-----------|--------|--------|--------|
| Crypto BTC Live | BTC/USD | Aster DEX | LIVE |
| Stocks (Dow 20) | US Equities | Alpaca Paper | PAPER |
| Crypto BTC | BTC/USD | Alpaca Paper | PAPER |
| Crypto Multi (5) | BTC/ETH/AVAX/LINK/DOGE | Alpaca Paper | PAPER |

## Stack

Python 3.13 · Stable-Baselines3 · PPO/DQN · OpenClaw · React · Recharts
