# ESP32 Doorbell

A local-first video doorbell project built around the Freenove ESP32-WROVER CAM and Home Assistant.

## Project goals

- Operate locally without a cloud subscription
- Send a doorbell event to Home Assistant
- Provide a live camera view and capture a snapshot when the button is pressed
- Use a printable, serviceable wall enclosure
- Keep credentials and site-specific configuration out of Git

## Current status

**Planning and hardware validation.** The existing camera board must be positively identified and measured before an enclosure is finalized or firmware pin assignments are committed.

## Repository layout

- `firmware/` — ESPHome configuration
- `home-assistant/` — automations, scripts, and dashboard examples
- `hardware/` — bill of materials, wiring, and measurements
- `enclosure/` — editable CAD, printable exports, and attribution
- `docs/` — design decisions, build instructions, and testing notes

## Known hardware starting point

The earlier prototype used a Freenove ESP32-WROVER camera board with an OV2640 camera. This is not the ESP32-S3 board used in the XDA article, so its pin assignments and enclosure geometry must not be copied blindly.

## Reference projects

- [XDA local-first ESP32 doorbell article](https://www.xda-developers.com/built-local-first-ring-doorbell-esp32/)
- [Adam Conway's ESPHome example](https://github.com/Incipiens/Adam-Home-Assistant-Snippets/tree/main/ESPHome/Local-first%20Ring%20Doorbell)
- [Freenove ESP32-WROVER CAM enclosure](https://www.printables.com/model/803138-esp32-wrover-cam-box-freenove)

Third-party designs and code remain under their respective licenses. See `enclosure/README.md` before importing or modifying enclosure files.

## Security

Do not commit real Wi-Fi credentials, ESPHome API keys, OTA passwords, Home Assistant tokens, public URLs, or precise installation-location details.

## License

Original code and documentation in this repository are licensed under the MIT License unless a file states otherwise. Imported enclosure designs and other third-party material may use different licenses.
