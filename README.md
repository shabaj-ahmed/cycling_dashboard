# cycling_dashboard
The Cycling Dashboard is a companion Flutter application that connects to the [cycling computer](https://github.com/shabaj-ahmed/cycling-computer) to display sensor data in real time. While the cycling computer operates fully offline, the dashboard provides a user-friendly interface for visualising ride metrics and monitoring device status.

The app connects to the cycling computer via Bluetooth and provides cyclists with real-time performance data, sensor connection indicators, and ride history. It is designed to be lightweight, responsive, and operable on both iOS and Android devices.

A companion mobile app connected via Bluetooth was chosen over a dedicated LCD display or Wi-Fi connectivity to balance usability, reliability, and practicality. A built-in LCD increases hardware complexity and introduces more potential points of failure in outdoor environments. Wi-Fi, while capable of high data throughput, would prevent the rider’s phone from maintaining an internet connection, something many cyclists rely on for safety, navigation, and communication during rides. Since riders almost always carry a phone, leveraging it as the primary display provides a more robust, extensible, and user-friendly solution without compromising connectivity.

# System Requirements
This section outlines the requirements for the Cycling Dashboard, divided into User Requirements (URs), Functional Requirements (FRs), and Non-Functional Requirements (NFRs).

## User Requirements
### Core Functionality
- UR1: As a user, I want to see real-time cycling metrics (speed, cadence, heart rate, distance, elevation, ride duration) so I can monitor my performance.
### Device Operation & Control
- UR2: As a user, I want clear indicators of device/sensor status (connected, disconnected, error).
- UR3: As a user, I want to configure device settings (e.g., preferred units, display preferences).
- UR4: As a user, I want notifications when a ride starts or stops recording.
### Data Logging
- UR5: As a user, I want all ride data to be stored locally on my phone so I can review past sessions.
### Environment & Usability
- UR6: As a user, I want the dashboard interface to be clean and usable while riding.
- UR7: As a user, I want the app to work offline so I can use it without internet access.
- UR8: As a user, I want the UI to adapt for outdoor readability (dark/light themes).

## Functional Requirements
## Data Handling
- FR1: The app shall connect to the cycling computer via Bluetooth.
- FR2: The app shall receive and display real-time data (speed, cadence, HR, GPS position, elevation).
- FR3: The app shall store ride session data in a local database.
- FR4: The app shall timestamp received data using system time for consistency.
### User Interface
- FR5: The app shall display data on customizable dashboard screens (numeric view, graph view).
- FR6: The app shall show sensor/device connection status indicators.
- FR7: The app shall notify the user (visual/audio/vibration) when the device connects or disconnects.
- FR8: The app shall allow switching between metric and imperial units.
### Settings & Control
- FR9: The app shall automatically reconnect to the cycling computer if the connection is lost.

## Non-Functional Requirements
### Performance
- NFR1: The dashboard shall display incoming data with a latency below 500 ms.
- NFR2: The app shall support at least 3 hours of continuous operation without significant performance degradation.
### Usability
- NFR3: The UI shall be responsive and adapt to different phone screen sizes and orientations.
- NFR4: The app shall provide outdoor-readable colour themes (light and dark).
- NFR5: The app shall support one-handed operation for use during riding.
### Reliability & Safety
- NFR3: The UI shall be responsive and adapt to different phone screen sizes and orientations.
- NFR4: The app shall provide outdoor-readable colour themes (light and dark).
- NFR5: The app shall support one-handed operation for use during riding.
### Maintainability & Extensibility
- NFR9: The app shall allow easy integration of new data fields and sensors without refactoring core modules.
- NFR10: The app shall be open-source and include developer documentation for community contributions.
