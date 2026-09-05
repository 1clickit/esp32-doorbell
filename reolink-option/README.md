# Reolink option

This folder documents the finished-product alternative to the custom ESP32 doorbell.

## Recommended device

**Reolink Video Doorbell WiFi (D340W)**, using the existing doorbell transformer and two-wire cable.

## Recommended installation

Use the existing transformer and doorbell cable, bypass the old mechanical chime with the jumper included by Reolink, and use the Reolink plug-in wireless chime for audible alerts.

This is Reolink's **Method 1** and is the simplest likely fit for the existing one-transformer, one-chime, one-front-button system.

## Critical limitation

The Reolink D340W/D340P does **not** operate the existing mechanical chime. Once the old chime is bypassed, it will no longer ring. Use the paired Reolink Chime and/or Home Assistant announcements instead.

## Required power

The doorbell accepts:

- 12–24 VAC, 50/60 Hz; or
- 24 VDC

Reolink identifies 16 VAC, 30 VA as a commonly compatible mechanical-doorbell supply. Verify both the voltage and VA rating on the actual transformer before installation.

## Documents

- [Recommended existing-wiring installation](INSTALL_EXISTING_WIRING.md)
- [Pre-purchase and installation checklist](CHECKLIST.md)

## Official sources

- [Reolink: install with existing doorbell wiring](https://support.reolink.com/articles/10313334138265-How-to-Install-Reolink-Video-Doorbell-Cameras-to-the-Existing-Doorbell-Wiring/)
- [Reolink Video Doorbell WiFi](https://reolink.com/product/reolink-video-doorbell-wifi/)

This is an independent project summary, not Reolink documentation. Check the current manufacturer instructions supplied with the purchased hardware before installation.
