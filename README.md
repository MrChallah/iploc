# GPS + IP GEO Location Dual Mode Overlay - for Kick/Twitch/YouTube/Rumble and More!

## Two Versions Available

### 🌐 IP-Only Version (Most Compatible)
**URL:** `https://mrchallah.github.io/iploc`
- **Best for:** PRISM Live, OBS, XSplit, and most streaming apps
- **Accuracy:** Lower (IP-based location)
- **Compatibility:** Universal - works in all environments
- **Use case:** When you need maximum compatibility across different streaming platforms like OBS and PRISM Live Studio

### 📍 GPS + IP Version (Most Accurate)  
**URL:** `https://mrchallah.github.io`
- **Best for:** IRL Pro and GPS-capable environments
- **Accuracy:** High (GPS + IP fallback)
- **Compatibility:** Limited to GPS-friendly environments
- **Use case:** When you need precise location data and are using apps like IRL Pro

## Quick Setup

### For PRISM Live / OBS / Most Streaming Apps
Use the **IP-Only version**: `https://mrchallah.github.io/iploc`

### For IRL Pro / GPS-Capable Apps
Use the **GPS+IP version**: `https://mrchallah.github.io`

## Features

### 🕒 Real-Time Clock
- Displays current day, date, and time
- Format: "Day, DD/MM/YYYY, HH:MM:SS AM/PM"
- Updates every second

### 📍 Location Detection

#### IP-Only Version Features:
- **PRISM Live Integration** - Detects and uses PRISM Live's location data
- **Universal IP Location** - Works with Google, IP-API, IPInfo, and IPAPI.co
- **App Environment Detection** - Automatically detects streaming app environments
- **No GPS Conflicts** - Avoids GPS permission issues in app environments

#### GPS+IP Version Features:
- **IRL Pro GPS** - Primary source for IRL Pro users
- **High-Accuracy GPS** - Browser-based GPS with mobile optimization
- **Smart Fallback** - Falls back to IP location when GPS fails
- **GPS Caching** - Remembers recent GPS data for reliability

### 🌤️ Weather Information
- Current temperature in both Celsius and Fahrenheit
- Detailed weather description
- Powered by Open Meteo API (no API key required)

### 📱 Mobile & App Optimized
- Enhanced timeout settings for iOS devices
- Streaming app compatibility detection
- Mobile-specific GPS handling
- Responsive design for all screen sizes

## Detailed Compatibility

### IP-Only Version (`mrchallah.github.io/iploc`)
✅ **Works Great With:**
- PRISM Live
- OBS Studio
- XSplit
- Streamlabs Desktop
- Any streaming software
- Mobile browsers
- Desktop browsers

❌ **Limitations:**
- Less accurate location (city-level)
- No GPS precision

### GPS+IP Version (`mrchallah.github.io`)
✅ **Works Great With:**
- IRL Pro
- Desktop browsers with GPS
- Mobile browsers
- Direct browser usage

❌ **Limitations:**
- May not work in PRISM Live
- Can have GPS permission conflicts in some apps
- Requires location permissions

## Setup Instructions

### Method 1: Browser Source (OBS/Streaming Software)
1. Add a new "Browser Source"
2. Enter URL:
   - For maximum compatibility: `https://mrchallah.github.io/iploc`
   - For GPS accuracy: `https://mrchallah.github.io`
3. Set width: 800, height: 600 (or as needed)
4. Check "Shutdown source when not visible" for performance

### Method 2: PRISM Live Overlay
1. Go to PRISM Live overlay settings
2. Add web overlay with URL: `https://mrchallah.github.io/iploc`
3. Position as desired

### Method 3: IRL Pro Integration
1. Use URL: `https://mrchallah.github.io`
2. Allow location permissions when prompted
3. IRL Pro's GPS data will be automatically detected and used

## Configuration

### Location Refresh
Both versions auto-refresh location data every 90 seconds to ensure current information while preserving performance.

### App Detection (IP-Only Version)
The IP-only version automatically detects streaming app environments and optimizes accordingly:
- Skips GPS attempts in app environments
- Uses specialized PRISM Live location interfaces
- Falls back to multiple IP location services

## API Dependencies

### No API Keys Required!
Both versions use free services:
- **Reverse Geocoding**: Google Maps API (with Nominatim fallback)
- **Weather**: Open Meteo API
- **IP Location**: Multiple free services (Google, IP-API, IPInfo, IPAPI.co)

## Styling & Customization

### Visual Design
- Transparent background for overlay use
- White text with black shadow for maximum visibility
- Font Awesome icons for professional appearance
- Responsive layout that works on any screen size

### Icons Used
- 🕒 Clock icon for time display
- 📍 Location dot for place information  
- ☁️ Cloud icon for weather data

## Browser Compatibility

### Supported Browsers
- Chrome/Chromium (recommended)
- Firefox
- Safari
- Edge
- Mobile browsers (iOS Safari, Chrome Mobile)

### Required Permissions
- **GPS Version**: Location access required
- **IP Version**: No permissions needed
- **Both**: Internet connection required

## Troubleshooting

### Location Not Loading (IP Version)
1. **Check internet connection**: Ensure network connectivity
2. **Try different browser**: Some corporate networks block location services
3. **Clear browser cache**: Refresh the page completely

### Location Not Loading (GPS Version)  
1. **Check browser permissions**: Ensure location access is granted
2. **HTTPS required**: Modern browsers require HTTPS for GPS access
3. **Try IP version**: Use `mrchallah.github.io/iploc` as fallback
4. **Indoor GPS issues**: GPS accuracy decreases indoors

### Weather Not Displaying
1. **Internet connectivity**: Verify network access
2. **Temporary service issue**: Weather API might be temporarily unavailable
3. **Refresh page**: Try reloading the overlay

### PRISM Live Issues
1. **Use IP version**: Make sure you're using `mrchallah.github.io/iploc`
2. **Check overlay settings**: Ensure web overlay is properly configured
3. **Browser permissions**: Some versions require location permissions

## Performance Tips

### For Streaming
- Use IP version for better stability during streams
- Position overlay in a corner to avoid content interference
- Test before going live to ensure proper functionality

### For Mobile IRL Streaming
- GPS version works best with IRL Pro
- IP version recommended for other mobile streaming apps
- Consider battery impact of GPS usage

## Version History & Updates

The overlays are automatically updated on the GitHub Pages hosting, so you'll always get the latest version by using the URLs above.

## License

This project is open source. Feel free to modify and distribute as needed.

## Contributing

Feel free to submit issues, feature requests, or pull requests to improve the overlay.

---

**Quick Reference:**
- **Maximum Compatibility**: `https://mrchallah.github.io/iploc`
- **Maximum Accuracy**: `https://mrchallah.github.io`
- **PRISM Live**: Use IP version
- **IRL Pro**: Use GPS version
- **OBS/XSplit**: Use IP version 
