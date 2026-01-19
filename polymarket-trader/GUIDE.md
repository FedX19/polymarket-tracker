# 📊 Polymarket Trader Tracker - Complete Guide

## ✅ How to Use (5 Steps)

1. **Open the File**
   - Double-click `notifications.html`
   - Opens in your default browser
   - Works on Mac, Windows, Linux

2. **Enable Notifications**
   - Click "Enable Now" button in yellow banner
   - Browser will ask permission → Click "Allow"
   - You'll see a test notification confirming it works

3. **Add Traders to Portfolio**
   - Paste wallet address (starts with 0x...)
   - Give it a label (e.g., "Whale #1")
   - Click "Add Trader"
   - Repeat for all traders you want to track

4. **Configure Settings** (Optional)
   - **Check Interval**: How often to check (30 sec to 10 min)
   - **Minimum Bet**: Only alert for bets above this amount
   - **Sound Alerts**: Enable/disable beep sound
   - **Discord Webhook**: Get phone notifications via Discord

5. **Start Monitoring**
   - Click green "Start Monitoring" button
   - Status changes to "LIVE" with pulsing dot
   - Leave browser tab open (can minimize)
   - You'll get alerts when tracked traders bet!

---

## 🎯 Finding Wallets to Track

### Method 1: High-Volume Markets
1. Go to polymarket.com
2. Browse top markets
3. Click on a popular market
4. Look at large positions in order book
5. Copy wallet addresses from big traders

### Method 2: Use Polygonscan
1. Go to polygonscan.com
2. Search for Polymarket contracts
3. View recent transactions
4. Find active trading wallets

### Method 3: Community Sources
- Polymarket Discord
- Crypto Twitter
- Ask for known successful traders

---

## ⚠️ Troubleshooting

### Notifications Not Working

**Desktop notifications not showing?**
- Check browser notification settings
- Make sure you clicked "Enable Now"
- Permissions must be "Allow" not "Block"
- Some browsers block notifications in incognito mode
- Keep the browser tab open (can be minimized)

**How to fix blocked notifications:**
- Chrome: Settings → Privacy and Security → Site Settings → Notifications
- Firefox: Preferences → Privacy & Security → Permissions → Notifications
- Safari: Preferences → Websites → Notifications
- Find `notifications.html` and set to "Allow"

**File:// protocol issues:**
- Some browsers restrict notifications on local files
- **Fix**: Run a local server instead:
  ```bash
  python -m http.server 8000
  ```
  Then open `http://localhost:8000/notifications.html`

### Sound Not Playing

**No beep when testing?**
- Click "Test Sound" button first (initializes audio)
- Check sound settings are "Enabled"
- Volume must be up
- Some browsers require user interaction before playing audio
- Try clicking anywhere on page, then test again

### Discord Webhook Not Working

**Messages not appearing in Discord?**
- Verify webhook URL is complete and correct
- Check Discord channel still exists
- Make sure webhook wasn't deleted
- Click "Test Discord" to verify
- Check for typos in URL

**Getting webhook URL:**
1. Discord → Server Settings → Integrations
2. Webhooks → New Webhook
3. Name it "Polymarket Alerts"
4. Select channel
5. Copy webhook URL
6. Paste into app

### No Alerts Showing

**Not seeing any alerts?**
- Verify wallets are actually trading
  - Check on polymarket.com
  - Make sure they're active
- Lower minimum bet size to $0 temporarily
- Click "Check Now" to force immediate check
- Enable "Demo Mode" to test with fake alerts
- Check that monitoring is actually started (green "LIVE" status)

### App Errors / Crashes

**localStorage quota exceeded:**
- Click "Clear Log" to free space
- Lower "Alert Log Limit" to 200
- Export data before clearing

**API errors showing:**
- Polymarket API might be down (rare)
- Check internet connection
- Try again in a few minutes
- Error count shows in stats

**State corrupted:**
- Open browser console (F12)
- Type: `localStorage.removeItem('polymarket_tracker_state')`
- Press Enter
- Refresh page - starts fresh

### Performance Issues

**Browser slowing down?**
- Increase check interval to 5-10 minutes
- Reduce number of tracked wallets to <10
- Clear alert log regularly
- Lower log limit to 100

---

## 🚀 Advanced Features

### Demo Mode
- Click "Enable Demo"
- Generates fake alerts every check
- Perfect for testing notifications
- No API calls made
- Turn off when ready for real tracking

### Export Data
- **JSON**: Full alert data for analysis
- **CSV**: Import into Excel/Google Sheets
- Use for backtesting strategies
- Track historical performance

