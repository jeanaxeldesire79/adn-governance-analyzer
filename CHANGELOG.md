# Changelog — ADN Governance Analyzer

All notable changes to the ADN Governance Analyzer will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/), and this project adheres to [Semantic Versioning](https://semver.org/).

## [2.0.1] — 2026-05-24

### Changed
- Production release with live data integration
- Updated analysis database with latest governance statements
- Enhanced sentiment visualization with improved color coding
- Optimized French-language interface for local stakeholders
- Improved mobile layout for field access

## [1.0.0] — 2026-05-23

### Added
- Initial release of the ADN Governance Analyzer for Côte d'Ivoire 2024
- 113-statement policy speech analysis database
- Theme-based filtering and classification (12 governance themes)
- Speaker timeline with chronological statement browsing
- Sentiment analysis visualization (positive/neutral/negative)
- Keyword and topic search across all statements
- Governance dimension classification
- Policy implications view for each statement
- Key quote extraction display
- French-language interface support
- Responsive dark theme design

### Technical
- Single-file French-language HTML application
- Vanilla JavaScript with async API calls
- Data from `political_economy.adn_statements` (113 manually analyzed statements)
- API: `/api/data/adn/*` endpoints
- Backend: Python FastAPI → PostgreSQL (datasci_db)
