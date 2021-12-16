# smokestack

Add "smart" control to your "dumb" Traeger smoker.

This repository tracks version 2.0 (SwiftUI app, Vapor REST/WebSocket backend), for version 1 (UIKit app, Google Firebase backend) please see [smokestack-legacy](https://www.github.com/magnolialogic/smokestack-legacy)

### Components
[smokestack-core](https://github.com/magnolialogic/smokestack-core): Swift Package with shared data model for iOS app and Vapor backend
[smokestack-app](https://github.com/magnolialogic/smokestack-app): SwiftUI 3.0 app, requires iOS 15.2+
[smokestack-vapor](https://github.com/magnolialogic/smokestack-vapor): Vapor backend/services, supports macOS and Linux (via docker-compose)
[smokestack-firmware](https://github.com/magnolialogic/smokestack-firmware): Python smoker firmware for Raspberry Pi
[smokestack-3D](https://github.com/magnolialogic/smokestack-3D): 3D-printable parts for the controller box
