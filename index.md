<p align="center">
  <img src="https://smokestack.magnolialogic.net/img/3D.png" width=480/><br>
  <img src="https://smokestack.magnolialogic.net/img/smoker.png" width=480/>
</p>

<br>

**Note:** This repository tracks version 2.0 (SwiftUI app, Vapor backend) which is a work in progress, for version 1 (UIKit app, Google Firebase backend) please see [smokestack-legacy](https://www.github.com/magnolialogic/smokestack-legacy)<br><br>

## Components
[smokestack-core](https://github.com/magnolialogic/smokestack-core): Swift Package with shared data model for iOS app and Vapor backend<br>
[smokestack-app](https://github.com/magnolialogic/smokestack-app): SwiftUI 3.0 app, requires iOS 15.2+<br>
[smokestack-vapor](https://github.com/magnolialogic/smokestack-vapor): Vapor backend/services, supports macOS and Linux (via docker-compose)<br>
[smokestack-firmware](https://github.com/magnolialogic/smokestack-firmware): Python smoker firmware for Raspberry Pi<br>
[smokestack-3D](https://github.com/magnolialogic/smokestack-3D): 3D-printable parts for the controller box<br><br>

## Technologies
iOS app:
- SwiftUI, Swift 5.5
- Supports light + dark mode
- Apple Associated Domain (allows password autofill)
- Sign In With Apple
- Handles WebSocket/APNS messages from Vapor backend<br><br>

Backend:
- Vapor 4.0, Swift 5.5
- Redis
- REST endpoints for iOS app and smoker firmware
- Uses APNS/WebSocket to send messages to iOS app (WebSocket when app is foregrounded, APNS when app is backgrounded)<br><br>

Firmware:
- Python3
- Uses MAX31855 (thermocouple) and MAX31855 (RTD) drivers to read temperatures
- Uses relays to control smoker's igniter, auger, and fan
- Uses HTTP requests to interact with Vapor backend<br><br>

## Screenshots
<p align="center">
  <img src="https://smokestack.magnolialogic.net/img/running.png" alt="Running" width=240/>
  <img src="https://smokestack.magnolialogic.net/img/hero_dark.png" alt="Dark mode" width=240/><br>
  <img src="https://smokestack.magnolialogic.net/img/SIWA.png" alt="Sign In With Apple" width=240/>
  <img src="https://smokestack.magnolialogic.net/img/landing_page.png" alt="Landing Page" width=240/><br>
  <img src="https://smokestack.magnolialogic.net/img/setup.png" alt="Setup" width=240/>
  <img src="https://smokestack.magnolialogic.net/img/settings.png" alt="Settings" width=240/>
</p>
