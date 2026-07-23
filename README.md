# DXCC Interactive World Map v3.4.0

An advanced, interactive world map designed specifically for amateur radio enthusiasts (HAM radio). This tool provides real-time tracking, geophysical data, satellite orbits, and DXCC entity visualization powered by the robust `dxccmap-v3` engine.

**Live Demo**
You can access the live application here: https://es7aaz.github.io/dxcc-map/

## Key Features

* **Interactive DXCC List:** Click on "DXCC" to toggle a searchable list of all DXCC entities with coordinates.
* **Advanced Search Engine:** Powered by a Cloudflare Worker utilizing the official `cty.dat` standard and the HamQTH.com JSON DXCC API for highly stable and accurate prefix, country, and callsign queries.
* **IBP Beacons:** Real-time visualization and tracking of International Beacon Project (IBP) stations across multiple bands.
* **Real-time Solar Data:**
  * **Day/Night Terminator:** Highly accurate solar terminator overlay.
  * **Sun Position:** Real-time tracking of the sun's position.
  * **WWV Alerts:** Hover over "WWV" to see the latest geophysical alerts, including SFI, Kp-index, and X-ray flux.
* **Azimuth & Distance Tools:**
  * **Manual & Auto QTH:** Set your home location via automatic browser geolocation (right-click the globe icon) or manually enter a **6-character Maidenhead locator** (grid square). Manual entries override geolocation and are saved in local storage.
  * Calculate azimuth and distance to any point on the map with a right-click.
* **Satellite & Aurora Tracking:** 
  * Built-in support for satellite tracking using the modern **OMM v3.0 JSON standard**.
  * **Live Transponder Data:** View metadata for active SAT transponders during the initial flyby phase.
  * **Weather Satellites (WX SAT):** Track 137-138 MHz NOAA (APT) and METEOR M2 (LRPT) series.
  * Aurora zone visualization.

## How to Use

* **Navigation:** Use the mouse wheel or double-click to zoom. Click and drag to move the map.
* **Reset View:** Press the 'R' key or left-click the globe icon to return to the default view.
* **Azimuth Marker:** Right-click anywhere on the map to place an azimuth marker.
* **Set Home QTH:** Enter your 6-character locator in the provided input field, or right-click the globe icon to use browser geolocation as the starting point for calculations.

## Technical Details

This static web application is built with modern, high-performance technologies:
* **D3.js & D3-geo** for high-performance map rendering.
* **Solar-calculator** for accurate astronomical calculations.
* **Satellite.js** for real-time orbital tracking.
* **Cloudflare Workers** acting as a secure, fast backend search engine.
* **Custom GeoJSON & cty.dat** for precise DXCC borders and entity locations.

## Credits & License

**Author:** Riho Bergmann, ES7AAZ  
Developed for the amateur radio community. If you find this tool useful, feel free to share it with your local radio club!

---

## Changelog

### v3.4.0
* **Code Refactoring:** CSS and JS have been completely separated from the HTML file, alongside various additional minor fixes.

### v3.2.0
* **Manual Home QTH:** Added an input field for a 6-character Maidenhead locator (with data validation). This allows manual placement of your home location on the map, overriding geolocation. The configured location is automatically saved in the browser's local storage.
* **Search Engine Upgrade:** The Cloudflare Worker has been updated to utilize the official `cty.dat` standard, ensuring much more stable and precise query results for prefixes, countries, and callsigns.
* **API Migration:** Callsign-based searches have been migrated to the HamQTH.com JSON DXCC API.

### v3.1.0
* **Core Engine Update:** The application is now powered by the new `dxccmap-v3` engine under the hood.
* **OMM v3.0 Standard:** Satellite orbital data has been transitioned to the modern OMM v3.0 JSON standard.
* **Transponder Metadata:** Metadata for active SAT transponders is now displayed during the initial phase of the flyby.
* **WX SAT Addition:** Added tracking for Weather Satellites, specifically the 137-138 MHz NOAA (APT) and METEOR M2 (LRPT) series.
* **Security Fix:** Eliminated an XSS vulnerability related to satellite table rendering.
