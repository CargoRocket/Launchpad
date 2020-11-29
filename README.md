CargoRocket Launchpad - using Mapbox GL Directions
---

A cargo bike routing client using a custom graphhopper routing service.

### Usage

```javascript
var mapboxgl = require('mapbox-gl');
var MapboxDirections = require('@mapbox/mapbox-gl-directions');

var directions = new MapboxDirections({
  accessToken: 'YOUR-MAPBOX-ACCESS-TOKEN',
  unit: 'metric',
  profile: 'mapbox/cycling'
});

var map = new mapboxgl.Map({
  container: 'map',
  style: 'mapbox://styles/mapbox/streets-v9'
});

map.addControl(directions, 'top-left');
```

Live example: https://launchpad.xatellite.io