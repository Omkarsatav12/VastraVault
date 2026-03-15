# VastraVault
वस्त्रVault — AI-Powered Boutique Inventory Intelligence
About
VastraVault is a frontend-only web application designed for small Indian fashion boutique owners. It provides a complete retail management suite including smart POS, inventory tracking, WhatsApp order management, customer profiling, and AI-powered analytics — all without requiring any server or installation.


Live Demo
Open https://vastravault.netlify.app/  in any modern browser. No installation or server required.

Getting Started
Prerequisites
•	Any modern browser (Chrome, Firefox, Safari, Edge)
•	No Node.js, Python, or server required for basic usage
•	Internet connection only required for Chart.js (loaded from CDN)

Project Structure
vastravault/
├── index.html              # Landing page
├── dashboard.html          # Main dashboard
├── pos.html                # Point of Sale
├── inventory.html          # Inventory manager
├── whatsapp-orders.html    # WhatsApp order log
├── customers.html          # Customer profiles
├── analytics.html          # Analytics & reports
├── css/
│   ├── styles.css          # Global / landing styles
│   └── dashboard.css       # App / dashboard styles
├── js/
│   ├── data.js             # Mock data store
│   ├── dashboard.js        # Core app logic
│   └── app.js              # Landing page JS
└── assets/                 # Images and illustrations

Features
•	Smart POS & Billing: GST-compliant invoice generation, cart management, discount application, multiple payment modes.
•	WhatsApp Commerce: Log and track orders received via WhatsApp, status lifecycle from Pending to Delivered.
•	Inventory Management: Product grid with search, category and stock filters. Barcode scan placeholder.
•	Customer Profiles: Auto-built from purchase history, style preferences, targeted WhatsApp notifications.
•	Dead Stock Detector: Auto-flags items unsold 30+ days, AI-recommended discount percentages.
•	AI Demand Forecast: Predicted demand by category for next month (beta), with confidence scores.
•	Analytics Dashboard: Monthly revenue trend, sales by category, weekly performance charts.
Tech Stack
•	HTML5 + CSS3 + Vanilla JavaScript (ES6+)
•	Chart.js v4.4.7 for data visualization
•	CSS Custom Properties for theming
Browser Support
•	Chrome 90+ (recommended)
•	Firefox 88+
•	Safari 14+
•	Edge 90+
•	Mobile browsers (iOS Safari, Chrome Android)

Customization
Changing Mock Data
Edit js/data.js to update products, customers, and orders. All pages will reflect changes automatically on next load.
Changing Colors
Update CSS variables in css/styles.css under the :root block. The --primary (maroon) and --gold variables control the entire brand palette.
Adding a Real Backend
Replace the data arrays in data.js with fetch() calls to your REST API or Firebase. The rendering functions in dashboard.js are already separated from data concerns for easy integration.

Roadmap
•	Barcode scanning via device camera (WebRTC / BarcodeDetector API)
•	WhatsApp Business API integration for automated order notifications
•	Real AI demand forecasting using Claude API
•	PDF invoice export
•	Multi-store / multi-user support
•	Offline mode via Service Workers and IndexedDB
•	Mobile app wrapper via Capacitor or PWA

License
MIT License — free to use, modify, and distribute with attribution.
