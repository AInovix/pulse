# PULSE - Global Intelligence Monitor

![PULSE Banner](https://img.shields.io/badge/PULSE-Global%20Intelligence%20Monitor-00ff88?style=for-the-badge&labelColor=0a0e12)
![License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)
![Status](https://img.shields.io/badge/Status-Live-00ff88?style=flat-square)
![DEFCON](https://img.shields.io/badge/DEFCON-3%20(OSINT%20EST.)-ff9500?style=flat-square)

A real-time global situation awareness dashboard inspired by defense intelligence platforms like Anduril and Palantir. PULSE aggregates open-source intelligence (OSINT) to provide comprehensive monitoring of global events, conflicts, and geopolitical developments.

## 📡 Real-Time Data Sources

PULSE fetches live data from these free APIs (no keys required):

| Source | Data | Refresh Rate |
|--------|------|--------------|
| **Polymarket API** | Prediction market odds | 30 seconds |
| **BBC World RSS** | World news headlines | 2 minutes |
| **Al Jazeera RSS** | International news | 2 minutes |
| **RSS2JSON** | RSS feed conversion | As needed |

All APIs are CORS-friendly and work directly in the browser without a backend.

## 🌍 Live Demo

Deploy your own instance or view the demo at your Netlify URL.

## ✨ Features

### 🗺️ Global Situation Map
- Interactive world map with threat zone markers
- Color-coded threat levels (Critical, Elevated, Watch, Monitor, Intel)
- Click markers for detailed intelligence briefs and Polymarket odds
- Real-time tracking overlay with military-style HUD

### 📊 Intelligence Feeds
- **OSINT Feed**: Real-time open-source intelligence updates
- **World/Geopolitical**: Global news and developments
- **Government/Policy**: Policy changes and official statements
- **Technology/AI**: Tech sector intelligence

### 📈 Prediction Markets
- Live Polymarket odds on geopolitical events
- Visual probability indicators
- Volume and trend data
- Categories: Conflicts, Iran, Asia, US Politics, Markets

### 💹 Market Data
- Real-time financial market indicators
- S&P 500, NASDAQ, VIX, Gold, Oil, BTC
- Trend direction and percentage changes

### 🔴 DEFCON Status
- Current estimated DEFCON level (OSINT-based)
- Threat index calculation
- Regional command status
- Historical context

### 🐦 X/Twitter OSINT Integration
- Curated list of OSINT accounts
- Live search feed links
- Real-time social intelligence

## 🚀 Deployment

### Netlify (Recommended)

1. Fork this repository
2. Connect to Netlify
3. Deploy with default settings (no build command needed)

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start)

### GitHub Pages

1. Fork this repository
2. Go to Settings > Pages
3. Select "Deploy from a branch"
4. Choose `main` branch and `/ (root)` folder

### Local Development

```bash
# Clone the repository
git clone https://github.com/yourusername/pulse-monitor.git

# Navigate to directory
cd pulse-monitor

# Open in browser (no build required)
open index.html

# Or use a local server
npx serve .
```

## 🛠️ Technology Stack

- **Frontend**: React 18 (via CDN)
- **Styling**: Tailwind CSS (via CDN)
- **Mapping**: Leaflet.js
- **Fonts**: JetBrains Mono, Space Grotesk, IBM Plex Mono
- **No backend required** - Static HTML deployment

## 📡 Data Sources

All data is sourced from open-source intelligence:

- [DEFCON Level](https://defconlevel.com) - OSINT DEFCON estimates
- [Polymarket](https://polymarket.com) - Prediction market data
- [ISW](https://understandingwar.org) - Institute for the Study of War
- News agencies: Al Jazeera, Reuters, BBC, CNN
- Government sources: State Dept, Pentagon, NATO
- OSINT Twitter/X accounts

## ⚠️ Disclaimer

**UNCLASSIFIED // OSINT**

- DEFCON levels shown are **OSINT estimates**, not official classifications
- Official DEFCON status is classified by the US government
- This tool is for **educational and informational purposes only**
- Data accuracy depends on source reliability
- Not affiliated with any government or military organization

## 🎨 Design Philosophy

PULSE is designed with a military command center aesthetic:

- **Dark theme** with tactical green accents
- **Monospace typography** for data clarity
- **Grid overlays** and scan lines for atmosphere
- **Minimal animations** that don't distract
- **Information density** balanced with readability

## 📋 Roadmap

- [ ] Live API integrations (NewsAPI, financial data)
- [ ] WebSocket real-time updates
- [ ] Aircraft/ship tracking (OpenSky, MarineTraffic)
- [ ] Customizable alert thresholds
- [ ] Mobile-responsive improvements
- [ ] Dark/light theme toggle
- [ ] Export/share functionality
- [ ] Push notifications for critical alerts

## 🔧 Configuration

Edit the `CONFIG` object in `index.html`:

```javascript
const CONFIG = {
    DEFCON_LEVEL: 3,           // Current estimated DEFCON
    UPDATE_INTERVAL: 30000,    // Data refresh rate (ms)
    NEWS_UPDATE_INTERVAL: 60000,
};
```

## 🤝 Contributing

Contributions are welcome! Please read our contributing guidelines before submitting PRs.

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by defense intelligence platforms
- OSINT community for data aggregation methodologies
- Open-source mapping libraries
- Prediction market platforms for probability data

---

**Built with ☕ and vigilance**

*"In God we trust. All others we monitor."*
