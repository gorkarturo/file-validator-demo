# File Validator

A web-based application for validating PDF, JPG, and TIFF files against specific recursos (resources) requirements.

## Features

- **Trimbox Dimension Validation**: Checks if file dimensions match expected valores with ±2mm tolerance
- **Color Mode Detection**: Validates that files are in CMYK color mode
- **Resolution Verification**: Ensures files meet minimum 100 PPP (pixels per inch) requirement
- **Search Functionality**: Quickly find recursos from a database of 24,954+ entries
- **Real-time Validation**: Instant feedback on file compliance

## How to Use

1. Enter a recurso code (e.g., R17-006705) or use the search feature
2. Upload your PDF, JPG, or TIFF file
3. Click "Validate File" to check compliance
4. Review the detailed validation results

## Validation Rules

- **Dimensions**: File trimbox must match recurso dimensions within ±2mm tolerance
- **Color Mode**: File must be in CMYK color space
- **Resolution**: Minimum 100 PPP required

## Technical Details

- Built with React 18 and Tailwind CSS
- Client-side file processing (no server required)
- Database of 24,954 recursos loaded from CSV
- Supports PDF, JPG, JPEG, TIFF, and TIF file formats

## Demo

Visit the live demo: [File Validator](https://YOUR-USERNAME.github.io/file-validator-demo/)

## License

© 2026 All rights reserved
