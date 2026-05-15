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
  
### [CamClops](https://github.com/Nutball-Labs/CamClops)

Desktop GUI + CLI toolset for organizing dashcam footage into trips, extracting GPS tracks,
and building synchronized multi-camera 4K videos. Started with a Pruveeo D90 360° 4 channel.

- C++17 · Qt6 · CMake · AlmaLinux 9.x primary target; Linux/macOS/Windows
- Qt6 GUI: manifest browser, trip grid, collage builder, GPS export, moving map, instrument dashboard, HUD overlay
- CLI tools: `clops_probe`, `clops_gpsinfo`, `clops_gpsexport`, `clops_audit`, `clops_ls`, `clops_videos`
- `camclops-tl` timelapse editor for variable-speed clip creation

**Status:** Active development — v2.0.1a · Phase 1 (CLI) feature-complete · Phase 2 (Qt6 GUI) shipping

---

### [SRoute](https://github.com/Nutball-Labs/SRoute)

- SRoute project set to Private while undergoing initial building.

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

---

## Socials

- [Facebook](https://www.facebook.com/profile.php?id=61582196172416)
