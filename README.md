# 🎯 Habit Tracker PWA

A beautiful, modern Progressive Web App for tracking daily habits, building streaks, and staying accountable with a unique punishment system for missed habits.

![Habit Tracker Preview](https://img.shields.io/badge/PWA-Ready-green) ![No Dependencies](https://img.shields.io/badge/Dependencies-None-blue) ![Vanilla JS](https://img.shields.io/badge/JavaScript-Vanilla-yellow) ![License](https://img.shields.io/badge/License-MIT-green)

## ✨ Features

### 🏆 Core Functionality
- **Daily Habit Tracking** - Check off habits for each day of the week
- **Streak Counting** - Automatic calculation of consecutive completion days
- **Weekly & Monthly Dashboards** - Visual progress tracking with charts
- **Accountability System** - Fun punishment activities for missed habits
- **Offline-First** - Works completely offline after first load

### 🎨 User Experience
- **Beautiful Dark Theme** - Modern glassmorphism design
- **Responsive Design** - Perfect on mobile, tablet, and desktop
- **Toast Notifications** - Real-time feedback for all actions
- **Confetti Celebrations** - Milestone streak achievements (7, 30, 100+ days)
- **Keyboard Shortcuts** - Power user navigation
- **Install Prompt** - Add to home screen functionality

### 📊 Analytics & Insights
- **Progress Visualization** - SVG-based circular progress charts
- **Weekly Completion Rates** - Track your consistency
- **Monthly Performance** - Detailed habit-by-habit breakdown
- **Best/Worst Performers** - Identify habits that need attention
- **Consistency Scoring** - Gamified progress tracking

### 🔧 Technical Features
- **PWA Compliant** - Installable with offline support
- **No Dependencies** - Pure vanilla JavaScript
- **Local Storage** - All data stored securely in your browser
- **Export/Import** - Backup and restore your data
- **Service Worker** - Background sync and caching

## 🚀 Quick Start

### Option 1: Direct Download
1. Download the `index.html` file
2. Open it in any modern web browser
3. Start adding your habits!

### Option 2: Clone Repository
```bash
git clone https://github.com/yourusername/habit-tracker-pwa.git
cd habit-tracker-pwa
```

Then simply open `index.html` in your browser or serve it with any static file server:
```bash
# Using Python
python -m http.server 8000

# Using Node.js (if you have http-server installed)
npx http-server

# Using PHP
php -S localhost:8000
```

### Option 3: Install as PWA
1. Open the app in Chrome, Safari, or other PWA-compatible browser
2. Look for the "Install App" button or browser install prompt
3. Add to your home screen for a native app experience

## 🎮 Usage

### Adding Habits
1. Click on the "My Habits" tab
2. Enter your habit name (e.g., "Drink 8 glasses of water", "Exercise for 30 minutes")
3. Press Enter or click "Add Habit"

### Tracking Progress
- Check off completed habits for each day of the week
- View your current streak for each habit
- Switch to Weekly/Monthly dashboards for detailed analytics

### Accountability System
- If you miss habits from the previous day, you'll get a morning check-in
- Choose whether you actually missed the habit or just forgot to check it off
- Get assigned fun punishment activities for actually missed habits

### Keyboard Shortcuts
- `Ctrl/Cmd + 1`: Switch to Habits tab
- `Ctrl/Cmd + 2`: Switch to Weekly Dashboard
- `Ctrl/Cmd + 3`: Switch to Monthly Dashboard
- `Ctrl/Cmd + K`: Focus on habit input field

## 🛠️ Tech Stack

- **HTML5** - Semantic markup with PWA meta tags
- **CSS3** - Modern styling with Grid, Flexbox, animations
- **Vanilla JavaScript** - ES6+ features, no frameworks
- **PWA APIs** - Service Worker, Web App Manifest, Cache API
- **Local Storage** - Client-side data persistence
- **SVG** - Scalable graphics for progress visualization

## 📱 Browser Support

- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 11+
- ✅ Edge 79+
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 🎯 Architecture

```
habit-tracker-pwa/
├── index.html              # Single-file PWA application
├── README.md              # This file
├── LICENSE                # MIT License
└── screenshots/           # App screenshots
    ├── desktop-view.png
    ├── mobile-view.png
    └── dashboard-view.png
```

### Code Structure
- **HabitTracker Class** - Main application logic
- **Utils Object** - Utility functions for storage, dates, notifications
- **PWA Setup** - Service worker and manifest generation
- **Event Handlers** - User interactions and lifecycle events

## 🎨 Customization

### Changing Colors
Modify the CSS custom properties in the `<style>` section:
```css
:root {
  --primary-color: #3b82f6;
  --secondary-color: #8b5cf6;
  --success-color: #10b981;
  --danger-color: #ef4444;
}
```

### Adding New Punishments
Edit the `PUNISHMENTS` array in the JavaScript section:
```javascript
const PUNISHMENTS = [
    "Your custom punishment activity! 🎯",
    // ... add more
];
```

### Modifying Habit Categories
The app currently supports general habits, but you can extend it by:
1. Adding category selection in the `addHabit` function
2. Filtering habits by category in the UI
3. Creating category-specific dashboards

## 📊 Data Format

Habits are stored in localStorage as JSON:
```json
{
  "habits": [
    {
      "id": 1640995200000,
      "name": "Drink 8 glasses of water",
      "completions": {
        "2024-01-01": true,
        "2024-01-02": true
      },
      "createdAt": "2024-01-01T00:00:00.000Z"
    }
  ]
}
```

## 🔒 Privacy & Security

- **No Data Collection** - All data stays on your device
- **No Analytics** - No tracking or telemetry
- **No Network Requests** - Works completely offline
- **Local Storage Only** - Data never leaves your browser

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/amazing-feature`
3. **Commit your changes**: `git commit -m 'Add amazing feature'`
4. **Push to the branch**: `git push origin feature/amazing-feature`
5. **Open a Pull Request**

### Development Guidelines
- Keep it dependency-free (vanilla JS only)
- Maintain single-file architecture
- Follow existing code style
- Test on multiple browsers
- Update README if needed

## 🐛 Bug Reports

Found a bug? Please create an issue with:
- Browser and version
- Steps to reproduce
- Expected vs actual behavior
- Screenshots if applicable

## 💡 Feature Requests

Have an idea? Open an issue with:
- Clear description of the feature
- Use case explanation
- Mockups or examples (if applicable)
- Priority level

## 📈 Roadmap

- [ ] **Habit Categories** - Organize habits by type (health, work, etc.)
- [ ] **Custom Punishment Lists** - User-defined punishment activities
- [ ] **Habit Templates** - Pre-made popular habits
- [ ] **Data Sync** - Optional cloud backup (keeping privacy-first)
- [ ] **Advanced Analytics** - Trend analysis and insights
- [ ] **Social Features** - Share achievements (optional)
- [ ] **Themes** - Light mode and custom color schemes
- [ ] **Habit Scheduling** - Different frequencies (weekly, monthly)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by popular habit tracking apps like Habitica and Streaks
- Icons and emojis from Unicode standard
- Design inspiration from modern glassmorphism trends
- Community feedback and contributions

## 📞 Support

- **Documentation**: Check this README and inline code comments
- **Issues**: Use GitHub Issues for bug reports and feature requests
- **Discussions**: Use GitHub Discussions for questions and ideas

## ⭐ Show Your Support

If this project helped you, please consider:
- ⭐ Starring the repository
- 🍴 Forking for your own modifications
- 📢 Sharing with friends who need habit tracking
- 💝 Contributing improvements

---

**Made with ❤️ using vanilla web technologies**

*No frameworks, no dependencies, no complexity - just pure web standards working beautifully together.*
