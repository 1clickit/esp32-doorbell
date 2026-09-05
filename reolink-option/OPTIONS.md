# Installation options

| Feature | Existing transformer + Wi-Fi | PoE + isolated Camera VLAN |
|---|---|---|
| Doorbell model | D340W | D340P |
| Reuses current two-wire cable | Yes | No |
| New cable required | No | Ethernet |
| Power source | 12–24 VAC or 24 VDC | Managed PoE switch/injector |
| Network connection | Wi-Fi | Ethernet |
| Audible indoor alert | Reolink plug-in Chime | Reolink plug-in Chime |
| Existing mechanical chime | Bypassed; does not operate | Not used |
| Installation complexity | Lower | Higher |
| Connection reliability | Depends on Wi-Fi | Preferred |
| Exterior-port security | Not applicable | Camera VLAN plus firewall and port security |

## Option A: typical existing-wiring installation

Use the D340W, retain the compatible transformer and existing two-wire cable, bypass `TRANS` and `FRONT` at the old mechanical chime, and pair the Reolink plug-in Chime.

Choose this when avoiding a new cable run matters most.

See [INSTALL_EXISTING_WIRING.md](INSTALL_EXISTING_WIRING.md).

## Option B: preferred PoE installation

Use the D340P on a dedicated access port assigned to an isolated Camera VLAN. Permit only the exact local services needed by Home Assistant, Frigate/NVR, DNS, NTP, and trusted administration.

Choose this when a new Ethernet run is practical and connection reliability matters most.

See [INSTALL_POE_ISOLATED.md](INSTALL_POE_ISOLATED.md).
