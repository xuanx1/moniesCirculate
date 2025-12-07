# Ringgit in Circulation, Over the Years

An interactive [visualization](https://xuanx1.github.io/moniesCirculate/currency_treemap.html) showing the circulation of Malaysian Ringgit by denominations over 25 years.

## Overview

This project provides an animated, interactive visualization of Malaysian currency in circulation from historical data. The visualization uses a Voronoi treemap to represent different banknote denominations, with smooth morphing animations as you navigate through various years.

![Screenshot 2025-12-07 221842](https://github.com/user-attachments/assets/e41cd872-c72d-46d7-8d85-fc2eec790f30)

## Features

### Visual Design
- **Voronoi Treemap Layout**: Denominations are represented as proportional polygonal regions
- **Smooth Morphing Animations**: 1200ms transitions between years showing smooth cell transformations
- **Gradient Coloring**: Color-coded denominations with gradient text styling
- **Arc-based Typography**: Curved title and statistics text following circular arcs
- **Banknote Previews**: Hover tooltips showing obverse/reverse images of banknotes

### Interactive Elements
- **Timeline Scrubber**: Click or drag the timeline at the bottom to navigate through years
- **Play/Pause Animation**: Auto-play through all years with smooth transitions
- **Hover Tooltips**: View denomination details including:
  - Human-readable denomination labels (e.g., "100 Ringgit")
  - Circulating value in millions
  - Percentage of total circulation
  - Monthly trend chart for the selected year
  - Banknote images (obverse and reverse)

### Animated Indicators
- **Title Gradient Progress**: Title text color transitions from pink (#c06c84) to peach (#f8b195) as animation progresses
- **Timeline Progress Bar**: Smoothly fills as years are navigated
- **Animated Statistics**: Total circulation value smoothly transitions between years (displayed in Billions)


## Data Structure
The visualization uses `data/currency_in_circulation.csv` with columns:
- **date**: Date in YYYY-MM-DD format
- **denomination**: Denomination code (e.g., note_100, coin_rm1)
- **value**: Amount in circulation (RM Million)

## File Structure

```
moniesCirculate/
├── currency_treemap.html    # Main visualization file
├── data/
│   └── currency_in_circulation.csv  # Historical circulation data
├── myr/                      # Banknote images
│   ├── obverse images       # Front side of notes
│   └── reverse images       # Back side of notes
├── bnd/                      # Supporting data (optional)
└── README.md                 # This file
```

## Future Enhancements

Potential improvements:
- Comparative analysis between years
- Currency composition statistics
- Historical trend analysis
- Export/download functionality
- Multiple visualization modes

