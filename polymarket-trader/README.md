# 📊 Polymarket Trader Tracker

**Real-time alerts when top Polymarket traders place bets**

Track whale wallets, get instant notifications (desktop + Discord + sound), and never miss a trade signal.

🔗 **[LIVE DEMO →](https://yourusername.github.io/polymarket-tracker/notifications.html)**

![Demo](https://img.shields.io/badge/status-live-success) ![No Dependencies](https://img.shields.io/badge/dependencies-none-blue) ![License](https://img.shields.io/badge/license-MIT-green)

---

## ✨ Features

- 🎯 **Track Multiple Traders** - Build a portfolio of proven Polymarket wallets
- 🔔 **Multi-Channel Alerts** - Desktop notifications, sound alerts, Discord webhooks
- 🎨 **Futuristic UI** - Cyberpunk dashboard with glass morphism and neon accents
- 📊 **Live Stats** - Track alerts, volume, and trader activity in real-time
- 🔒 **100% Private** - All data stored locally in your browser, no server required
- ⚡ **Smart Filtering** - Filter by bet size, side (BUY/SELL), and more
- 📥 **Export Data** - Download alerts as JSON or CSV for analysis
- 🎭 **Demo Mode** - Test with fake alerts before tracking real traders

---

## 🚀 Quick Start

### Option 1: Use Live Version
1. Go to the [Live Demo](https://yourusername.github.io/polymarket-tracker/notifications.html)
2. Click "Enable Notifications"
3. Add a trader wallet address
4. Click "Start Monitoring"

### Option 2: Run Locally
1. Download `notifications.html`
2. Double-click to open in browser
3. OR run local server: `python -m http.server 8000`
4. Open `http://localhost:8000/notifications.html`

---

## 📖 How It Works

The app polls Polymarket's public API every 30-60 seconds to check for new trades from wallets in your portfolio. When a tracked trader places a bet:

1. ✅ Desktop notification pops up
2. 🔊 Sound alert plays (optional)
3. 💬 Discord message sent (optional)
4. 📋 Alert logged in-app

All without any server - everything runs in your browser!

---

## 🎯 Finding Wallets to Track

**Method 1: High-Volume Markets**
- Go to [polymarket.com](https://polymarket.com)
- Browse top markets
- Look at order books for large positions
- Copy wallet addresses

**Method 2: Polygonscan**
- Visit [polygonscan.com](https://polygonscan.com)
- Search Polymarket contracts
- Find active trading wallets

**Method 3: Community**
- Ask in Polymarket Discord
- Follow crypto Twitter for known traders
- Share discoveries with friends

---

## ⚙️ Configuration

### Check Interval
- **30 seconds**: Aggressive (catch every trade fast)
- **1 minute**: Balanced (recommended)
- **5-10 minutes**: Relaxed (lower API usage)

### Filters
- **Minimum Bet Size**: Only alert for bets above X USDC
- **Side Filter**: Track only BUY, only SELL, or both
- **Sound Alerts**: Enable/disable beep on new trades

### Discord Integration
1. Create webhook in Discord (Server Settings → Integrations)
2. Paste webhook URL into app
3. Get mobile notifications via Discord app!

---

## 💡 Use Cases

### 📈 Copy Trading
Track 5-10 proven traders with 60%+ win rates, set minimum bet to $500+, get instant alerts, and copy their positions.

### 🔬 Research
Track 20+ diverse traders, export data weekly, analyze patterns in successful predictions.

### 🎓 Learning
Study timing, sizing, and market selection from top performers across different categories.

---

## 🛠️ Technical Details

- **Single File**: Pure HTML/CSS/JavaScript, no build tools
- **No Dependencies**: Works offline, no frameworks
- **localStorage**: All data saved in browser (privacy-first)
- **API**: Uses Polymarket's public `/activity` endpoint
- **Smart First-Run**: Doesn't spam alerts for historical trades

---

## 📱 Screenshots

### Main Dashboard
![Dashboard](https://via.placeholder.com/800x500?text=Futuristic+Cyber+Dashboard)

### Live Alerts
![Alerts](https://via.placeholder.com/800x500?text=Real-time+Trade+Alerts)

### Portfolio Management
![Portfolio](https://via.placeholder.com/800x500?text=Trader+Portfolio)

---

## 🐛 Troubleshooting

### Notifications Not Working?
- Click "Enable Notifications" and allow permission
- Check browser notification settings
- Some browsers block notifications on `file://` - use web server or GitHub Pages

### CORS Errors?
- Don't open HTML directly (`file://` protocol)
- Use: `python -m http.server 8000` 
- Or deploy to GitHub Pages (works perfectly)

### API Errors?
- Check internet connection
- Polymarket API might be temporarily down
- Try again in a few minutes

**[Full Troubleshooting Guide →](GUIDE.md)**

---

## 📚 Documentation

- **[Complete Guide](GUIDE.md)** - Setup, usage, and advanced features
- **[API Reference](https://docs.polymarket.com)** - Polymarket API documentation

---

## 🤝 Contributing

Found a bug? Have a feature idea? PRs welcome!

1. Fork the repo
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

MIT License - feel free to use, modify, and distribute!

---

## ⭐ Star This Repo

If you find this useful, give it a star! It helps others discover the project.

---

## 🔗 Links

- [Live Demo](https://yourusername.github.io/polymarket-tracker/notifications.html)
- [Polymarket](https://polymarket.com)
- [Report Bug](https://github.com/yourusername/polymarket-tracker/issues)
- [Request Feature](https://github.com/yourusername/polymarket-tracker/issues)

---

## 💰 Support Development

Built with ❤️ for the Polymarket community

If this saves you time or helps you make better trades, consider:
- ⭐ Starring the repo
- 🐛 Reporting bugs
- 💡 Suggesting features
- 📢 Sharing with friends

---

**Disclaimer**: This tool is for informational purposes only. Not financial advice. Always do your own research before making trades.

**Made by traders, for traders** 🚀
