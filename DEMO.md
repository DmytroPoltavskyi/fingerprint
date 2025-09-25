# Live Demo

🌐 **Try the live demo:** [https://dmytropoltavskyi.github.io/fingerprint/](https://dmytropoltavskyi.github.io/fingerprint/)

## What You'll See

The demo will automatically:
1. **Generate your device fingerprint** using 10 stable parameters
2. **Display the data in JSON format** for easy reading
3. **Provide a copy button** to export the fingerprint data

## Cross-Browser Testing

To see the universal compatibility in action:

1. **Open the demo in different browsers** on the same device:
   - Chrome
   - Firefox  
   - Safari
   - Edge
   - Mobile browsers

2. **Compare the results** - they should be identical across all browsers

3. **Test in webviews** - mobile apps, embedded browsers, etc.

## Expected Results

You should see consistent fingerprint data like:
```json
{
  "colorDepth": 24,
  "screenWidth": 1920,
  "screenHeight": 1080,
  "dpr": 1,
  "hardwareConcurrency": 8,
  "timezone": "America/New_York",
  "platform": "MacIntel",
  "maxTouchPoints": 0,
  "reducedMotion": false,
  "reducedTransparency": false
}
```

## Integration Example

Use the fingerprint data in your applications:
```javascript
// Copy the collectEnvSimple function from the demo
const fingerprint = collectEnvSimple();
const fingerprintHash = btoa(JSON.stringify(fingerprint));
console.log('Device ID:', fingerprintHash);
```
