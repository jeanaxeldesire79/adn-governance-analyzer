# 📜 ADN Governance Analyzer

[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![HTML](https://img.shields.io/badge/HTML-5-orange)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS-3-blueviolet)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Status](https://img.shields.io/badge/status-BETA-yellow)]()

> Analyse des discours politiques de Côte d'Ivoire — 113 déclarations à travers 12 thèmes de gouvernance. Moteur d'analyse des politiques publiques pour l'ADN (Agence Nationale de Développement).

**Part of the [Axel Dev Group (ADG)](https://axeldevlab.com) portal ecosystem.**

---

## 🚀 Live Demo

Visit **[portal.axeldevlab.com](https://portal.axeldevlab.com)** → Navigate to **ADN Governance Analyzer**

> ⚠️ Portal access requires login credentials. Contact the ADG team for access.

![ADN Governance Analyzer Screenshot](docs/screenshot.png)

---

## ✨ Features

- 🎤 **113 Policy Statements** — Hand-analyzed governance statements from 14 speakers
- 🏷️ **12 Governance Themes** — Corruption, education, security, economy, health, and more
- 📅 **Timeline View** — Chronological browsing of all statements by date
- 📊 **Sentiment Analysis** — Positive/negative/neutral classification with color coding
- 🔍 **Keyword Search** — Full-text search across all statements
- 👥 **Speaker Filter** — Filter by government official or institution
- 📖 **Key Quote Extraction** — Notable quotes highlighted for each statement
- 🇫🇷 **French Language** — Full interface in French for local stakeholders
- 🌙 **Dark Theme** — Optimized for dashboard monitoring

---

## 🏗️ Architecture

```
┌──────────────┐     ┌──────────────────────┐     ┌──────────────────┐
│   Browser    │────▶│   Portal API         │────▶│   PostgreSQL     │
│  (Vanilla    │     │   (Python FastAPI)   │     │   (datasci_db)   │
│   HTML/CSS/  │◀────│                      │◀────│                  │
│   JS)        │     │  /api/data/adn/*     │     │  political_      │
│              │     │                      │     │  economy.        │
└──────────────┘     └──────────────────────┘     │  adn_statements  │
                                                   └──────────────────┘
```

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|------------|
| **Frontend** | Vanilla HTML5, CSS3 (custom properties), JavaScript (ES6+) |
| **Icons** | Font Awesome (via CDN) |
| **Charts** | Chart.js (via CDN) |
| **Backend** | Python FastAPI |
| **Database** | PostgreSQL 15 (`datasci_db`) |
| **Analysis** | Manual expert analysis (113 statements) |
| **Deployment** | Portal module viewer on `portal.axeldevlab.com` |

---

## Analysis Methodology

Each statement is analyzed across three dimensions:

1. **Governance Theme** — Classified into 1 of 12 governance categories
2. **Sentiment** — Manually rated as positive, negative, or neutral
3. **Policy Implications** — Assessment of real-world policy impact

---

## 📁 Repository Structure

```
adn-governance-analyzer/
├── README.md               # This file (Français)
├── LICENSE                 # MIT License
├── CHANGELOG.md            # Version history
├── CONTRIBUTING.md         # How to contribute
├── src/
│   └── index.html          # Single-file app (production HTML)
├── docs/
│   └── screenshot.png      # App screenshot
├── data/
│   └── schema.md           # Database schema reference
├── scripts/
│   └── deploy.sh           # Deployment script
└── .github/
    └── workflows/          # GitHub Actions (future)
```

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
