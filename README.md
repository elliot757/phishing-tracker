# Global Phishing Tracker 🛡️

A real-time, interactive web-based dashboard that visualizes phishing email threats detected across the world. This educational project demonstrates how cybersecurity threat intelligence is tracked and analyzed globally.

![License](https://img.shields.io/badge/license-MIT-blue)
![Status](https://img.shields.io/badge/status-active-brightgreen)
![JavaScript](https://img.shields.io/badge/javascript-100%25-yellow)

## 🌍 Features

- **Live Global Heatmap** - Interactive world map showing phishing threat distribution by country
- **Real-Time Statistics** - Live counts of detected emails, affected countries, and threat types
- **24-Hour Trend Analysis** - Line chart showing phishing detection patterns over time
- **Attack Type Breakdown** - Doughnut chart displaying distribution of different phishing tactics
- **Top Affected Regions** - Sortable table showing countries with highest phishing activity
- **Detection Feed** - Live stream of individual phishing detections with details
- **Smart Filtering** - Filter threats by type (banking, cloud services, e-commerce, social media)
- **Dark Mode Support** - Full dark mode compatibility with system preferences
- **Fully Responsive** - Works seamlessly on desktop, tablet, and mobile devices

## 🎯 Threat Types Tracked

1. **Credential Theft** (34%) - Fake login pages capturing usernames/passwords
2. **Banking Trojan** (22%) - Financial institution impersonation and malware
3. **Package Delivery** (18%) - Shipping scam phishing campaigns
4. **Cloud Service Impersonation** (15%) - Fake Office 365, Google Drive, Dropbox
5. **CEO Fraud** (11%) - Executive impersonation for wire transfers

## 🚀 Getting Started

### Prerequisites

- Any modern web browser (Chrome, Firefox, Safari, Edge)
- No backend or server required
- Works offline (after initial load)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/elliot757/phishing-tracker.git
cd phishing-tracker
```

2. Open in your browser:
```bash
# Option 1: Direct file open
open index.html

# Option 2: With Python (for testing)
python -m http.server 8000
# Visit http://localhost:8000

# Option 3: With Node.js
npx http-server
```

That's it! No installation or build process required.

## 📁 Project Structure

```
phishing-tracker/
├── index.html          # Main HTML file
├── styles.css          # CSS styling (fully responsive)
├── data.js             # Threat data and helper functions
├── dashboard.js        # Dashboard functionality and interactivity
├── README.md           # This file
├── LICENSE             # MIT License
├── CONTRIBUTING.md     # Contribution guidelines
└── SECURITY.md         # Security and educational use guidelines
```

## 🔧 Technology Stack

- **Frontend**: HTML5, CSS3, JavaScript (Vanilla)
- **Charting**: Chart.js 4.4.1
- **Mapping**: D3.js 7.8.5 + TopoJSON 3.0.2
- **Data Source**: Simulated threat intelligence (educational)
- **Styling**: CSS Variables with dark mode support
- **CDN**: jsDelivr, cdnjs.cloudflare.com

## 📊 Data Overview

### Global Coverage
- 157+ countries tracked
- 10 top affected regions detailed
- Real-time metric updates every 15 seconds

### Sample Regions
| Country | Emails | % Global |
|---------|--------|----------|
| United States | 185K | 18% |
| India | 142K | 14% |
| United Kingdom | 98K | 10% |
| Germany | 87K | 8% |
| Canada | 76K | 7% |

## 💡 How It Works

1. **Data Collection** - Simulates aggregation from:
   - Email security gateways (Microsoft Defender, Proofpoint)
   - User phishing reports
   - Email authentication (DMARC, SPF, DKIM)
   - URL reputation services
   - Machine learning detection systems

2. **Processing** - Dashboard processes and visualizes:
   - Regional threat distribution
   - Attack type classification
   - Temporal trends (24-hour analysis)
   - Detection status (blocked vs. flagged)

3. **Visualization** - Interactive elements show:
   - Global heatmap with color-coded intensity
   - Live statistics and metrics
   - Detailed detection feed
   - Trend analysis charts

## 🎨 Customization

### Change Color Scheme
Edit CSS variables in `styles.css`:
```css
:root {
    --primary-color: #378ADD;
    --danger-color: #E24B4A;
    /* ... more colors ... */
}
```

### Add Real Data
Replace simulated data in `data.js` with real threat intelligence from:
- Proofpoint APIs
- Mimecast threat feeds
- Cisco Talos
- Microsoft Graph Security
- Custom data sources

### Modify Update Frequency
In `dashboard.js`, change the interval:
```javascript
updateInterval = setInterval(() => {
    // Update logic
}, 15000); // Change from 15 seconds
```

## 📈 Statistics

- **Total Dashboard Code**: ~1000 lines
- **Supported Browsers**: All modern browsers (Chrome 90+, Firefox 88+, Safari 14+, Edge 90+)
- **Page Load Time**: < 1 second
- **Data Update Interval**: 15 seconds
- **Responsive Breakpoints**: 480px, 768px, 1200px

## 🔒 Security & Educational Purpose

This project is for **educational purposes only**. It demonstrates:
- How threat intelligence dashboards work
- Visualization techniques for security data
- Real-world cybersecurity concepts

### Important Notes:
- Uses simulated/sample data, not real phishing statistics
- Does not collect personal information
- Does not connect to external threat databases by default
- Fully client-side processing (no backend required)

For detailed security information, see [SECURITY.md](SECURITY.md)

## 🤝 Contributing

We welcome contributions! See [CONTRIBUTING.md](CONTRIBUTING.md) for:
- Code style guidelines
- How to submit issues and pull requests
- Development setup
- Testing procedures

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

```
MIT License

Copyright (c) 2024 Global Phishing Tracker Contributors

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files...
```

## 🙏 Acknowledgments

- Chart.js for powerful charting capabilities
- D3.js and TopoJSON for geographic visualization
- Cybersecurity community for threat intelligence best practices
- All contributors and users

## 📞 Support & Contact

- **Issues**: Report bugs via [GitHub Issues](https://github.com/elliot757/phishing-tracker/issues)
- **Discussions**: Join [GitHub Discussions](https://github.com/elliot757/phishing-tracker/discussions)
- **Email**: your-email@example.com

## 🚀 Roadmap

Future enhancements planned:
- [ ] Real threat intelligence API integration
- [ ] WebSocket support for true real-time updates
- [ ] Advanced analytics and filtering
- [ ] Export reports (PDF, CSV)
- [ ] Historical data comparison
- [ ] Threat actor attribution
- [ ] Mobile native app version
- [ ] Notification system

## ⚡ Quick Facts

- ✅ Zero dependencies (except CDN libraries)
- ✅ Works completely offline after first load
- ✅ Mobile-responsive design
- ✅ Dark mode support
- ✅ WCAG accessible
- ✅ SEO optimized
- ✅ Progressive enhancement
- ✅ Cross-browser compatible

## 📚 Educational Resources

Learn more about phishing and cybersecurity:

1. **Phishing Detection**
   - NIST Cybersecurity Framework
   - OWASP Top 10
   - CIS Controls

2. **Email Security**
   - DMARC, SPF, DKIM protocols
   - Email authentication best practices
   - Threat intelligence feeds

3. **Data Visualization**
   - D3.js documentation
   - Chart.js tutorials
   - Responsive design principles

## 📄 Additional Documentation

- [SECURITY.md](SECURITY.md) - Security guidelines and responsible disclosure
- [CONTRIBUTING.md](CONTRIBUTING.md) - How to contribute to this project
- [LICENSE](LICENSE) - MIT License details

---

**Made with ❤️ for cybersecurity education**

Last Updated: January 2024 | Version 1.0.0
