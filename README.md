# GPS + IP GEO Location Dual Mode Overlay - for Kick/Twitch/YouTube/Rumble and More!

# Credits
Weather icons from [@mrdarrengriffin](https://github.com/mrdarrengriffin/google-weather-icons) - A collection of the official weather icons used by Google officially.

## Four Versions Available

### 🌐 IP-Only Version (Most Compatible) - Best for OBS/Prism Live
**URL:** `https://mrchallah.github.io/iploc`
- **Best for:** PRISM Live, OBS, XSplit, and most streaming apps
- **Accuracy:** Lower (IP-based location)
- **Compatibility:** Universal - works in all environments
- **Weather Icons:** Japanese Google Weather Icons
- **Use case:** When you need maximum compatibility across different streaming platforms like OBS and PRISM Live Studio

### 📍 GPS + IP Version (Most Accurate) - Best for IRL Pro
**URL:** `https://mrchallah.github.io/`
- **Best for:** IRL Pro and GPS-capable environments
- **Accuracy:** High (GPS + IP fallback)
- **Compatibility:** Limited to GPS-friendly environments
- **Weather Icons:** Japanese Google Weather Icons
- **Use case:** When you need precise location data and are using apps like IRL Pro

### 🎨 Font Awesome IP-Only Version (Alternative Style)
**URL:** `https://mrchallah.github.io/classiciploc`
- **Best for:** Users who prefer Font Awesome icon style
- **Accuracy:** Lower (IP-based location)
- **Compatibility:** Universal - works in all environments
- **Weather Icons:** Font Awesome icons with day/night variations
- **Use case:** Alternative styling for OBS, PRISM Live, and streaming apps

### 🎨📍 Font Awesome GPS + IP Version (Alternative Style + Accuracy)
**URL:** `https://mrchallah.github.io/classic`
- **Best for:** Users who prefer Font Awesome icons with GPS accuracy
- **Accuracy:** High (GPS + IP fallback)
- **Compatibility:** Limited to GPS-friendly environments, includes PRISM Live support
- **Weather Icons:** Font Awesome icons with day/night variations
- **Use case:** Alternative styling for IRL Pro and apps requiring GPS precision

## Quick Setup

### For PRISM Live / OBS / Most Streaming Apps
**Japanese Google Weather Icons:** `https://mrchallah.github.io/iploc`
**Font Awesome Icons:** `https://mrchallah.github.io/classiciploc`

### For IRL Pro / GPS-Capable Apps
**Japanese Google Weather Icons:** `https://mrchallah.github.io/`
**Font Awesome Icons:** `https://mrchallah.github.io/classic`

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
- **Two Icon Styles Available** - Choose between Japanese Google weather icons or Font Awesome icons
- **Enhanced Weather Detection** - Uses multiple Open-Meteo parameters (wind speed, precipitation, visibility, temperature) for comprehensive condition analysis
- **Complete Weather Coverage** - Supports all weather conditions including:
  - Wind conditions (windy, wind with rain, blizzards)
  - All precipitation types (light/moderate/heavy rain, snow, mixed precipitation, hail)
  - Severe weather (thunderstorms, tornadoes, tropical storms)
  - Extreme conditions (very hot, very cold, icy conditions)
  - Special conditions (fog, dust, blowing snow)
- **Smart Weather Logic** - Temperature-based descriptions (shows "Sunny" instead of "Clear" when temperature > 27°C)
- **Day/Night Icon Variations** - Proper weather icons that change based on time of day
- **Reliable Fallback System** - Japanese Google weather icons automatically fall back to Google Maps icons if they fail to load
- **Current temperature** in both Celsius and Fahrenheit
- **Detailed weather descriptions** with accurate condition mapping
- **Powered by Open Meteo API** (no API key required)

### 🎭 Heat Wave & Wind Effects
- **Animated Heat Wave Indicator** - Shows when temperature exceeds regional thresholds
- **Animated Wind Indicator** - Displays during windy conditions (>18 km/h)
- **Smart Positioning** - Heat and wind effects position automatically based on combinations
- **Regional Heat Wave Detection** - Intelligent temperature thresholds based on geographic location

### 📱 Mobile & App Optimized
- Enhanced timeout settings for iOS devices
- Streaming app compatibility detection
- Mobile-specific GPS handling
- Responsive design for all screen sizes

## Weather Icon Systems

### 🎌 Japanese Google Weather Icons (Default)

**Primary choice for most users** - Beautiful distinctive Google Weather Icon designs

- **Premium Visual Experience** - Distinctive Google Weather Icon designs from official Google collection
- **Enhanced Weather Detection** - Advanced condition analysis using wind speed, precipitation, visibility, and temperature
- **Complete Weather Coverage** - Icons for all weather conditions including extreme weather, mixed precipitation, and severe storms
- **Automatic Fallback** - Seamlessly falls back to Google Maps icons if Google Weather Icons fail to load
- **Day/Night Variations** - Proper time-of-day specific icons for enhanced accuracy

### 🎨 Font Awesome Icons (Alternative)

**Alternative choice for different visual preference** - Clean, standardized Font Awesome weather icons

- **Consistent Font Awesome Style** - Uses familiar fa-sun, fa-cloud, fa-snowflake, etc. icons
- **Day/Night Icon Variations** - fa-sun/fa-moon for clear conditions, fa-cloud-sun/fa-cloud-moon for partial clouds
- **Enhanced Weather Mapping** - Comprehensive weather code mapping including:
  - Clear/Sunny: fa-sun (day) / fa-moon (night)
  - Partly Cloudy: fa-cloud-sun (day) / fa-cloud-moon (night)
  - Rain: fa-cloud-rain / fa-cloud-showers-heavy (heavy rain)
  - Snow: fa-snowflake for all snow conditions
  - Thunderstorms: fa-cloud-bolt
  - Fog: fa-eye-slash
- **Heat & Wind Effects Preserved** - Still includes animated heat wave (fa-water) and wind (fa-wind) indicators
- **No Fallback Needed** - Font Awesome icons load reliably from CDN

### 🌍 Comprehensive Weather Conditions

Both icon systems detect and display icons for:

#### 🌬️ **Wind Conditions**
- Windy conditions (wind speed > 18 km/h)
- Very windy conditions (wind speed > 35 km/h)
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

### IP-Only Versions
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

### GPS+IP Versions
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
2. Choose your preferred version:
   - **Japanese Google Weather Icons + IP**: `https://mrchallah.github.io/iploc`
   - **Font Awesome + IP**: `https://mrchallah.github.io/classiciploc`
   - **Japanese Google Weather Icons + GPS**: `https://mrchallah.github.io/`
   - **Font Awesome + GPS**: `https://mrchallah.github.io/classic`
3. Set width: 800, height: 600 (or as needed)
4. Check "Shutdown source when not visible" for performance

### Method 2: PRISM Live Overlay
1. Go to PRISM Live overlay settings
2. Add web overlay with URL (choose IP-only version):
   - **Japanese Google Weather Icons**: `https://mrchallah.github.io/iploc`
   - **Font Awesome**: `https://mrchallah.github.io/classiciploc`
3. Position as desired

### Method 3: IRL Pro Integration
1. Choose GPS version:
   - **Japanese Google Weather Icons**: `https://mrchallah.github.io/`
   - **Font Awesome**: `https://mrchallah.github.io/classic`
2. Allow location permissions when prompted
3. IRL Pro's GPS data will be automatically detected and used

## Configuration

### Location Refresh
All versions auto-refresh location data every 90 seconds to ensure current information while preserving performance.

### App Detection (IP-Only Versions)
The IP-only versions automatically detect streaming app environments and optimize accordingly:
- Skips GPS attempts in app environments
- Uses specialized PRISM Live location interfaces
- Falls back to multiple IP location services

### Enhanced Weather System
- **Two Icon Style Options** - Choose between Japanese Google Weather icons or Font Awesome icons
- **Multi-Parameter Detection** - Uses wind speed, precipitation, visibility, and temperature for accurate condition analysis
- **Comprehensive Coverage** - All Google Weather API condition types supported with appropriate icons
- **Smart Fallback System** - Japanese Google Weather icons versions have reliable icon loading with automatic fallback to Google Maps icons
- **Advanced Weather Logic** - Temperature-aware descriptions and extreme weather detection

## API Dependencies

### No API Keys Required!
All versions use free services:
- **Reverse Geocoding**: Google Maps API (with Nominatim fallback)
- **Weather**: Enhanced Open Meteo API with multi-parameter detection (wind_speed_10m, precipitation, visibility, temperature_2m, weather_code, is_day)
- **IP Location**: Multiple free services (Google, IP-API, IPInfo, IPAPI.co)
- **Weather Icons**: 
  - Japanese Google Weather Icon versions: Official Google Weather icons with default Google Map icons as fallback
  - Font Awesome versions: Font Awesome 6.5.0 from CDN

## Styling & Customization

### Visual Design
- Transparent background for overlay use
- White text with black shadow for maximum visibility
- Professional icon systems (Japanese Google Weather or Font Awesome)
- Responsive layout that works on any screen size
- Enhanced weather icons with drop shadows for better visibility

### Icons Used
- 🕒 Clock icon for time display
- 📍 Location dot for place information  
- 🎌 **Japanese Google Weather icons**: Dynamic Google Weather Icons that change based on conditions, time of day, and weather parameters
- 🎨 **Font Awesome**: Standard Font Awesome weather icons (fa-sun, fa-cloud, fa-snowflake, etc.) with day/night variations

## Browser Compatibility

### Supported Browsers
- Chrome/Chromium (recommended)
- Firefox
- Safari
- Edge
- Mobile browsers (iOS Safari, Chrome Mobile)

### Required Permissions
- **GPS Versions**: Location access required
- **IP Versions**: No permissions needed
- **All**: Internet connection required

## Troubleshooting

### Location Not Loading (IP Versions)
1. **Check internet connection**: Ensure network connectivity
2. **Try different browser**: Some corporate networks block location services
3. **Clear browser cache**: Refresh the page completely

### Location Not Loading (GPS Versions)  
1. **Check browser permissions**: Ensure location access is granted
2. **HTTPS required**: Modern browsers require HTTPS for GPS access
3. **Try IP version**: Use IP-only versions as fallback
4. **Indoor GPS issues**: GPS accuracy decreases indoors

### Weather Not Displaying
1. **Internet connectivity**: Verify network access
2. **Temporary service issue**: Weather API might be temporarily unavailable
3. **Refresh page**: Try reloading the overlay
4. **Icon fallback**: Japanese Google Weather icons automatically fall back to Google Maps icons if needed

### PRISM Live Issues
1. **Use IP version**: Make sure you're using IP-only versions
2. **Check overlay settings**: Ensure web overlay is properly configured
3. **Browser permissions**: Some versions require location permissions

## Recent Updates

### Font Awesome Icon Versions
- **Alternative Icon Style** - Added Font Awesome weather icon versions for users who prefer this style
- **Complete Feature Parity** - Font Awesome versions include all advanced features (heat waves, wind detection, regional thresholds)
- **Four Total Versions** - Now offering Japanese Google Weather icons and Font Awesome icon styles in both IP-only and GPS+IP variants
- **Day/Night Icon Support** - Font Awesome versions include proper day/night icon variations
- **Preserved Animations** - Heat wave and wind effect animations maintained in Font Awesome versions

### Major Weather System Features
- **Universal Japanese Google Weather Icons** - Beautiful Google Weather Icons as primary option
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
- Use IP versions for better stability during streams
- Position overlay in a corner to avoid content interference
- Test before going live to ensure proper functionality
- Weather icons now load more reliably with improved fallback system (Japanese Google Weather icons) or reliable CDN (Font Awesome)

### For Mobile IRL Streaming
- GPS versions work best with IRL Pro
- IP versions recommended for other mobile streaming apps
- Consider battery impact of GPS usage
- All users can choose between Japanese Google Weather or Font Awesome icons

## Version History & Updates

The overlays are automatically updated on the GitHub Pages hosting, so you'll always get the latest version by using the URLs above. Recent major updates include the universal Japanese Google Weather Icon system, comprehensive multi-parameter weather detection, and Font Awesome icon alternatives.

## License

This project is open source. Feel free to modify and distribute as needed.

## Contributing

Feel free to submit issues, feature requests, or pull requests to improve the overlay.

---

**Quick Reference:**
- **Maximum Compatibility (Japanese Google Weather Icons)**: `https://mrchallah.github.io/iploc`
- **Maximum Compatibility (Font Awesome)**: `https://mrchallah.github.io/classiciploc`
- **Maximum Accuracy (Japanese Google Weather Icons)**: `https://mrchallah.github.io/`
- **Maximum Accuracy (Font Awesome)**: `https://mrchallah.github.io/classic`
- **PRISM Live**: Use IP versions
- **IRL Pro**: Use GPS versions
- **OBS/XSplit**: Use IP versions  
- **Weather Icons**: Choose between Japanese Google Weather icons or Font Awesome icons
- **Weather Coverage**: Complete multi-parameter weather detection system 
