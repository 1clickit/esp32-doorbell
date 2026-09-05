# Reolink option

This folder documents the finished-product alternative to the custom ESP32 doorbell.

## Supported choices

### Option A — existing transformer and Wi-Fi

Use the **Reolink Video Doorbell WiFi (D340W)** with the existing compatible transformer and two-wire cable. Bypass the old mechanical chime with Reolink's supplied jumper, then use the Reolink plug-in Chime.

This is the normal, least-invasive replacement.

### Option B — PoE with an isolated exterior port

Use the **Reolink Video Doorbell PoE (D340P)** with a new Ethernet run. Assign its managed PoE switch port to a dedicated Camera VLAN and restrict it through OPNsense. Use port security as an additional control so the exposed cable does not provide useful access to the trusted network.

This is the preferred option when running Ethernet is practical.

## Critical chime limitation

Neither the D340W nor D340P operates the existing mechanical chime. The mechanical chime is bypassed or retired. Use the paired Reolink plug-in Chime and/or Home Assistant announcements.

## Documents

- [Side-by-side installation options](OPTIONS.md)
- [Option A: existing transformer and Wi-Fi](INSTALL_EXISTING_WIRING.md)
- [Option B: isolated PoE installation](INSTALL_POE_ISOLATED.md)
- [Pre-purchase and installation checklist](CHECKLIST.md)

## Wi-Fi model power requirements

The D340W accepts:

- 12–24 VAC, 50/60 Hz; or
- 24 VDC

Reolink identifies 16 VAC, 30 VA as a commonly compatible mechanical-doorbell supply. Verify both voltage and VA rating on the actual transformer before selecting Option A.

## Official sources

- [Reolink: install with existing doorbell wiring](https://support.reolink.com/articles/10313334138265-How-to-Install-Reolink-Video-Doorbell-Cameras-to-the-Existing-Doorbell-Wiring/)
- [Reolink Video Doorbell WiFi](https://reolink.com/product/reolink-video-doorbell-wifi/)
- [Reolink Video Doorbell PoE](https://reolink.com/product/reolink-video-doorbell-poe/)

This is an independent project summary, not Reolink documentation. Check the current manufacturer instructions supplied with the purchased hardware before installation.
