# Dreamscape F722
Dreamscape F722 is an open-hardware STM32-based flight controller designed for FPV and custom drone platforms. It targets high-performance firmware such as Betaflight, iNav, and ArduPilot while remaining developer-friendly for experimentation and customization. The design focuses on a powerful MCU, robust connectivity, and support for a wide range of peripherals to enable advanced flight control features and future expansion.

# Features
## MCU
- STM32 F722RET6
- 32-bit ARM Cortex-M7 CPU
- Up to 216 MHz clock speed
- Large memory for advanced firmware features
- Compatible with Betaflight/iNav/ArduPilot

## Power System
- 5V input with built-in 3.3v regulator
- Power distribution for peripherals
- USB Power support
- Protection for USB

## Connectivity
- USB Type-C for programming and communication
- Multiple UART ports for telemetry and peripherals
- I2C bus for sensors and accessories
- SPI interface for high-speed communication
- SWD debugging port

## Sensors
- ICM-42688-P 6-axis IMU (3-axis gyroscope + 3-axis accelerometer) via SPI for precise flight control and low latency
- BMP280 barometer for altitude sensing
- Optional external sensor support via I2C

## Flight Control Outputs
- 8 PWM outputs
- Supports DSHOT, Oneshot, and standard PWM protocols
- Compatible with individual ESCs or 4-in-1 ESCs

## Radio / Receiver Support
- CRSF (Crossfire) support for long-range control
- SBUS support for standard RC receivers
- PPM support for legacy receivers
- Support for external radio modules via UART

## Status & Indicators
- Power LED
- User LED
- Boot/Status LED

## Expansion & Peripherals
- GPS module support via UART
- Telemetry Radios
- VTX control (SmartAudio or Tramp)
- Buzzer for audible alerts
- Camera control
- External sensor support (e.g., magnetometer, external barometer)

## Physical Design
- Compact flight-controller form factor (30x30mm)
- Standard mounting pattern
- Designed for custom drones

## Development Friendly
- Open-source hardware design files
- Open-source firmware support (Betaflight, iNav, ArduPilot)
- Easy debugging with SWD port

## Planned Future Features
- Integrated ELRS receiver
- Dual-Band telemetry support
- Advanced Sensor suite
- Power monitoring improvements
- Integrated OSD support

# Specifications
## Core Specifications
### MCU
- MCU: STM32 F722RET6
- Architecture: ARM Cortex-M7
- Clock Speed: Up to 216 MHz
- Flash Memory: 512 KB
- RAM: 256 KB
- Hardware Floating Point Unit (FPU)

### Inertial Measurement Unit (IMU)
- IMU: ICM-42688-P
- HIgh-speed SPI bus for low latency
- Optimied placement for reduced vibration noise

### Power System
- Input Voltage: 5V (via USB or power distribution)
- Built-in 3.3V regulator for peripherals
- USB Power support with protection
- Power distribution for connected peripherals

## I/O and Connectivity
### UART Ports
- UART1: Receiver 
- UART2: GPS module
- UART3: Telemetry
- UART4: VTX Control
- UART5: Reserved for future expansion

### SPI Interfaces
- SPI1: IMU (ICM-42688-P)
- SPI2: Reserved for future sensor expansion

### I2C Bus
- I2C bus available for peripherals such as magnetometers, external barometers, etc.

### SWD
- SWD header for debugging and firmware development

## Motor Outputs
- Up to 8 PWM outputs
- Suppored Protocols:
  - DShot150/300/600
  - OneShot
  - Multishot
  - Standard PWM
  - Compatible with individual ESCs or 4-in-1 ESCs

## Receiver Support
- CRSF (Crossfire) support for long-range control
- SBUS support for standard RC receivers
- PPM support for legacy receivers
- Support for external radio modules via UART

## Additional Peripherals
- Buzzer output
- LED Strip output
- Camera control
- VTX control (SmartAudio or Tramp)

## Status Indicators
- Power LED
- User LED
- Boot/Status LED

## Physical Dimensions
- Size: 30x30mm
- Board Layers: 4
- PCB Thickness: 1.6mm
- Copper Weight: 1oz
- Dimensions: Standard flight controller mounting pattern

## Firmware Compatibility
- Designed for compatibility with Betaflight, iNav, and ArduPilot
- Open-source firmware support for customization and development

## Development Features
- Open Hardware design
- Full SWD debugging support
- Compatible with ST-Link Programmers
- Designed for experimentation and customization

## Planned Future Features
- Integrated ELRS receiver for long-range control
- Dual-Band telemetry support for improved communication
- Advanced Sensor suite including magnetometer and external barometer support
- Integrated ESC for AIO support
- Integrated OSD support for on-screen display of flight information
- Improved powwer monitoring with current sensing and voltage monitoring

# Firmware Building
````bash
cd ~/Dreamscape-F722/firmware/betaflight/betaflight
make configs
make DREAMSCAPEF722
````

# Blender Render:
![BlenderRender](blender/Untitled.png)
![Purple](blender/Purple.png)

# Schematics & PCB view
![Schematic](images/Schematic.jpg)
![Schematic1](images/Schematic1.jpg)
![PCB](images/PCB.jpg)
![PDF](images/Schematic.pdf)

# prices
![Cart](images/jlcpcb/jlcpcb_cart.png)
# LCSC (Hand Soldering)
![LCSC1](images/jlcpcb/lcsc_1.png)
![LCSC2](images/jlcpcb/lcsc_2.png)
![LCSC3](images/jlcpcb/lcsc_3.png)
![LCSC4](images/jlcpcb/lcsc_4.png)
![LCSC5](images/jlcpcb/lcsc_5.png)
![LCSC6](images/jlcpcb/lcsc_6.png)
