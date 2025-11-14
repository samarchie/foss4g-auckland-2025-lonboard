# FOSS4G Auckland 2025: Fast and Free
## High-performance WebGL Geospatial Visualisation using Lonboard

This repository contains the demonstration notebooks from Sam Archie's presentation at FOSS4G Auckland 2025, showcasing how Lonboard eliminates preprocessing bottlenecks in geospatial analysis workflows.

## 🚀 Quick Start
### Prerequisites

- Python 3.10+
- [uv](https://docs.astral.sh/uv/) for dependency management

### Installation

1. Clone this repository:
```bash
git clone https://github.com/samarchie/foss4g-auckland-2025-lonboard.git
cd foss4g-auckland-2025-lonboard
```

2. Install dependencies with uv (this will automatically create a virtual environment):
```bash
uv sync
```

3. Start Jupyter Lab using uv:
```bash
uv run jupyter lab
```

## 📊 Demonstration Notebooks
### 1. Climate Projections Analysis (climate_viewer.ipynb)

Visualises NIWA's 2024 climate projections across New Zealand using SSP scenarios.

Key Features:

- Property-level climate impact assessment
- Interactive filtering by historical temperature ranges
- GPU-accelerated rendering of temperature gradients
- Real-time exploration of climate adaptation scenarios

### 2. Traffic Crash Analysis (crash_viewer.ipynb)

Explores 25+ years of crash data from Waka Kotahi's Crash Analysis System.

Key Features:

- Multi-dimensional filtering (year, fatalities, injuries)
- Spatial clustering visualisation
- Road safety pattern identification
- Performance with large temporal datasets

### 3. Auckland Urban Infrastructure (osm_viewer.ipynb)

Maps Auckland's road networks and building footprints from OpenStreetMap.

Key Features:

- Speed limit-based road hierarchy visualisation
- Building footprint rendering
- Mixed geometry type handling
- Urban development pattern analysis

### 4. Real-Time Flight Tracking (flights_viewer.ipynb)

Animates flight paths across New Zealand airspace with temporal controls.

Key Features:

- Temporal flight path animation
- High-frequency positional data visualisation
- Aviation pattern analysis
- Interactive playback controls

## 🎯 Key Performance Improvements

Lonboard delivers order-of-magnitude performance gains over traditional approaches:

- 135× faster data serialization vs GeoJSON
- 26× smaller file sizes for data transfer
- 5.6× faster parsing in browser
- GPU-accelerated rendering enabling millions of features

## 🔧 Technical Architecture

Lonboard combines four foundational technologies:

- deck.gl - GPU-accelerated WebGL rendering
- GeoArrow - Efficient columnar geospatial memory format
- GeoParquet - Compressed binary geospatial file format
- anywidget - Modern Jupyter widget framework

## 🙏 Acknowledgments

This work builds on the groundbreaking technical innovations of Kyle Barron, creator and maintainer of Lonboard. Kyle's architectural work makes high-performance geospatial visualisation accessible to the Python community.

## 📚 Additional Resources

- Lonboard Documentation: https://developmentseed.org/lonboard/
- FOSS4G Auckland 2025: https://2025.foss4g.org/