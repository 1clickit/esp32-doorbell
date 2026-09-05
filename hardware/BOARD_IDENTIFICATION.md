# Existing camera board identification

## Confirmed from the hardware photograph

| Feature | Identification |
|---|---|
| Board label | Freenove ESP32-WROVER-DEV |
| ESP32 family | Original ESP32/WROVER generation, not ESP32-S3 |
| USB connector | Micro-USB |
| Programming controls | EN/RST and BOOT/IO0 pushbuttons |
| Camera connection | Front-facing FPC connector |
| Camera placement | Camera centered over the ESP32 module shield |
| Header style | Two long through-hole pin-header rows |
| Status markings | ON, TX, and RX indicators |
| Camera ribbon marking | Appears to include `OV2` and `640-V2`; exact sensor remains to be confirmed from the rear or documentation |

## Enclosure implications

Use the original Freenove ESP32-WROVER CAM enclosure geometry, not the ESP32-S3 remix. The enclosure must accommodate:

- Micro-USB at the short edge
- Both EN/RST and BOOT/IO0 buttons beside the USB connector
- Camera centered above the module
- Camera flex cable and connector below the module
- Full-length side headers, or clearance for their solder joints if headers are removed
- Indicator LEDs near the lower-right portion of the board

## Still requiring measurement

A photograph confirms the family and layout but is not dimensionally reliable. Before producing final CAD, measure:

1. Overall PCB length and width
2. Maximum depth from PCB rear to lens face
3. Lens-center position from the PCB sides and top edge
4. USB connector width, height, and projection
5. Mounting-hole locations, if present
6. Clearance required for the external button wiring
7. Wall mounting area and desired downward camera angle

## Reference enclosure

- [ESP32 Wrover Cam Box (Freenove) on Printables](https://www.printables.com/model/803138-esp32-wrover-cam-box-freenove/)
- [Original Thingiverse listing](https://www.thingiverse.com/thing:6528728)

These listings are the closest identified dimensional starting point. Their files and license must be checked and attributed before importing them into this repository.
