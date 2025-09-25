# Fingerprint

A simple web application that collects and displays browser fingerprint information in a beautiful, user-friendly interface.

## Features

- **Browser Fingerprint Collection**: Gathers various browser and device characteristics
- **Beautiful UI**: Modern, responsive design with gradient backgrounds and smooth animations
- **Copy Functionality**: Large, prominent copy button to easily copy fingerprint data
- **Responsive Design**: Works well on both desktop and mobile devices
- **Real-time Generation**: Automatically generates fingerprint on page load

## Collected Data

The application collects the following browser fingerprint data:

- **Languages**: Browser language preferences
- **Color Depth**: Screen color depth or pixel depth
- **Screen Dimensions**: Width and height of the screen
- **Device Pixel Ratio**: Display density ratio
- **Hardware Concurrency**: Number of logical processors
- **Timezone**: User's timezone
- **Platform**: Operating system platform
- **Max Touch Points**: Maximum number of simultaneous touch points
- **Reduced Motion**: User's motion preference setting
- **Reduced Transparency**: User's transparency preference setting
- **DateTime Locale**: Date/time formatting locale
- **Theme Preference**: Dark, light, or no preference

## Usage

1. Open `index.html` in any modern web browser
2. The fingerprint will be automatically generated and displayed
3. Click the "Copy Fingerprint" button to copy the data to clipboard
4. Use the "Generate Fingerprint" button to refresh the data

## Technical Details

- Pure HTML, CSS, and JavaScript - no external dependencies
- Uses modern browser APIs for data collection
- Graceful fallbacks for unsupported features
- Responsive design with CSS Grid and Flexbox
- Clipboard API with fallback for older browsers

## Browser Compatibility

- Modern browsers (Chrome 60+, Firefox 55+, Safari 12+, Edge 79+)
- Fallback support for older browsers where possible
- Mobile browsers supported

## Privacy Note

This application only collects publicly available browser information that websites can normally access. No personal data or tracking is performed.
