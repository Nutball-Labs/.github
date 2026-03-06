# Nutball Labs
```
      / \__
     (    @\___
     /         O
    /   (_____/
   /_____/   U

      Nutball-Labs  Kali Approved, 2026
```

Small-shop C++ tooling for people who want to do something useful with their data.

---

## Projects
- Projects are currently set to Private while undergoing initial building.
  
### [PathMux](https://github.com/Nutball-Labs/PathMux)

CLI tool for Linux that works with dashcam footage, started with a Pruveeo D90 360° 4 channel.
Scans SD card directories, groups video segments into trips, caches manifests,
and extracts GPS tracks to GPX/KML/geojson for mapping or archiving.

- C++17 · CMake · AlmaLinux 9.x primary target
- Extracts LIGOGPSINFO GPS streams via ExifTool; outputs GeoJSON track files
- Batch tools: `pm_gpsinfo`, `pm_gpsexport`, `pm_findgpslock`, `pm_audit`, `pm_probe`
- Phase 2 (Qt6 viewer) planned

**Status:** Active CLI development — v0.9.x

---

### [SRoute](https://github.com/Nutball-Labs/SRoute)

Qt6 desktop application that turns a Strava activity into a shareable 4K video.
Pulls route data from the Strava API, matches geotagged photos to GPS trackpoints,
and renders a video with a progressively drawn moving map and split-screen photo moments.

- C++17 · Qt6 · CMake · AlmaLinux 9.x primary target
- Two render modes: tile-based (Mapbox/OSM) and abstract (route line only, no location context)
- ffmpeg linked directly — no subprocess; hardware encode via NVENC, QSV, VAAPI, or CPU
- GPL v3 / donationware

**Status:** Early development — scaffolding in progress

---

## Common Stack

Both projects share the same development conventions: C++17, CMake, AlmaLinux 9.x as the primary platform with Linux portability as a hard requirement, ffmpeg for media work, and metric-internal / display-toggleable unit handling.

---

*AlmaLinux 9.x · C++17 · CMake · ffmpeg · Qt6*
