# Start_Hack_Jfl

**JFL Solar** is our START Hack 2023 project. We were the top team in the Energy category of the Google track.

The app puts the solar power potential of anywhere on Earth onto Google Maps, next to what electricity costs there.

![Solar potential layer](media/solar-world.jpg)

![Europe close-up](media/solar-europe.jpg)

## What's in here

- `jfl-solar/` is the web app (Next.js, React, TypeScript, Google Maps).
- `jfl-solar/public/files/` holds the solar potential layer: the Global Solar Atlas photovoltaic output (PVOUT) map cut into 28,000+ map tiles across zoom levels 0 to 8. Each tile is a PNG with a KML file giving its bounds.
- `jfl-solar/src/app/tariff.js` matches a location to its country via reverse geocoding, then looks up electricity prices per kWh for 30 countries.

The screenshots above are stitched from the tiles in `jfl-solar/public/files` (zoom 4 for the world, zoom 6 for Europe).

Solar data: [Global Solar Atlas](https://globalsolaratlas.info/), published by the World Bank Group, funded by ESMAP and prepared by Solargis.
