# Tide station data for Tideline (TRMNL plugin)

Static files read by the Tideline plugin for TRMNL:

- `stations.json`: every station the plugin can use. `t` = TICON-3 tide gauges `[lat, lon, nearest town]`, `r` = Rijkswaterstaat stations with an astronomical tide `[lat, lon, code, name]`, `n` = NOAA tide prediction stations `[lat, lon, id, name, harmonic]`.
- `s/{i}.json`: harmonic constants of TICON-3 station `i` (amplitude in cm, phase lag in degrees, UTC).

Sources and licences:

- TICON-3: Hart-Davis, M. G., Dettmering, D., Seitz, F. (2022). TICON-3: Tidal Constants based on GESLA-3 sea-level records from globally distributed tide gauges including gauge type information (data). PANGAEA, https://doi.org/10.1594/PANGAEA.951610, CC-BY-4.0.
- Town names: GeoNames (https://www.geonames.org), CC-BY-4.0.
- Station lists: Rijkswaterstaat Waterinfo (DD API) and NOAA CO-OPS.

Built with `data/build.py` in the plugin repository.