### Side Filtering
- **Both**: See all BUY and SELL
- **Only Buy**: Only BUY signals
- **Only Sell**: Only SELL signals
- Great for specific strategies

---

## 💡 Pro Tips

### For Best Results

**Tracking Strategy:**
- Start with 3-5 proven traders
- Focus on one category (Politics, Crypto, etc.)
- Track their wins with the analyzer first
- Only track traders with 60%+ win rate

**Notification Settings:**
- Use 30-second interval for active trading
- Set minimum bet to $100+ to reduce noise
- Enable Discord for mobile alerts
- Keep sound on during trading hours

**Portfolio Management:**
- Label traders clearly ("Politics Expert", "Whale #3")
- Copy full addresses for reference
- Edit labels as you learn their edges
- Remove inactive traders monthly

### Common Use Cases

**Copy Trading:**
```
1. Track 5-10 proven traders
2. Set min bet to $500+ (serious money only)
3. Check interval: 30 seconds
4. Discord webhook for instant mobile alerts
5. When alert fires → check market → copy trade
```

**Research:**
```
1. Track 20+ diverse traders
2. No minimum bet (see everything)
3. Check interval: 1-5 minutes
4. Export data weekly for analysis
5. Find patterns in successful bets
```

**Learning:**
```
1. Track top 3 traders per category
2. Min bet $100
3. Study their timing and sizing
4. Note when they bet early vs late
5. Learn market selection
```

---

## 🔒 Privacy & Security

**Data Storage:**
- Everything stored in browser localStorage
- No server, no cloud, no tracking
- Your data never leaves your computer
- Clear browser data = clear tracking history

**API Calls:**
- Only to Polymarket's public API
- No authentication required
- No API keys stored
- All blockchain data is public anyway

**Discord Webhook:**
- Optional - you control it
- Only you can see messages
- Delete webhook anytime in Discord
- URL stored locally only

---

## 🛠️ Future Upgrades Ideas

**Planned features you could add:**
- Telegram bot integration
- SMS alerts via Twilio
- Email notifications
- Portfolio grouping (whales, experts, etc.)
- Win rate tracking per trader
- Bet size trend analysis
- Category-specific alerts
- Market price tracking
- Profit/loss calculator
- Historical charts
- Mobile app version
- Server version with database
- WebSocket real-time updates
- Multi-user sharing
- Public leaderboards

---

## 📱 Running 24/7

**Desktop Computer:**
- Keep browser tab open always
- Set computer to never sleep
- Use dedicated browser profile
- Consider old laptop as dedicated monitor

**Cloud Server (Advanced):**
- Deploy to AWS/Digital Ocean
- Run headless Chrome
- Set up cron job
- Forward alerts to phone
- Never miss a trade

**Raspberry Pi:**
- $35 dedicated device
- Runs 24/7
- Low power consumption
- Perfect for always-on monitoring

---

## ❓ FAQ

**Q: Do I need a Polymarket account?**
A: No! This just tracks traders. No account needed.

**Q: Does this cost money?**
A: Completely free. Uses free public API.

**Q: Can I track my own wallet?**
A: Yes! Add your own address to track your trades.

**Q: How many traders can I track?**
A: Unlimited, but 5-20 is optimal for performance.

**Q: Will this drain my battery?**
A: Minimal impact. Uses ~1-2% CPU when monitoring.

**Q: Can I use on mobile?**
A: Yes! Works on mobile Safari/Chrome. Enable notifications.

**Q: What if a trader deletes their wallet?**
A: Rare. Just remove them and add a new one.

**Q: Can I share my portfolio with friends?**
A: Not directly, but share the file - they can add same wallets.

**Q: Does first run alert for all past trades?**
A: No! Smartly only alerts for NEW trades after you start.

---

## 🆘 Still Need Help?

**Browser Console (for errors):**
1. Press F12 (or Cmd+Option+I on Mac)
2. Click "Console" tab
3. Look for red errors
4. Screenshot and search error online

**Reset Everything:**
```javascript
// In browser console (F12)
localStorage.clear()
location.reload()
```

**Test Components Individually:**
- Test Sound: Click "Test Sound" button
- Test Discord: Click "Test Discord" button  
- Test Notification: Click "Test Alert" button
- Test API: Click "Check Now" button

---

## 📊 Understanding the Stats

**Tracking:** Number of wallets in your portfolio  
**Alerts Today:** Resets at midnight, daily count  
**Total Signals:** Lifetime alert count  
**API Errors:** Failed API calls (should be low)  
**Last Check:** When system last polled API

---

**Remember:** This is a tool, not financial advice. Always do your own research before making trades. Good luck! 🚀
