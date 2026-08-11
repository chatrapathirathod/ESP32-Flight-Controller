ESP32 Custom Flight Controller

A custom-built ESP32-based flight controller designed from scratch for learning and experimentation with embedded systems, PCB design, sensor fusion, PID control, and quadcopter flight control.

Project Status

Current status: Flying successfully 🚁


ESP32-based flight controller

Custom-designed PCB

MPU6500 IMU

BMP280 barometer

HMC5883L magnetometer

FlySky iBUS receiver

PWM ESC output
PID-based stabilization
Custom Quad-X mixer
Successfully tested in flight
Hardware
Component	Details
MCU	ESP32
IMU	MPU6500
Barometer	BMP280
Magnetometer	HMC5883L
Receiver	FlySky iBUS
ESC protocol	PWM
Motors	A2212 1400KV
Battery	3S LiPo
Frame	F450
Propellers	8×4.5
Custom PCB







Architecture
             ┌──────────────────┐
             │      ESP32       │
             │                  │
             │  Flight Control  │
             └────────┬─────────┘
                      │
       ┌──────────────┼──────────────┐
       │              │              │
    MPU6500         BMP280       HMC5883L
       │              │              │
       └──────────────┼──────────────┘
                      │
                 PID Controller
                      │
                   Mixer
                      │
             ┌────────┴────────┐
             │                 │
           ESC 1             ESC 4
             │                 │
           Motor             Motor














           
Current Limitations

 This makes the project look more professional, not less.

For example:

No production-grade filtering yet
Altitude hold still under development
VL53L0X not currently integrated into ESP-FC firmware
GPS navigation not yet implemented
Further PID tuning required
Prototype PCB intended for educational/hobby use
Future Work
 Altitude hold using BMP280
 VL53L0X rangefinder integration
 Soft landing controller
 GPS integration
 Position hold
 Improved filtering
 STM32-based second-generation FC
 Custom PCB revision 2
