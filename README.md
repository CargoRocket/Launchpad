<div align="center">
  <img src="https://cologne.xatellite.io/logo-pfade.svg" alt="Logo" height="100px" />

  [DEPRECATED] CargoRocket Launchpad
  ---
</div>

> This prototype was developed during MobiData BW Hackathon 2021 and is no longer maintained or up to date. It will be replaced by our new CargoRocket App/Backend which is developed during our 3 month funding phase.

A cargo bike routing client using  Mapbox GL Directionsan and custom graphhopper routing service.

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