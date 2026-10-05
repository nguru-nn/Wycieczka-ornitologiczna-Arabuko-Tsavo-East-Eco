# Diani Beach → Arabuko Sokoke Forest & Tsavo East: 3-Day Safari Map
 
This is an interactive 3D map of a 3-day safari from **Diani Beach** that combines coast and bush. The route heads north along Kenya's coast to the **Arabuko Sokoke Forest**, the largest remaining coastal forest in East Africa and a well-known birdwatching site. It then enters **Tsavo East National Park** through the remote **Sala Gate** and follows the Galana River inland to Voi.
 
🗺️ **See the full itinerary and the live map:**
[Arabuko Sokoke i Tsavo East](https://safarikenia.com.pl/arabuko-sokoke-i-tsavo-east) on **Safari Kenia**
 
---
 
## The route
 
| Day | Destination | Accommodation / Highlight |
|-----|-------------|---------------------------|
| Start | Departure from Diani Beach | — |
| Day 1 | Arabuko Sokoke Forest | Birdwatching stop |
| Day 1 | Start of the safari | Doa Doa Safari Camp |
| Day 2 | Tsavo East National Park | Voi Wildlife Lodge |
| Day 3 | Return to Diani Beach | — |
 
**Day 1, up the coast:** Diani Beach → Likoni Ferry → Mombasa → Nyali → Mtwapa → Kilifi Bridge → Arabuko Sokoke Forest
**Day 2, across Tsavo East:** Marafa turn-off → Sala Gate → Galana River → Ashaka → Voi
**Day 3, back to the coast:** Voi → Mariakani → Mombasa → Likoni Ferry → Diani Beach
 
The trip is a full loop: north along the coast, west through the park and back down the Mombasa highway. The interface labels are in Polish, matching the tour page it's embedded on.
 
## Features
 
- **Coast-to-bush loop.** The route covers the Indian Ocean coastline, the Kilifi creek crossing, coastal forest and the Tsavo East plains, so every leg is distinct and none is driven twice.
- **Entry through Sala Gate.** Waypoints follow the less-travelled eastern entrance to Tsavo East and the Galana River, rather than the usual Voi-side approach.
- **Satellite basemap with 3D terrain.** The map uses the Mapbox Standard Satellite style with DEM terrain at 1.5× exaggeration and a tilted camera.
- **Road-accurate route.** Each leg is fetched from the Mapbox Directions API (driving profile) and stitched into one line. If a request fails, the leg falls back to a straight segment.
- **Animated route line.** A golden "marching ants" dashed line runs over a soft glow layer.
- **Interactive itinerary panel.** A glassmorphism sidebar lists each stop. Clicking a card flies the camera there and opens its popup.
- **Custom markers.** Gold SVG pins mark the main stops. Hidden waypoints shape the route without cluttering the map.
- **Mobile-friendly.** On small screens the sidebar becomes a bottom sheet, and cooperative gestures keep page scrolling smooth.
- **WordPress-ready.** Styles are scoped to a single container, so the code can be pasted into a Custom HTML block.
## Tech stack
 
- [Mapbox GL JS](https://docs.mapbox.com/mapbox-gl-js/) v3.9.0
- [Mapbox Directions API](https://docs.mapbox.com/api/navigation/directions/)
- Vanilla JavaScript, no build step
- Plus Jakarta Sans (Google Fonts)
## Usage
 
1. Copy the HTML into a WordPress **Custom HTML** block or any web page.
2. Replace the Mapbox access token with your own and restrict it to your domain in your [Mapbox account](https://account.mapbox.com/access-tokens/).
3. Adjust the container height in `.wp-safari-itinerary-container` to fit your layout.
To change the route, edit the `itineraryData` array. Entries with `isWaypoint: true` shape the route only. All other entries get a marker and a sidebar card.
 
## About
 
Built for [Safari Kenia](https://safarikenia.com.pl/), a Polish-language site offering safari tours and travel guides for Kenya.
 
➡️ [View this Arabuko Sokoke & Tsavo East itinerary](https://safarikenia.com.pl/arabuko-sokoke-i-tsavo-east)
