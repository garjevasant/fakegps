# Fake GPS

> A clean Android GPS simulation tool for testing location-based apps without leaving your desk.

Fake GPS lets developers choose a point on the map, hold a simulated location, or drive a complete route with realistic movement, speed and bearing.

## What it does

- Pick any location from the map or search by place name and coordinates.
- Start and stop a fixed GPS mock from one control deck.
- Simulate a road trip between a start point, stops and a destination.
- Control trip duration, average speed or arrival time.
- Save favorite locations and reopen them quickly.
- Keep a history of fixed mocks and simulated routes.
- Switch between Auto, Streets, Minimal, Dark and Satellite map styles.
- Download offline map areas for saved places and routes.
- Use Android Quick Settings tiles and home-screen widgets.
- Open shared locations from Google Maps, OpenStreetMap, Waze and other map apps.

## Screenshots

Add screenshots here when the first production build is ready.

## Requirements

- Flutter 3.5 or newer
- Android Studio or Android SDK
- Android device or emulator
- Developer Options enabled

To use GPS mocking on a device, open:

`Settings → Developer Options → Select mock location app → Fake GPS`

## Run locally

```bash
git clone https://github.com/garjevasant/fakegps.git
cd fakegps
flutter pub get
flutter run
```

## Build an APK

```bash
flutter build apk --debug
```

For a signed production build, add your own `android/key.properties` and keystore, then run:

```bash
flutter build apk --release
```

Application ID:

```text
com.vasant.fakegps
```

## Free map services

Fake GPS uses keyless services from the OpenStreetMap ecosystem:

- Map styles: Immich Tiles and OpenFreeMap
- Satellite imagery: Esri World Imagery
- Search: Photon
- Routing: OSRM

Network services can be unavailable or rate-limited. The app always shows the current map and route state instead of pretending a request succeeded.

## Responsible use

Fake GPS is intended for software testing, development, privacy experiments in controlled environments and education. Location spoofing may violate the terms of service of games, transport, delivery, dating and other services. Use it legally and responsibly.

## Project

- Repository: https://github.com/garjevasant/fakegps
- Issues: https://github.com/garjevasant/fakegps/issues
- Releases: https://github.com/garjevasant/fakegps/releases

## Contributors

- Garje Vasant

## License

This project is released under the MIT License. See [LICENSE](LICENSE).

