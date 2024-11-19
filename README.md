# ThermoBee Lite

**ThermoBee Lite** is a compact, energy-efficient ZigBee sensor for measuring temperature, humidity, air quality, and battery level. Designed to be compatible with Home Assistant, it aims to provide at least 6 months of battery life on a single battery.

## Features

- **Temperature and Humidity Monitoring**: Accurate readings using high-quality sensors.
- **Air Quality Measurement**: Monitors CO₂ and VOC levels for a healthier environment.
- **Battery Level Reporting**: Keeps track of battery status to notify when replacements are needed.
- **ZigBee Connectivity**: Seamless integration with ZigBee networks and Home Assistant.
- **Compact Design**: Small form factor suitable for various locations.
- **Open Source**: Hardware and software are open for community contributions and customization.

## Getting Started

### Prerequisites

- A ZigBee coordinator compatible with Home Assistant.
- Basic knowledge of electronics and soldering (for hardware assembly).
- Development environment set up for firmware compilation (if modifying firmware).

### Installation

1. **Hardware Assembly**:
   - Gather all components listed in the [Bill of Materials](./hardware/BillOfMaterials/BOM.xlsx).
   - Follow the [Hardware Assembly Guide](./docs/UserManual.md#hardware-assembly) to assemble the device.

2. **Firmware Upload**:
   - Download the pre-compiled firmware or compile it yourself from the [firmware](./firmware/) directory.
   - Upload the firmware to the microcontroller using the appropriate programmer.

3. **Enclosure Assembly**:
   - Print the enclosure parts from the [STL files](./enclosure/STL-Files/).
   - Assemble the enclosure as per the instructions in the [User Manual](./docs/UserManual.md#enclosure-assembly).

4. **Integration with Home Assistant**:
   - Add the ThermoBee Lite device to your ZigBee network.
   - Configure the device in Home Assistant using the steps outlined in the [User Manual](./docs/UserManual.md#home-assistant-integration).

## Usage

- Monitor sensor readings directly from the Home Assistant dashboard.
- Set up automations based on temperature, humidity, or air quality levels.
- Receive notifications when the battery level is low.

## Contributing

Contributions are welcome! Please read our [Contributing Guidelines](./CONTRIBUTING.md) to get started.

## License

This project is licensed under multiple licenses:

- **Firmware**: [MIT License](./firmware/LICENSE)
- **Hardware Designs**: [CERN OHL v2 Permissive](./hardware/LICENSE)
- **Enclosure Designs**: [CERN OHL v2 Permissive](./enclosure/LICENSE)
- **Documentation**: [CC BY-SA 4.0](./docs/LICENSE)

## Contact

- **Project Maintainer**: [Tobias Lechenauer](mailto:tobiaslechenauer@gmail.com)
- **Issues**: Please report issues on the [GitHub Issues](https://github.com/yourusername/ThermoBeeLite/issues) page.

---
