# Global Angler

Offshore fishing game and live weather app for Android — fish 19 spots
around the world with real forecast, swell, and tide data.

## Play it

Open `Global_Angler.html` in any modern browser, or build the Android app
from `android/` (see below). No account, no sign-up.

## What it is

Pick a fishing spot, cast a line, and reel in fish — with live conditions
for the spot you are fishing:

- **19 fishing locations** around the world, from the Amazon River to the
  Florida Keys.
- **Live forecast** from Open-Meteo: temperature, wind, and weather for the
  spot you pick.
- **Live swell and waves** from the Open-Meteo Marine API.
- **Real tides** from NOAA CO-OPS for the Florida Keys (Key West station
  8724580). Other spots show no mapped tide station rather than estimated
  tides.
- **Honest fallbacks:** if live data is unavailable the app says so and
  shows an "Offline estimate" instead of pretending the data is live.

## Gameplay

Casting and reeling with a power meter, bite windows, and a streak system.
Boats and a fleet to upgrade, an aquarium to fill, tournaments, quests,
achievements, a workbench for crafting, and a sonar to find the fish.

## Data sources

- Forecast and marine data: [Open-Meteo](https://open-meteo.com/)
- Tides: [NOAA CO-OPS](https://tidesandcurrents.noaa.gov/)

The app sends only the preset coordinates of the fishing spot you pick to
these services to fetch the weather. It does not access your device's live
location and collects no personal data. See
[Privacy Policy](https://mrnomaguow.github.io/global-angler/privacy-policy.html).

## Donate

Global Angler is free and open source. The Donate button in the app shows a
PayPal QR code for the developer.

## Android app

`android/` is the Android (Gradle) project that wraps the HTML in a WebView.
Package `com.livewire.globalangler`, version 1.0.1. Build it with
`./gradlew assembleRelease` (requires Android SDK 36 and JDK 17).

## License

Apache License 2.0 — see `LICENSE`. Copyright 2026 Elijah Wougamon.
