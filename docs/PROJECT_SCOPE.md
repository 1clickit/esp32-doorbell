# Project scope

## Objective

Build a reliable, locally operated video doorbell using the existing Freenove ESP32-WROVER CAM, an external doorbell button, and Home Assistant.

## Initial deliverables

1. Confirm the exact camera-board revision and dimensions.
2. Validate camera streaming with ESPHome.
3. Select the doorbell button and power arrangement.
4. Generate a Home Assistant event on button press.
5. Capture and retain a snapshot locally.
6. Produce a serviceable, rain-resistant wall enclosure.
7. Document assembly, installation, rollback, and testing.

## Design principles

- Local operation first
- Simple and reversible configuration
- No credentials in source control
- Replaceable electronics and button
- Weather resistance without trapping condensation
- Clear attribution for imported code and CAD
- Test indoors before permanent outdoor installation

## Out of scope for the first prototype

- Cloud recording
- Facial recognition
- Package detection
- Two-way audio
- Mains-voltage work
- Claiming an enclosure is weatherproof before physical testing

## Current decisions

| Item | Decision |
|---|---|
| Repository | `1clickit/esp32-doorbell` |
| Visibility | Public |
| Controller | Existing Freenove ESP32-WROVER CAM |
| Camera | OV2640, pending physical confirmation |
| Automation platform | Home Assistant |
| Firmware framework | ESPHome, pending board test |
| Primary operation | Local network |
