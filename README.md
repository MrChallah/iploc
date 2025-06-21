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
- Displays current date and time.
- Format: "DD/MM/YYYY, HH:MM:SS AM/PM"
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

### 🌤️ Enhanced Weather Information
- **Universal Japanese Regional Weather Icons** - Beautiful v4 repository icons for all users worldwide
- **Enhanced Weather Detection** - Uses multiple Open-Meteo parameters (wind speed, precipitation, visibility, temperature) for comprehensive condition analysis
- **Complete Weather Coverage** - Supports all weather conditions including:
  - Wind conditions (windy, wind with rain, blizzards)
  - All precipitation types (light/moderate/heavy rain, snow, mixed precipitation, hail)
  - Severe weather (thunderstorms, tornadoes, tropical storms)
  - Extreme conditions (very hot, very cold, icy conditions)
  - Special conditions (fog, dust, blowing snow)
- **Smart Weather Logic** - Temperature-based descriptions (shows "Sunny" instead of "Clear" when temperature > 27°C)
- **Day/Night Icon Variations** - Proper weather icons that change based on time of day
- **Reliable Fallback System** - Automatically falls back to Google Maps icons if v4 icons fail to load
- **Current temperature** in both Celsius and Fahrenheit
- **Detailed weather descriptions** with accurate condition mapping
- **Powered by Open Meteo API** (no API key required)

### 📱 Mobile & App Optimized
- Enhanced timeout settings for iOS devices
- Streaming app compatibility detection
- Mobile-specific GPS handling
- Responsive design for all screen sizes

## Weather Icon System

### 🎌 Universal Japanese Regional Icons

**NEW**: All users worldwide now get the beautiful Japanese regional weather icons as the primary choice!

- **Premium Visual Experience** - Distinctive v4 repository weather icon designs for everyone
- **Enhanced Weather Detection** - Advanced condition analysis using wind speed, precipitation, visibility, and temperature
- **Complete Weather Coverage** - Icons for all weather conditions including extreme weather, mixed precipitation, and severe storms
- **Automatic Fallback** - Seamlessly falls back to Google Maps icons if v4 icons fail to load
- **Day/Night Variations** - Proper time-of-day specific icons for enhanced accuracy

### 🌍 Comprehensive Weather Conditions

The enhanced weather system now detects and displays icons for:

#### 🌬️ **Wind Conditions**
- Windy conditions (wind speed > 25 km/h)
- Wind with rain combinations
- Blowing snow in cold conditions

#### ❄️ **Enhanced Snow Detection**
- Blizzards (temperature < -10°C + high wind)
- Snowstorms (heavy snow + moderate wind)
- Heavy snow storms (extremely cold conditions)
- Snow with various intensities and wind combinations

#### 🌧️ **Advanced Rain Detection**
- Light, moderate, and heavy rain distinctions
- Mixed rain and snow (near freezing temperatures)
- Rain with wind combinations

#### ⛈️ **Severe Weather**
- Thunderstorms with intensity variations
- Hail detection in thunderstorms
- Scattered vs. heavy thunderstorms based on wind speed

#### 🌡️ **Extreme Temperature Conditions**
- Very hot conditions (> 35°C)
- Very cold conditions (< -20°C)
- Temperature-aware weather descriptions

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

### Enhanced Weather System
- **Universal v4 Icons** - Japanese regional weather icons for all users worldwide
- **Multi-Parameter Detection** - Uses wind speed, precipitation, visibility, and temperature for accurate condition analysis
- **Comprehensive Coverage** - All Google Weather API condition types supported with appropriate icons
- **Smart Fallback System** - Reliable icon loading with automatic fallback to Google Maps icons
- **Advanced Weather Logic** - Temperature-aware descriptions and extreme weather detection

## API Dependencies

### No API Keys Required!
Both versions use free services:
- **Reverse Geocoding**: Google Maps API (with Nominatim fallback)
- **Weather**: Enhanced Open Meteo API with multi-parameter detection (wind_speed_10m, precipitation, visibility, temperature_2m, weather_code, is_day)
- **IP Location**: Multiple free services (Google, IP-API, IPInfo, IPAPI.co)
- **Weather Icons**: Universal v4 repository Japanese regional icons with Google Maps fallback

## Styling & Customization

### Visual Design
- Transparent background for overlay use
- White text with black shadow for maximum visibility
- Font Awesome icons for professional appearance
- Responsive layout that works on any screen size
- Enhanced weather icons with drop shadows for better visibility

### Icons Used
- 🕒 Clock icon for time display
- 📍 Location dot for place information  
- 🎌 Dynamic Japanese regional weather icons that change based on conditions, time of day, and weather parameters

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
4. **Icon fallback**: v4 icons automatically fall back to Google Maps icons if needed

### PRISM Live Issues
1. **Use IP version**: Make sure you're using `mrchallah.github.io/iploc`
2. **Check overlay settings**: Ensure web overlay is properly configured
3. **Browser permissions**: Some versions require location permissions

## Recent Updates

### Major Weather System Overhaul
- **Universal Japanese Regional Icons** - All users worldwide now get beautiful v4 repository weather icons
- **Enhanced Weather Detection** - Multi-parameter analysis using wind speed, precipitation, visibility, and temperature
- **Complete Weather Coverage** - Support for all weather conditions including extreme weather, mixed precipitation, and severe storms
- **Smart Condition Logic** - Advanced weather condition detection beyond basic weather codes
- **Reliable Fallback System** - Automatic fallback to Google Maps icons ensures 100% reliability
- **Improved Performance** - Better error handling and reduced console noise

### New Weather Conditions Supported
- Wind-based conditions (windy, wind with rain)
- Enhanced snow detection (blizzards, snowstorms, heavy snow storms)
- Advanced rain detection (light/moderate/heavy distinctions)
- Severe weather variations (thunderstorm intensities, hail detection)
- Extreme temperature conditions (very hot, very cold)
- Mixed precipitation (rain and snow combinations)
- Visibility-based conditions (blowing snow, enhanced fog detection)

## Performance Tips

### For Streaming
- Use IP version for better stability during streams
- Position overlay in a corner to avoid content interference
- Test before going live to ensure proper functionality
- Weather icons now load more reliably with improved fallback system

### For Mobile IRL Streaming
- GPS version works best with IRL Pro
- IP version recommended for other mobile streaming apps
- Consider battery impact of GPS usage
- All users now get premium Japanese regional weather icons automatically

## Version History & Updates

The overlays are automatically updated on the GitHub Pages hosting, so you'll always get the latest version by using the URLs above. Recent major updates include the universal Japanese regional weather icon system and comprehensive multi-parameter weather detection.

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
- **Weather Icons**: Universal Japanese regional v4 icons for everyone
- **Weather Coverage**: Complete multi-parameter weather detection system 
