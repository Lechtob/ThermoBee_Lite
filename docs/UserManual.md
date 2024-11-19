# ThermoBee Lite User Manual

## Table of Contents

1. [Introduction](#introduction)
2. [Safety Information](#safety-information)
3. [Hardware Assembly](#hardware-assembly)
4. [Firmware Upload](#firmware-upload)
5. [Enclosure Assembly](#enclosure-assembly)
6. [Installation and Setup](#installation-and-setup)
7. [Home Assistant Integration](#home-assistant-integration)
8. [Troubleshooting](#troubleshooting)
9. [Maintenance](#maintenance)
10. [Specifications](#specifications)
11. [Support](#support)

---

## Introduction

Thank you for choosing ThermoBee Lite! This user manual will guide you through the assembly, setup, and usage of your new ZigBee sensor device.

## Safety Information

- Handle electronic components with care to avoid damage from static electricity.
- Keep the device away from water and extreme temperatures.
- Use the recommended batteries and ensure correct polarity.

## Hardware Assembly

### Components Required

- **Printed Circuit Board (PCB)**
- **Microcontroller** (as specified in the BOM)
- **Sensors**: Temperature/Humidity sensor, Air Quality sensor
- **Passive Components**: Resistors, capacitors, etc.
- **Battery Holder**
- **LED Indicator**
- **Programming Header** (optional)

### Tools Needed

- Soldering iron and solder
- Tweezers
- Multimeter (optional for testing)

### Assembly Steps

1. **Prepare the Workspace**: Ensure you have a clean, well-lit workspace.

2. **Place Small Components**:
   - Start with the smallest components like resistors and capacitors.
   - Use tweezers to place them accurately on the PCB.

3. **Solder the Microcontroller**:
   - Carefully align the microcontroller pins with the PCB pads.
   - Solder the corners first, then proceed to the remaining pins.

4. **Attach Sensors**:
   - Solder the temperature/humidity sensor.
   - Solder the air quality sensor.

5. **Install the Battery Holder**:
   - Secure the battery holder onto the PCB.

6. **Add the LED Indicator**:
   - Ensure correct orientation (check the datasheet for polarity).

7. **Inspect Solder Joints**:
   - Verify all connections are secure and free of shorts.

## Firmware Upload

### Requirements

- **Programmer**: e.g., J-Link, ST-Link, or equivalent compatible with your microcontroller.
- **Firmware Binary**: Download from the [firmware releases](https://github.com/yourusername/ThermoBeeLite/releases).

### Steps

1. **Connect the Programmer**:
   - Attach the programmer to the programming header or pads on the PCB.

2. **Install Programming Software**:
   - Use software compatible with your programmer (e.g., SEGGER J-Flash).

3. **Upload the Firmware**:
   - Open the firmware binary in the programming software.
   - Follow the software instructions to flash the firmware onto the microcontroller.

4. **Verify Installation**:
   - Confirm that the device powers on and the LED indicator behaves as expected.

## Enclosure Assembly

### Printing the Enclosure

- **Download STL Files**: Available in the [enclosure STL files directory](../enclosure/STL-Files/).
- **3D Printing**: Use a 3D printer to print the top and bottom parts.
  - **Material Recommendation**: PLA or ABS.

### Assembly Steps

1. **Prepare Printed Parts**:
   - Remove any support material.
   - Smooth edges if necessary.

2. **Insert the PCB**:
   - Place the assembled PCB into the bottom part of the enclosure.
   - Ensure sensors are properly aligned with any openings.

3. **Attach the Top Cover**:
   - Align the top part and press gently until it snaps into place.
   - If screws are used, secure them accordingly.

4. **Battery Installation**:
   - Insert the battery into the holder, ensuring correct polarity.

## Installation and Setup

### Placing the Device

- **Optimal Location**: Place the ThermoBee Lite in an area where you wish to monitor environmental conditions.
- **Avoid Obstructions**: Ensure the device is not blocked by large objects that may interfere with sensor readings or signal transmission.

### Powering On

- After inserting the battery, the device should power on automatically.
- The LED indicator may flash to indicate startup.

## Home Assistant Integration

### Adding the Device

1. **ZigBee Coordinator**:
   - Ensure your ZigBee coordinator is up and running with Home Assistant.

2. **Pairing Mode**:
   - If the device doesn't automatically enter pairing mode, press the pairing button (if available) or follow the firmware instructions.

3. **Home Assistant Configuration**:
   - Navigate to the ZigBee integration in Home Assistant.
   - Start the pairing process.

4. **Confirm Connection**:
   - Once paired, the device should appear in the list of connected devices.
   - Assign names and configure entities as desired.

### Configuring Entities

- **Temperature and Humidity**: Available as sensors in Home Assistant.
- **Air Quality**: CO₂ and VOC levels displayed as separate entities.
- **Battery Level**: Monitor battery percentage or voltage.

## Troubleshooting

### Device Not Powering On

- **Check Battery**: Ensure the battery is inserted correctly and has sufficient charge.
- **Inspect Soldering**: Verify all solder joints are secure.

### Unable to Pair with Home Assistant

- **Signal Strength**: Move the device closer to the ZigBee coordinator.
- **Reset Device**: Try resetting the device (refer to firmware instructions).

### Inaccurate Sensor Readings

- **Calibration**: Sensors may require calibration—refer to the sensor datasheets.
- **Environmental Factors**: Ensure the device is placed appropriately and not influenced by external factors (e.g., direct sunlight).

## Maintenance

- **Battery Replacement**: Replace the battery when the battery level is low.
- **Firmware Updates**: Check for firmware updates to improve performance or add features.
- **Cleaning**: Gently clean the enclosure with a dry cloth; avoid moisture.

## Specifications

- **Dimensions**: [Provide dimensions]
- **Weight**: [Provide weight]
- **Operating Conditions**:
  - Temperature: -10°C to 50°C
  - Humidity: 10% to 90% RH
- **Power Supply**: [Battery type and specifications]

## Support

- **Community Forum**: [Link to community or discussion board]
- **Issues**: Report issues on the [GitHub Issues](https://github.com/yourusername/ThermoBeeLite/issues) page.
- **Email Support**: [tobiaslechenauer@gmail.com](mailto:tobiaslechenauer@gmail.com)

---

Thank you for using ThermoBee Lite!
