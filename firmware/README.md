# Firmware

This directory will contain the ESPHome package and an example device configuration.

## Before adding a pin map

Confirm all of the following from the physical board or its authoritative documentation:

- Exact Freenove model and revision
- ESP32 module marking
- Camera sensor
- Camera data and clock pins
- USB connector type
- Available GPIO for the doorbell button
- Whether a status LED, flash LED, microSD slot, or PSRAM shares required pins

The ESP32-S3 configuration from the referenced XDA project is **not** compatible by assumption with the older ESP32-WROVER board.

## Planned files

- `doorbell-base.yaml` — reusable configuration without private values
- `example-device.yaml` — example substitutions and secrets usage
- `secrets.example.yaml` — variable names only, never real credentials

## Safety rule

Never commit `secrets.yaml`, API encryption keys, OTA passwords, Wi-Fi passwords, or Home Assistant tokens.
