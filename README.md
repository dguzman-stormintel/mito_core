# mito_core
MITO Core is a unified data processing hub that combines powerful CSV/spreadsheet manipulation with real-time NOAA weather intelligence. Designed for environmental professionals, it streamlines data preparation for machine learning workflows and compliance documentation.
Key Features:

 Universal file converter (Excel, CSV, TSV, JSON, XML, ODS, and more)
 Real-time NOAA weather forecasts and precipitation data
 Automatic Google Maps integration
 Interactive data editor with cleaning tools
 H2O.ai export for ML model training
 Responsive design - works on desktop and mobile


 Quick Start
Option 1: Run Locally

Download mito_core.html
Open in any modern browser (Chrome, Firefox, Edge)
That's it! No server or installation required.

Option 2: GitHub Pages
Visit: https://dguzman-stormintel.github.io/mito-core/

 NOAA Weather Dashboard
Features

Location Search: Enter any U.S. city, zip code, or address
7-Day Forecast: Detailed weather predictions from NWS
Precipitation Table: Hourly breakdown of expected rainfall
Temperature Chart: Visual forecast using Chart.js
Auto-Updating Map: Google Maps centers on selected location

How It Works

Enter a location (e.g., "Los Angeles, CA")
System geocodes via OpenStreetMap/Nominatim
Fetches forecast from NOAA Weather API
Displays current conditions, forecast cards, and precipitation data
Updates map to show the location

Data Sources

NOAA/NWS API: Official National Weather Service forecasts
OpenStreetMap Nominatim: Geocoding services
Google Maps: Satellite/terrain visualization


Add/Delete Columns: Modify data structure
Add/Delete Rows: Edit records
Transpose: Flip rows and columns
Reformat & Clean: Standardize data formatting
Adjust to Consistent Format: Normalize column types
Live Preview: See changes in real-time

ML/AI Export Options

Download as CSV: Standard export for any use
Export for H2O.ai: Formatted specifically for H2O machine learning platform
Dataset Split: Configure training/validation splits (default 80/20)


🔌 Integration with Stormwater Intelligence Platform
MITO Core is designed to work seamlessly with other tools in the ecosystem:
┌─────────────────────────────────────────────────────────┐
│              STORMWATER INTELLIGENCE PLATFORM           │
├─────────────────────────────────────────────────────────┤
│                                                         │
│   Data Explorer ──►  MITO Core ──► 3D Earth             │
│         │                   │              │            │
│         │                   ▼              │            │
│         │                 ARCSEC ◄─────────┘            │
│         │                   │                           │
│         ▼                   ▼                           │
│        StormGPT ◄────     Monitoring                    │
│                                                         │
└─────────────────────────────────────────────────────────┘
Data Sharing
MITO Core uses browser LocalStorage to share data with other platform tools:
javascript// Location and weather data is automatically available to:
// - 3D Earth Viewer (flies to location)
// - ARCSEC (analyzes precipitation trends)
// - StormGPT (generates compliance documents)

🛠️ Technical Details
Architecture

Frontend: Vanilla HTML/CSS/JavaScript (no framework dependencies)
Charts: Chart.js for data visualization
File Processing: SheetJS (xlsx.js) for spreadsheet parsing
APIs: NOAA Weather API, OpenStreetMap Nominatim
Maps: Google Maps Embed API

Browser Compatibility
BrowserSupportedChrome 80+Firefox 75+Edge 80+Safari 13+
Dependencies (CDN-loaded)
html<script src="https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.18.5/xlsx.full.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>

Use Cases
1. Environmental Compliance

Process monitoring data (turbidity, pH, flow rates)
Integrate weather forecasts for QPE (Qualifying Precipitation Event) tracking
Prepare data for SWPPP documentation

2. Construction Site Management

Track precipitation forecasts for project sites
Process inspection logs and BMP inventories
Export data for compliance reporting

3. ML/AI Training Data Preparation

Clean and normalize environmental datasets
Split data for training/validation
Export in H2O.ai-compatible formats

4. General Data Processing

Convert between file formats
Clean and standardize messy data
Quick data exploration and editing


 Privacy & Security

Client-Side Processing: All data processing happens in your browser
No Data Upload: Your files never leave your computer
No Account Required: No login or registration needed
API Calls: Only weather/geocoding APIs are contacted (NOAA, OpenStreetMap)


 License
MIT License - Free for personal and commercial use.

Author
Daniel Guzman

7 years environmental compliance experience
UCAR COMET Certified (Quantitative Precipitation Forecasting)
Microsoft Azure AI/ML certified


Related Projects
ProjectDescriptionLinkData ExplorerFederal environmental data portal catalogView3D Earth ViewerCesium-based terrain visualizationViewARCSECAI analytics engine (LLM + Neural Network)ViewStormGPTCustom GPT for stormwater complianceViewStormwater IntelligenceMLOps monitoring dashboardView
