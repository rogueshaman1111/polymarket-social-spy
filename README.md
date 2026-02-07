

Copy-paste this full text into your README.md file on GitHub:markdown

# Polymarket Swarm - Social Spy Add-on

**Real-time social intelligence for smarter Polymarket trading.**

The Social Spy Add-on is a core module of the **Polymarket Swarm** — a powerful, AI-driven copy-trading platform that monitors Telegram, Discord, Reddit, and open news sources in real time to detect trading tips, whale alerts, big wallet activity, market sentiment, and high-confidence betting signals.

It uses advanced NLP (VADER sentiment analysis) + machine learning (Random Forest) to:
- Classify "whale posters" and high-signal accounts
- Score tip quality and relevance
- Generate actionable position ideas (e.g., "Buy YES on PSG win – strong whale sentiment")

All data is saved to `social_data.json` for seamless integration with the rest of the swarm (Time Travel Bot, Whale Tracker, Panic Detector, Main Copy Bot).

### Key Features
- Multi-platform monitoring: Telegram channels, Discord servers, Reddit subreddits, news feeds
- Keyword detection for trading terms (whale, big wallet, copy trade, insider tip, etc.)
- Real-time sentiment analysis on messages
- ML-based scoring of tip reliability and poster influence
- Dynamic channel discovery (via companion discovery bot)
- Structured JSON output for swarm integration
- Fully hosted & rentable as part of the Polymarket Swarm SaaS

### How It Powers the Swarm
- **Time Travel Bot**: Adjusts historical pattern win rates based on social sentiment trends
- **Whale Tracker Bot**: Validates tracked wallets with social mentions & hype
- **Panic Bot**: Boosts rebound probability when social chatter aligns
- **Main Copy Bot**: Increases conviction on HIGH signals with positive social confirmation

### Requirements
- Python 3.8+
- Libraries:
  ```bash
  pip install python-telegram-bot discord.py nltk scikit-learn requests feedparser

