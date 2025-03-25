# Sweater Stitch Calculator

## Overview

The Sweater Stitch Calculator is a comprehensive tool for knitters to generate all the key stitch and row counts needed to knit a sweater in the round. It calculates measurements based on a gauge swatch and body dimensions, and includes a yarn search feature that estimates yarn requirements, pricing, and detailed specifications.

## Features

### Stitch Calculations
- Converts gauge swatch measurements into stitch and row gauges
- Calculates bust, waist, and ribbing stitch counts
- Determines upper arm and cuff stitch counts
- Calculates sleeve increases/decreases needed
- Computes row counts for body and sleeves
- Works in both imperial (inches) and metric (cm) units

### Yarn Estimations
- Determines total yarn yardage needed based on standard reference tables
- Calculates number of balls required
- Estimates yarn weight in ounces/grams
- References a size chart for different bust measurements

### Yarn Search & Details
- Simulates searching for specific yarn brands and types
- Provides estimated price ranges and average costs
- Calculates total project cost based on number of balls needed
- Includes detailed yarn specifications:
  - Fiber content
  - Ball weight
  - Yardage per ball
  - Recommended needle size
  - Machine washability
  - Care instructions

## Project Files

The project consists of three main HTML files:

1. **index.html** - Main landing page with links to both imperial and metric versions
2. **imperial.html** - Calculator using imperial measurements (inches, yards, ounces)
3. **metric.html** - Calculator using metric measurements (cm, meters, grams)

Each HTML file contains all the necessary JavaScript code embedded directly in the page, so no external JavaScript files are required. This makes the calculator easy to deploy and use in any web browser without setting up a server.

## How to Use

1. **Download all three HTML files** to your local machine.
2. **Open index.html** in any modern web browser.
3. **Choose either the imperial or metric version** based on your preference.

### Using the Calculator

1. **Enter Gauge Swatch Measurements**
   - Number of stitches in your swatch
   - Width of swatch (inches or cm)
   - Number of rows in your swatch
   - Height of swatch (inches or cm)

2. **Enter Body Measurements**
   - Bust circumference
   - Waist circumference
   - Total torso length
   - Ribbing length
   - Arm length (from underarm)
   - Select yarn weight (light, medium, or heavy)

3. **Calculate Stitch Counts**
   - Click the "Calculate Stitches" button to generate all measurements

4. **Search for Yarn Information**
   - Enter a yarn brand name
   - Click "Search Yarn" to get detailed yarn information and price estimates

## Formulas Used

- **Stitch Gauge** = swatch stitch count ÷ swatch width
- **Row Gauge** = swatch row count ÷ swatch height
- **Bust Stitch Count** = stitch gauge × bust circumference
- **Waist Stitch Count** = stitch gauge × waist circumference
- **Bottom Ribbing Stitch Count** = bust stitch count × 0.9 (10% fewer stitches)
- **Upper Arm Stitch Count** = (33.3% of bust stitches) + (stitch gauge × 1 inch/2.54 cm)
- **Cuff Ribbing Stitch Count** = 20% of bust stitch count
- **Underarm Stitch Count** = 8% of bust stitch count
- **Sleeve Increases** = upper arm stitches - cuff ribbing stitches
- **Body Rows** = row gauge × (torso length - ribbing length)
- **Sleeve Rows** = row gauge × (arm length - 4 inches/10.16 cm)
- **Cuff Ribbing Rows** = row gauge × 2 inches/5.08 cm

## Technical Implementation

The calculator is built using modern web technologies:

1. **Frontend Framework**
   - React (loaded via CDN)
   - Babel for JSX transpilation
   - TailwindCSS for styling

2. **Embedded JavaScript**
   - All JavaScript code is included directly in the HTML files
   - No external files or server setup required
   - Self-contained application that works offline

3. **Reactive State Management**
   - Uses React's useState hooks for state management
   - Automatic UI updates when values change
   - Full form validation and error handling

## Deployment Options

There are several ways to use and share this calculator:

1. **Local Usage**
   - Download the HTML files and open them directly in a browser
   - No internet connection required after the initial load

2. **GitHub Pages**
   - Host on GitHub Pages for a free web version
   - Share with a simple URL

3. **Any Web Server**
   - Files can be hosted on any web server or CDN
   - No server-side processing required

## Future Enhancements

Potential improvements to consider:

- Save and load measurements
- Export results as PDF
- Integration with actual yarn databases for real-time pricing
- Support for different sweater construction methods
- Addition of colorwork and pattern stitch adjustments
- Integration with pattern libraries
- Mobile app version
- Visualization of the sweater based on measurements

## License

This project is available under the MIT License. See the LICENSE file for details.

## Credits

Designed and implemented for knitters looking to create custom-fit sweaters with accurate measurements and yarn requirements.
