# Daylight Atlas

A single-page web app showing sunrise, sunset and daylight length for any place in the world.

- Defaults to your current location; search by place name or type coordinates (`59.44, 24.75`)
- Selected-day view with the change vs. the previous day (DST clock jumps called out)
- Year view at day / week / month precision: daylight band chart, trend chart, calendar heatmap, table
- Times shown in the location's own time zone; handles polar day and polar night

Sun positions are computed in the browser (NOAA/Meeus approximations, ±1 min). Place search uses
[Open-Meteo](https://open-meteo.com/) geocoding; reverse geocoding uses OpenStreetMap Nominatim.

## Run

```sh
python3 -m http.server
```

Then open http://localhost:8000 (geolocation needs localhost or https).
