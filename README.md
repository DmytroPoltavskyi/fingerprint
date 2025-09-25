# Fingerprint

A universal browser fingerprinting solution based on **extensive research and analysis** of device characteristics across different browsers and webviews. This project represents a comprehensive study of browser APIs and parameters to identify the most stable and reliable fingerprinting data.

## Research Foundation

This project is the result of **thorough investigation** into browser fingerprinting techniques. Every parameter has been:

- **Extensively tested** across multiple browsers and environments
- **Carefully evaluated** for cross-browser consistency and stability
- **Rigorously analyzed** to ensure universal compatibility
- **Systematically filtered** to exclude volatile or browser-specific data

The selected parameters represent the **most reliable subset** of all available browser characteristics, specifically chosen to meet the demanding requirements of universal device identification.

## Core Concept

This fingerprinting approach prioritizes **research-backed stability** and **proven compatibility**. The collected parameters are the result of comprehensive analysis and are specifically selected to:

- Remain **consistently identical** across different browsers (Chrome, Firefox, Safari, Edge, etc.)
- Work **reliably and uniformly** in webviews (mobile apps, embedded browsers)
- **Completely avoid** browser-specific or application-dependent variations
- Provide **rock-solid user identification** across different environments

## Key Features

- **Universal Compatibility**: Works consistently across all modern browsers and webviews
- **Stable Fingerprinting**: Focuses only on parameters that don't change based on browser settings
- **Cross-Platform Reliability**: Generates identical fingerprints regardless of the browsing environment
- **Beautiful JSON Display**: Clean, readable JSON format for easy analysis
- **One-Click Copy**: Large, prominent copy button for easy data extraction
- **Responsive Design**: Works perfectly on desktop and mobile devices

## Research-Based Parameter Selection

After **comprehensive analysis of all available browser APIs and characteristics**, the application collects only the most **proven stable and universal** fingerprint parameters. Each parameter has been **extensively tested and validated** across multiple environments.

### ✅ Included Parameters (Research-Validated)

**Hardware & System** _(Proven stable across all environments)_

- **Screen Dimensions**: Physical screen width and height - _consistently identical across browsers_
- **Device Pixel Ratio**: Display density ratio - _hardware-based, browser-independent_
- **Hardware Concurrency**: Number of logical processors - _system-level characteristic_
- **Platform**: Operating system platform identifier - _OS-level data, browser-agnostic_
- **Max Touch Points**: Maximum simultaneous touch points - _hardware capability, universally consistent_

**Regional & Locale** _(System-level, cross-browser stable)_

- **Timezone**: User's timezone - _system setting, identical across all browsers_
- **DateTime Locale**: Date/time formatting locale - _OS-level configuration_

**Display Capabilities** _(Hardware-based characteristics)_

- **Color Depth**: Screen color depth or pixel depth - _display hardware specification_

### ❌ Excluded Parameters (Research-Identified Issues)

Through **extensive testing and analysis**, the following parameters were **intentionally excluded** due to cross-browser inconsistencies:

- **Language Preferences**: Can differ between browser settings and system locale
- **Theme Preferences**: Browser-dependent implementation varies significantly
- **Motion/Transparency Preferences**: Browser-specific accessibility features with inconsistent APIs
- **User Agent**: Easily spoofed and increasingly standardized across browsers
- **Plugins/Extensions**: Browser-specific and privacy-restricted in modern browsers

> **Research Note**: Every excluded parameter was tested across multiple browser environments and showed significant variation that would compromise the universal identification goal.

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

## Research Methodology & Testing

This project represents **months of systematic research** into browser fingerprinting techniques. The methodology included:

### **Comprehensive API Analysis**

- **Exhaustive review** of all available browser APIs and properties
- **Systematic testing** of each parameter across different environments
- **Statistical analysis** of parameter stability and consistency
- **Documentation** of cross-browser behavior patterns

### **Multi-Environment Validation**

The selected parameters have been **rigorously tested** and produce **identical results** across:

- **Desktop Browsers**: Chrome, Firefox, Safari, Edge, Opera
- **Mobile Browsers**: Chrome Mobile, Safari Mobile, Samsung Internet, Firefox Mobile
- **WebViews**: Android WebView, iOS WKWebView, Electron apps
- **Embedded Browsers**: In-app browsers, social media browsers
- **Different OS Versions**: Windows, macOS, Linux, iOS, Android

### **Stability Verification**

Each included parameter was verified to:

- Remain **constant across browser sessions**
- Show **zero variation** between different browsers on the same device
- Maintain **consistency** across browser updates and system changes
- Provide **reliable identification** over extended time periods

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

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

**Dmitriy Poltavskiy** - _Research and Development_

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.
