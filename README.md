# Fingerprint

A universal browser fingerprinting solution that collects the most stable and reliable device characteristics across different browsers and webviews. This project focuses on gathering fingerprint data that remains consistent regardless of the browser, application, or webview environment.

## Core Concept

This fingerprinting approach prioritizes **cross-browser stability** and **universal compatibility**. The collected parameters are carefully selected to:

- Remain consistent across different browsers (Chrome, Firefox, Safari, Edge, etc.)
- Work reliably in webviews (mobile apps, embedded browsers)
- Avoid browser-specific or application-dependent variations
- Provide stable user identification across different environments

## Key Features

- **Universal Compatibility**: Works consistently across all modern browsers and webviews
- **Stable Fingerprinting**: Focuses only on parameters that don't change based on browser settings
- **Cross-Platform Reliability**: Generates identical fingerprints regardless of the browsing environment
- **Beautiful JSON Display**: Clean, readable JSON format for easy analysis
- **One-Click Copy**: Large, prominent copy button for easy data extraction
- **Responsive Design**: Works perfectly on desktop and mobile devices

## Collected Parameters

The application collects only the most **stable and universal** fingerprint parameters:

### Hardware & System

- **Screen Dimensions**: Physical screen width and height
- **Device Pixel Ratio**: Display density ratio
- **Hardware Concurrency**: Number of logical processors available
- **Platform**: Operating system platform identifier
- **Max Touch Points**: Maximum simultaneous touch points supported

### Regional & Locale

- **Timezone**: User's timezone (stable across browsers)
- **DateTime Locale**: Date/time formatting locale

### Display Capabilities

- **Color Depth**: Screen color depth or pixel depth

### Excluded Parameters

Some parameters are intentionally **commented out** because they can vary between browsers or applications:

- Language preferences (can differ between browser and system settings)
- Theme preferences (browser-dependent)
- Motion/transparency preferences (browser-specific accessibility settings)

## Usage

1. Open `index.html` in any modern web browser or webview
2. The universal fingerprint will be automatically generated and displayed in JSON format
3. Click the "Copy Fingerprint" button to copy the complete data to clipboard
4. Use the "Generate Fingerprint" button to refresh the data
5. Test across different browsers to verify consistency

## Use Cases

- **Cross-Browser User Tracking**: Link user actions across different browsers on the same device
- **Fraud Detection**: Identify users attempting to bypass restrictions by switching browsers
- **Analytics & Research**: Study device characteristics across different browsing environments
- **Security Applications**: Device identification for authentication systems
- **A/B Testing**: Ensure consistent user experience across browser switches

## Technical Implementation

- **Pure Web Technologies**: HTML, CSS, and JavaScript - no external dependencies
- **Universal API Usage**: Only uses APIs available across all modern browsers
- **Stability Focus**: Avoids volatile parameters that change between browser sessions
- **JSON Output**: Clean, structured data format for easy integration
- **Responsive Design**: Works identically on desktop and mobile devices

## Cross-Browser Testing

This fingerprinting solution has been designed to produce **identical results** across:

- **Desktop Browsers**: Chrome, Firefox, Safari, Edge, Opera
- **Mobile Browsers**: Chrome Mobile, Safari Mobile, Samsung Internet, Firefox Mobile
- **WebViews**: Android WebView, iOS WKWebView, Electron apps
- **Embedded Browsers**: In-app browsers, social media browsers

## Privacy & Ethics

- Collects only **publicly available** device characteristics
- No personal information or browsing history is accessed
- All data collection is **transparent** and visible to the user
- Designed for legitimate use cases like fraud prevention and analytics
- Users can see exactly what data is being collected

## Integration

The `collectEnvSimple()` function can be easily integrated into any web application:

```javascript
const fingerprint = collectEnvSimple();
console.log(JSON.stringify(fingerprint, null, 2));
```
