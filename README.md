# HuntCofC

A campus scavenger-hunt app for the College of Charleston, built as a team project for CSCI 360.

Open the map, walk to a campus landmark, and claim its badge once you are physically close enough. A leaderboard on the home screen ranks the top explorers by badges earned.

## Features

- **Map** of campus locations with your live position, built on `react-native-maps` and `expo-location`
- **Badges** you can only claim when you are within range of a location (distance is checked on the device)
- **Home screen** listing locations, plus a "Top Explorers" leaderboard
- **Accounts** with email and password through Firebase Authentication; badges are stored in Cloud Firestore
- **Tests** for the main screens with Jest and React Native Testing Library

## Tech

Expo SDK 52, React Native 0.76, TypeScript, expo-router, Firebase (Authentication and Cloud Firestore), Jest.

## Repository layout

| Path | What it is |
|---|---|
| `HuntCofC/` | The Expo app |
| `HuntCofC/app/(tabs)/` | The three screens: Home, Map and Account |
| `HuntCofC/utils/locationBadges.ts` | Distance check and badge awarding |
| `Unit Test Code D7/` | Unit tests submitted for deliverable 7 |
| `*.pdf`, `D7.drawio.png` | Course deliverables: use cases, domain model, design documents and diagrams |

## Status

This was a semester project and is not maintained. The app expects a Firebase project; the one used during the course may no longer be available, so you would need to supply your own configuration in `HuntCofC/firebaseConfig.ts`.

## Team

Built by Aidan McKittrick ([@McKaidan26](https://github.com/McKaidan26)) and Kev Brigham ([@kev-devmethod](https://github.com/kev-devmethod)). This repository is a fork of the original team repository, [kev-devmethod/HelloWorldCSCI360](https://github.com/kev-devmethod/HelloWorldCSCI360).

## License

MIT. See [LICENSE](LICENSE).
