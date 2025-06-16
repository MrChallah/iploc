# GPS + IP GEO Location Dual Mode Overlay - for Kick/Twitch/YouTube/Rumble and More!

# TLDR - Paste https://mrchallah.github.io as a Web Overlay in your streaming app, works great on IRL Pro.

A lightweight, transparent HTML overlay that displays real-time location, time, and weather information. Perfect for streaming, screen recording, or any application where you need persistent location data on your screen.

## Features

### 🕒 Real-Time Clock
- Displays current time in HH:MM:SS format
- Shows timezone offset (GMT±X)
- Updates every second

### 📍 Multi-Source Location Detection
The overlay uses a smart fallback system to ensure reliable location data:

1. **IRL Pro GPS** - Primary source (if available)
2. **Browser GPS** - High-accuracy GPS when available
3. **IP Location** - Fallback using Google Geolocation API

### 🌤️ Weather Information
- Current temperature in both Celsius and Fahrenheit
- Weather description
- Powered by OpenWeatherMap API

### 📱 Mobile Optimized
- Enhanced timeout settings for iOS devices
- Mobile-specific GPS handling
- Responsive design for all screen sizes

## Setup

### 1. API Keys
The overlay requires API keys for full functionality:

- **OpenWeatherMap API**: Replace `OWM_KEY` in the script
- **Google Geolocation API**: Replace `GOOGLE_GEO_KEY` in the script

### 2. Get API Keys

#### OpenWeatherMap
1. Visit [OpenWeatherMap](https://openweathermap.org/api)
2. Sign up for a free account
3. Generate an API key
4. Replace `618628ae452ff89f0e4477fba20b9d5c` in the code

#### Google Geolocation API
1. Go to [Google Cloud Console](https://console.cloud.google.com/)
2. Create a new project or select existing
3. Enable the Geolocation API
4. Create credentials (API key)
5. Replace `AIzaSyBFwxZu_EqPgs7pEqk1uHn1f46F6vUoEFU` in the code

### 3. Usage

#### As Browser Source (OBS/Streaming)
1. Open the HTML file in any modern web browser
2. Copy the file URL or use as local file
3. Add as "Browser Source" in OBS Studio
4. Set width/height as needed
5. Check "Shutdown source when not visible" for performance

#### Standalone Display
1. Open the HTML file directly in your browser
2. Allow location permissions when prompted
3. The overlay will start displaying information automatically

## Configuration

### Location Settings
```javascript
const options = {
  enableHighAccuracy: true,
  timeout: isIOS ? 60000 : (isMobile ? 45000 : 15000),
  maximumAge: gpsSuccessful ? 30000 : 0
};
```

### Refresh Interval
The overlay auto-refreshes location data every 90 seconds:
```javascript
setInterval(() => updateLocationAndWeather(), 90000);
```

## Styling

### Customization
The overlay uses a transparent background with white text and black shadow for maximum visibility:

```css
html,body {
  margin: 0;
  padding: 0;
  background: transparent;
  color: #fff;
  font-family: sans-serif;
}
```

### Icon Styling
Uses Font Awesome 6.5.0 for icons:
- 🕒 Clock icon for time
- 📍 Location dot for place
- ☁️ Cloud icon for weather

## Browser Compatibility

### Supported Browsers
- Chrome/Chromium (recommended)
- Firefox
- Safari (with limitations)
- Edge

### Required Permissions
- **Location Access**: For GPS functionality
- **Internet Connection**: For weather and IP location services

## Troubleshooting

### Location Not Loading
1. **Check browser permissions**: Ensure location access is granted
2. **HTTPS required**: Modern browsers require HTTPS for GPS access
3. **API key issues**: Verify your Google Geolocation API key is valid
4. **Network connectivity**: Ensure internet access for API calls

### Weather Not Displaying
1. **OpenWeatherMap API**: Check if your API key is active
2. **Rate limits**: Free tier has request limits
3. **Network issues**: Verify internet connectivity

### GPS Accuracy Issues
- **Indoor usage**: GPS accuracy decreases indoors
- **Device limitations**: Some devices have poor GPS hardware
- **Fallback system**: The overlay automatically falls back to IP location

## Technical Details

### Location Fallback Logic
1. Checks for IRL Pro GPS data (`window.locationData`)
2. Attempts browser GPS with device-specific timeouts
3. Falls back to Google IP geolocation
4. Uses cached GPS data if recent (within 5 minutes)

### Performance Features
- Caches successful GPS results for 30 seconds
- Smart retry logic for failed GPS attempts
- Optimized API calls to prevent rate limiting

## License

This project is open source. Feel free to modify and distribute as needed.

## Contributing

Feel free to submit issues, feature requests, or pull requests to improve the overlay.

---

**Note**: Replace the API keys in the code with your own valid keys before using in production. 
