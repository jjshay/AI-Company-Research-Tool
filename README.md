# AI Company Research Tool

> An interactive M&A intelligence directory and research platform for 800+ private AI companies.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.0.0-green.svg)
![AI Companies](https://img.shields.io/badge/companies-800%2B-gold.svg)

## Overview

This tool provides comprehensive research capabilities for analyzing private AI companies, designed for:

- **M&A Professionals** - Identify acquisition targets, understand valuations, and analyze strategic fit
- **Investors** - Research funding rounds, evaluate company trajectories, and compare opportunities
- **Executives & CEOs** - Benchmark competitors, identify partnership opportunities, and track industry trends
- **Career Seekers** - Research potential employers, understand company cultures, and identify growth opportunities

## Features

### Main Directory (`index.html`)

#### Company Discovery
- **800+ Private AI Companies** across 8 categories:
  - Foundation Models (OpenAI, Anthropic, Mistral, etc.)
  - Developer Tools (LangChain, Cursor, Pinecone, etc.)
  - Enterprise AI (Glean, Moveworks, etc.)
  - GTM & Marketing AI
  - Fintech & Legal (Harvey, Ramp, etc.)
  - Healthcare AI (Tempus, PathAI, etc.)
  - Industrial AI (Scale AI, Figure, etc.)
  - Consumer AI (Perplexity, Midjourney, etc.)

#### Smart Filtering
- **Location Filter**: SF Bay Area, Boston, NYC, LA, Seattle, Austin, International
- **Badge Filter**:
  - 🦄 Unicorns ($1B+ valuation)
  - 🎯 M&A Targets (likely acquisition candidates)
  - 🌸 Late Bloomers (established companies with new momentum)
- **Category Filter**: All 8 AI categories
- **Tier System**: Organize companies into Tier 1, 2, 3 priorities

#### Interactive Features
- **Swipe Gestures** (Desktop & Mobile):
  - ← Left: Delete/Remove
  - → Right: Tier 1 (Top Priority)
  - ↑ Up: Tier 2 (Medium Priority)
  - ↓ Down: Tier 3 (Lower Priority)
- **AI Assistant**: Ask questions about M&A trends, Boston AI scene, unicorns, career advice
- **Voice Input**: Microphone support for hands-free queries
- **Insights Panel**: Rotating themes with actionable intelligence:
  - M&A Career Prep
  - Executive Trends
  - Hot Sectors
  - Investment Signals
  - Boston AI Scene
  - Unicorn Watch
  - Deal Flow Intel
  - Tech Talent Map

#### Alphabet Navigation
- Quick-jump A-Z navigation on the right side
- Smart highlighting shows which letters have matching companies

### Comparison Tool (`compare.html`)

#### Side-by-Side Analysis
- Compare up to **5 companies** simultaneously
- Key metrics comparison:
  - Funding (with visual bars)
  - Founded year
  - Employee count
  - CEO
  - Headquarters
  - Rating
  - Category

#### Deep Dive Analysis
- **Products & Secret Sauce**: Competitive advantages breakdown
- **M&A Intelligence**: Acquisition insights and success factors
- **AI-Generated Insights**:
  - Funding leader analysis
  - Company maturity assessment
  - Category diversification check
  - Geographic concentration warnings
  - Quality score evaluation

#### Export Options
- 📄 Export to PDF
- 📊 Export to CSV
- 🖨️ Print-friendly formatting

## Installation

### Option 1: Direct Download
1. Download or clone this repository
2. Open `index.html` in any modern browser
3. No server required - runs entirely client-side

### Option 2: GitHub Pages
1. Fork this repository
2. Go to Settings → Pages
3. Select "main" branch and save
4. Access at `https://yourusername.github.io/AI-Company-Research-Tool/`

### Option 3: Local Server
```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx serve .

# Using PHP
php -S localhost:8000
```

## Usage

### Basic Research Workflow

1. **Browse Companies**: Scroll through the card-based directory
2. **Filter & Search**: Use dropdowns and search to narrow results
3. **Tier Companies**: Swipe or click buttons to organize by priority
4. **View Details**: Click company name for M&A insights modal
5. **Compare**: Select companies and use comparison tool
6. **Export**: Download CSV or PDF for offline analysis

### For M&A Professionals

1. Filter by "🎯 M&A Targets" to see acquisition candidates
2. Use location filter to find regional targets
3. Check funding levels and employee counts for sizing
4. Read M&A Insights in company modals
5. Compare similar companies side-by-side
6. Export shortlist for deal team review

### For Investors

1. Filter by category to focus on sectors
2. Sort by "Funding High-Low" to see capital intensity
3. Use "🦄 Unicorns" filter for later-stage companies
4. Compare funding trajectories in comparison tool
5. Check success factors for due diligence

### For Career Seekers

1. Use location filter to find companies in your area
2. Check employee counts for company stage preference
3. Read "Secret Sauce" for culture/focus insights
4. Compare compensation-relevant factors (funding, stage)
5. Use AI Assistant for career advice queries

## Data Structure

Each company includes:

```javascript
{
  id: Number,
  name: String,
  product: String,
  category: String,
  founded: Number,
  ceo: String,
  funding: String,
  fundingValue: Number,
  rating: Number (1-5),
  website: String,
  hq: String,
  employees: String,
  secretSauce: String,
  description: String,
  maInsight: String,
  successFactors: Array<String>
}
```

## Browser Support

- Chrome (recommended)
- Firefox
- Safari
- Edge
- Mobile browsers (iOS Safari, Chrome for Android)

## Privacy

- **100% Client-Side**: No data sent to servers
- **Local Storage**: Tier selections saved in browser only
- **No Tracking**: No analytics or user tracking

## Contributing

Contributions welcome! Please:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Adding Companies

To add new companies, edit the `companies` array in the JavaScript section:

```javascript
{
  id: [next available ID],
  name: "Company Name",
  product: "Main Product",
  category: "category-slug",
  founded: 2023,
  ceo: "CEO Name",
  funding: "$XXM",
  fundingValue: XX000000,
  rating: 4,
  website: "company.com",
  hq: "City, State",
  employees: "XX-XX",
  secretSauce: "Key differentiator",
  description: "Brief description",
  maInsight: "M&A analysis",
  successFactors: ["Factor 1", "Factor 2"]
}
```

## Roadmap

- [ ] Real-time data updates via API
- [ ] User accounts for saved research
- [ ] Team collaboration features
- [ ] Advanced charting and visualization
- [ ] News feed integration
- [ ] LinkedIn integration
- [ ] Crunchbase data sync

## License

MIT License - see [LICENSE](LICENSE) file for details.

## Acknowledgments

- Data compiled from public sources including Crunchbase, LinkedIn, and company websites
- Built for the M&A and investment research community
- Inspired by the need for better AI company intelligence tools

---

**Disclaimer**: Company information is compiled from public sources and may not reflect current status. Always verify information before making investment or business decisions.
