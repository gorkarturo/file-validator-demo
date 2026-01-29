# File Validator - Digital & Print

A comprehensive web-based application for validating digital and print media files against specific requirements.

## Overview

This application provides two specialized validation modes:
- **Digital Validator**: For video and image files used in digital displays
- **Print Validator**: For print-ready PDF, JPG, and TIFF files

## Features

### Digital File Validator

- **Multi-File Upload**: Validate multiple video and image files simultaneously
- **Supported Formats**: MP4, MOV, JPG
- **Video Validation**:
  - Dimension matching against 56 digital display formats
  - FPS verification (24-25 FPS required)
  - Duration check (10 seconds ±0.5s)
- **Results Table**: Shows matched displays, validation status, and important annotations
- **Smart Warnings**: Alerts when dimensions match but FPS/duration don't meet requirements
- **Database**: 56 digital supports covering shopping centers and airports across Spain

### Print File Validator

- **Trimbox Dimension Validation**: Checks if file dimensions match expected values with ±2mm tolerance
- **Scale Support**: Validates files at any scale from 1:1 (full scale) to 1:10
- **Color Mode Detection**: Validates that files are in CMYK color mode
- **Resolution Verification**: Ensures files meet minimum 100 PPP (pixels per inch) requirement
- **Search Functionality**: Quickly find recursos from a database of 24,954+ entries
- **Real-time Validation**: Instant feedback on file compliance
- **Database**: 24,954 print recursos loaded from inventory

## How to Use

### Digital Validator

1. Click "Digital" on the landing page
2. Upload one or more video (MP4, MOV) or image (JPG) files
3. Click "Validate Files"
4. Review the results table showing:
   - Which displays match your file dimensions
   - FPS and duration validation (for videos)
   - Any special annotations or requirements

### Print Validator

1. Click "Impresión" on the landing page
2. Enter a recurso code (e.g., R17-006705) or use the search feature
3. Upload your PDF, JPG, or TIFF file
4. Click "Validate File"
5. Review the detailed validation results including scale detection

## Validation Rules

### Digital Files
- **Dimensions**: Must match display resolution (±5px tolerance)
- **FPS**: 24-25 FPS for videos
- **Duration**: 10 seconds (±0.5s tolerance) for videos
- **Warnings**: Shown when dimensions match but FPS or duration are incorrect

### Print Files
- **Dimensions**: File trimbox must match recurso dimensions within ±2mm tolerance
- **Scale Support**: Files can be at any scale from 1:1 (full scale) to 1:10 and still pass validation
- **Color Mode**: File must be in CMYK color space
- **Resolution**: Minimum 100 PPP required

## Technical Details

- Built with React 18 and Tailwind CSS
- Client-side file processing (no server required)
- Dual-mode interface with easy navigation
- Responsive design for mobile and desktop
- Custom color scheme: #e6007e primary color

## Databases

- **Digital Supports**: 56 displays from major shopping centers and airports
- **Print Recursos**: 24,954 recursos for outdoor advertising

## Demo

Visit the live demo: [File Validator](https://gorkarturo.github.io/file-validator-demo/)

## License

© 2026 All rights reserved
