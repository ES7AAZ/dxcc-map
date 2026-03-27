# DXCC Interactive World Map v2.7.5.0

An advanced, interactive world map designed specifically for amateur radio enthusiasts (HAM radio). This tool provides real-time tracking, geophysical data, and DXCC entity visualization.

## Live Demo
You can access the live application here:
[https://es7aaz.github.io/dxcc-map/](https://es7aaz.github.io/dxcc-map/)

## Key Features
* **Interactive DXCC List:** Click on "DXCC" to toggle a searchable list of all DXCC entities with coordinates.
* **IBP Beacons:** Real-time visualization and tracking of International Beacon Project (IBP) stations across multiple bands.
* **Real-time Solar Data:**
    * **Day/Night Terminator:** Highly accurate solar terminator overlay.
    * **Sun Position:** Real-time tracking of the sun's position.
    * **WWV Alerts:** Hover over "WWV" to see the latest geophysical alerts, including SFI, Kp-index, and X-ray flux.
* **Azimuth & Distance Tools:**
    * Set your home location via geolocation (right-click the globe icon).
    * Calculate azimuth and distance to any point on the map with a right-click.
* **Satellite & Aurora:** Built-in support for satellite tracking and aurora zone visualization.

## How to Use
* **Navigation:** Use the mouse wheel or double-click to zoom. Click and drag to move the map.
* **Reset View:** Press the **'R'** key or left-click the globe icon to return to the default view.
* **Azimuth Marker:** Right-click anywhere on the map to place an azimuth marker.
* **Geolocation:** Right-click the globe icon to set your current location as the starting point for azimuth/distance calculations.

## Technical Details
This is a static web application built with:
* **D3.js** & **D3-geo** for high-performance map rendering.
* **Solar-calculator** for accurate astronomical calculations.
* **Satellite.js** for real-time orbital tracking.
* Custom **GeoJSON** data for precise DXCC borders and entity locations.

## Credits & License
**Author:** Riho Bergmann, **ES7AAZ**

Developed for the amateur radio community. If you find this tool useful, feel free to share it with your local radio club!
