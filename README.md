# 🚗 AI-Powered Automated Automobile Career Scout Pipeline

A fully autonomous backend data pipeline that crawls core engineering job portals, parses raw HTML data, cleans unstructured text, evaluates listings against engineering profile constraints using LLMs, and pushes daily mobile alerts.

## 🛠️ System Architecture & Workflow Flow
`HTTP Scrapers (Portal Feeds)` ➔ `Text Parser (HTML-to-Text)` ➔ `Anthropic Claude (LLM Filter)` ➔ `Telegram Bot API (Mobile Push Notification)`

### Key Capabilities:
* **Background Scheduling:** Native automation configured to trigger autonomously every morning at 08:00 AM IST.
* **Data Sanitization:** Implemented a Text Parser layer reducing raw web crawl packet data overhead by 95% (shrinking 260K+ tokens down to <2K clean words) to optimize LLM performance constraints.
* **Context Filtering:** Customized prompt constraints instructing the AI engine to evaluate vacancies against B.Tech Automobile Engineering frameworks (Mechanical quotas, PSU eligibility, OEM parameters) while automatically suppressing unrelated fields (Civil, IT, Senior consultancies).

## 📁 Installation & Usage
1. Download the blueprint JSON configuration file from this repository.
2. Create a free account on Make.com and click **Import Blueprint** to replicate the pipeline layout instantly.
3. Connect your unique Telegram Bot API tokens and personal LLM credentials to activate the daily push channel.
