# Hadi Kianirad

**Python Backend & Automation Engineer** · Istanbul, Türkiye (GMT+3)

I build backend APIs, Telegram bots and automation tools for real business workflows: integrations with third-party APIs, multilingual user experiences, and running and maintaining applications in production.

**Focus:** Python · FastAPI · asyncio · Telegram Bots (aiogram) · API integrations · LLM automation

Open to **remote Python backend and automation roles**.

---

## Public code

- **[telbot](https://github.com/jjebraham/telbot)**: an async Telegram registration and KYC bot (aiogram 3). It has a 9-step FSM form, national-ID and card validation, identity matching through an external API, live exchange rates from several providers with fallback, and admin review. It comes with a pytest suite, CI and a mock mode so it runs locally.
- **[ai-support-bot](https://github.com/jjebraham/ai-support-bot)**: a Telegram support bot (aiogram 3) that answers questions from help articles with BM25 retrieval and the Claude API, and hands uncertain questions to a human admin chat. It has a reproducible eval (accuracy and escalation rate), a pytest suite with the LLM mocked, CI and a Dockerfile.
- **[orders-api](https://github.com/jjebraham/orders-api)**: an async FastAPI orders service for a fictional shop. Stock is reserved in one transaction with `SELECT ... FOR UPDATE`, orders take an idempotency key, and cancels release stock once. It runs on Postgres with Alembic migrations, a pytest suite that tests races for the last unit against a real database, and CI.
- **[kianirad.website](https://github.com/jjebraham/kianirad.website)**: a static site in English, Turkish and Persian (with RTL), built by Python i18n/SEO/sitemap scripts, with GitHub Actions and a small contact API.

## Production work (source code private)

**Kiani Exchange: Telegram bot, Mini App and admin panel**
- *Problem:* let customers register, pass KYC and get exchange quotes without leaving Telegram.
- *Built:* the registration and KYC flow, rate aggregation from several exchange APIs, a Telegram Mini App and a web admin panel, deployed behind Nginx and Supervisor.
- *Stack:* Python, aiogram, python-telegram-bot, FastAPI, SQLAlchemy, SQLite, Nginx, Supervisor.

**amooze.sh: automated science-Reel pipeline**
- *Problem:* publish short Persian science videos every day with little manual work.
- *Built:* an end-to-end pipeline. An LLM writes the script, a Persian pronunciation check runs (with owner-managed rules), Azure TTS voices it, the video is rendered, a human approves it in a Telegram bot, and it is published through the Instagram Graph API.
- *Stack:* Python, LLM APIs, Azure Speech, Instagram Graph API, systemd.

**[KriptoFarsi](https://kriptofarsi.com): Persian market-data platform**
- *Built:* a data pipeline that refreshes every five minutes, a public signal history that can be audited against its Telegram and X record, and a replay layer that rechecks the recorded lifecycle of each entry.

**[TRstudy bot](https://t.me/trstudy_bot)**: a Telegram bot that qualifies Persian-speaking students applying to Turkish universities.

## Tech

**Backend:** Python, FastAPI, asyncio, SQLAlchemy, Django, aiogram · **Data:** PostgreSQL, SQLite · **AI:** LLM APIs, prompt pipelines, AI code evaluation · **Ops:** Linux, Nginx, systemd/Supervisor, GitHub Actions, Cloudflare, GCP, DigitalOcean

## Contact

- Website: https://www.kianirad.website
- Email: kianirad2020@gmail.com
