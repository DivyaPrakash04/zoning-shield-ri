# ZoningShield RI 🏘️

**Rhode Island Parcel Zoning Explorer** - Built for GDG PVD Hackathon 2026

ZoningShield RI gives residents, nonprofits, and planners instant zoning clarity for any Rhode Island parcel — no consultants needed.

---

## 🚀 Quick Start

### Option 1: Open Directly (No Server Required)
Simply open `index.html` in any modern web browser:
- Double-click `index.html`
- Or drag it into your browser window

### Option 2: Live Server (Recommended for Development)
If you have VS Code or a similar editor:
1. Install the "Live Server" extension
2. Right-click `index.html`
3. Select "Open with Live Server"

---

## 🎯 Demo Instructions

### 1. Using Demo Cases (No API Key Required)
The app includes two pre-configured test cases:

**Test Case A - Providence (Urban Multi-Family)**
- Address: 245 Smith St, Providence, RI
- Zone: R-3 (Three-Family District)
- Features: Transit-proximate, allows 3 units by right

**Test Case B - Lincoln (Suburban Single-Family)**
- Address: 100 Old River Rd, Lincoln, RI
- Zone: R-20 (Single-Family Residential)
- Features: ADU state override, allows accessory dwelling unit

**To demo:**
1. Click either "Test Case A" or "Test Case B" button
2. View the four information panels that populate
3. Switch between languages using the language buttons
4. Click "Print / Save as PDF" to generate a report

### 2. AI-Powered Search (With Gemini API Key)
For live AI analysis of any RI address:

**Get a Gemini API Key:**
1. Go to [Google AI Studio](https://aistudio.google.com/)
2. Sign in with your Google account
3. Create a new API key
4. Copy the key (starts with "AIza...")

**Use AI Search:**
1. Paste your API key in the "🔑 Paste your Gemini API key" field
2. Click "Save Key"
3. Type any Rhode Island address (e.g., "123 Main St, Providence, RI")
4. Click "✨ Analyze with AI"
5. Wait for the analysis to complete

### 3. Smart Demo Mode (No API Key)
The app works without an API key using intelligent estimation:
1. Type any RI address in the search field
2. Click "✨ Analyze with AI"
3. The app will estimate zoning based on town detection
4. A yellow "Demo Mode" badge will appear

**Supported Towns in Demo Mode:**
- Providence, Pawtucket, Cranston, Warwick
- Cumberland, Lincoln, North Providence, Johnston
- Woonsocket, East Providence, Smithfield

---

## 🌐 Multilingual Support

The app supports 5 languages for accessibility:
- **English** 🇺🇸
- **Español** 🇪🇸
- **Português** 🇧🇷
- **Kreyòl Ayisyen** 🇭🇹
- **Français** 🇫🇷

Click any language button to instantly translate the entire interface.

---

## 📊 Information Panels

### Panel 1: Parcel Info
- Full address
- Zoning district classification
- Lot size and height limits
- Links to municipal ordinance
- Link to Rhode Island Zoning Atlas

### Panel 2: Town Checklist
- Baseline zoning constraints
- Setback requirements (front, side, rear)
- Maximum building height
- Units allowed by right
- Direct links to ordinance sections

### Panel 3: State Reform Audit
- **ADU Override**: Shows when state law (RIGL § 45-24-73) overrides local restrictions
- **Parking Reform**: Identifies transit-proximate parcels eligible for parking waivers
- **Middle Housing**: Highlights streamlined review pathways for 2-5 unit developments
- **E-Permits**: Notes electronic permitting standards for single-family lots

### Panel 4: Neighbor Summary
- Plain-language explanation of what can be built
- Nearby transit and amenities
- Distance to key locations
- Printable report generation

---

## 🛠️ Technical Details

### Tech Stack
- **Pure HTML/CSS/JavaScript** - No frameworks
- **Google Fonts**: Inter and Outfit
- **Google Gemini 1.5 Flash** (optional AI integration)
- **Responsive Design**: Mobile-first approach

### File Structure
```
GDGPVD/
├── index.html          # Main application (single-file architecture)
├── context.md          # AI agent system prompt
├── README.md           # This file
└── .gitignore          # Git configuration
```

### Browser Compatibility
- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Mobile)

---

## 🏆 Hackathon Context

**Built for**: GDG PVD Hackathon 2026

**Problem Solved**: Rhode Island's 39 municipal zoning codes are complex and inaccessible to everyday residents. ZoningShield RI simplifies this by:
- Providing instant zoning clarity
- Highlighting state-level housing reforms (2024-2026)
- Supporting multilingual communities
- Educating residents about their rights (e.g., ADU overrides)

**Civic Impact**:
- Increases housing accessibility awareness
- Promotes transit-oriented development
- Supports language justice for diverse communities
- Empowers residents with knowledge of state reform rights

---

## ⚖️ Legal Disclaimer

> ⚠️ Nothing in this application is official legal advice. Confirm all findings against the town's active ordinance and the Rhode Island Zoning Atlas.

This tool provides estimates and educational information. Always verify with local planning departments before making development decisions.

---

## 🔧 Development Notes

### Adding New Demo Cases
Edit the `CASES` object in `index.html` (line 1071) to add new parcel profiles.

### Adding New Languages
1. Add a new language key to the `T` object (line 1092)
2. Translate all required fields
3. Add a new language button in the HTML (line 1024-1028)

### Customizing Town Profiles
Edit the `riTowns` object in the `smartDemoFallback` function (line 1314) to adjust zoning profiles.

---

## 📝 License

This project was created for the GDG PVD Hackathon 2026. Please contact the authors for reuse permissions.

---

## 🤝 Contributing

This is a hackathon project. For suggestions or improvements, please open an issue or contact the development team.

---

**Built with ❤️ for Rhode Island communities**
