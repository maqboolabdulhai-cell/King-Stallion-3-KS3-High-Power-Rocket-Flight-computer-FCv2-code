FCv2 Rocket Flight Computer

FCv2 is a custom ESP32-based flight computer designed for high-power model rockets. It combines onboard flight logging, wireless monitoring, inertial navigation, and recovery deployment control into a compact avionics package.

The system uses a BMP280 barometric sensor for altitude tracking and an ICM-20948 9-axis IMU for orientation sensing and flight analysis. Flight data is continuously logged to a microSD card for post-flight review.

Features
ESP32-based flight computer
BMP280 altitude sensing
ICM-20948 9-axis IMU
MicroSD flight data logging
Integrated Wi-Fi configuration and monitoring interface
Live telemetry display through a web dashboard
Automatic launch detection
Automatic apogee detection
Main parachute deployment control
IMU calibration through the web interface
Multiple pyro output channels for recovery and staging events
Status LEDs, buzzer feedback, and physical arming key support
Safety Systems

FCv2 includes multiple layers of flight protection to reduce the risk of accidental deployment or false launch detection:

Physical key-switch arming system
Independent armed-status indicator LED
Audible arming and disarming feedback
Launch detection requires acceleration, altitude, and velocity thresholds to be met simultaneously
Apogee detection uses both altitude and vertical velocity confirmation
Main parachute deployment only occurs after apogee has been detected and descent has begun
Automatic disarming after flight timeout
Deployment event confirmation and timing safeguards
Ground-test functions accessible through the web interface for pre-flight verification
Data Logging

During flight, FCv2 records:

Timestamp
Barometric pressure
Altitude
Accelerometer data
Gyroscope data
Calculated vertical velocity
Flight event status

All flight data is stored locally on a microSD card for later analysis.

Project Status

🚧 Active Development

Disclaimer

This project is experimental and intended for educational and hobby rocketry purposes. All recovery systems and deployment electronics should be thoroughly ground-tested before flight. The author assumes no responsibility for damage, injury, or loss resulting from the use of this project.
