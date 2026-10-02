# MotoBuddy

MotoBuddy is a custom motorcycle companion device: a round, handlebar-mounted
display that pairs with a phone app over Bluetooth to track ride performance
(0–60 time, launches, GPS-based stats) and surface it at a glance while riding.

This repo is a **portfolio showcase** of the hardware and firmware work —
photos of the real, assembled boards. The PCB design files, firmware source,
companion app, and website are developed privately and aren't published here.

## What's inside

- `Rev1.0/` — the first built-and-tested revision ("Alpha"). Photos of the
  assembled board, plus screenshots of the companion app in use, are in
  [`Rev1.0/Photos_Videos`](Rev1.0/Photos_Videos).
- `Rev2.0/` — the in-progress second revision ("Beta").

## Hardware

- ESP32-based main board, round form factor sized to mount behind the
  handlebars
- Onboard GPS module for speed/position
- IMU for launch and shake detection (used for 0–60 timing)
- TFT display with adaptive brightness
- USB-C for charging/programming, coin-cell-backed RTC
- BLE link to a companion mobile app; Wi-Fi for OTA firmware updates

## Software (private)

- Firmware: C++ on the Arduino/ESP32 toolchain (PlatformIO)
- Companion app: Flutter (iOS/Android)
- Project site: Next.js

## Why the design files aren't here

The schematic, PCB layout, gerbers/manufacturing outputs, 3D models, and all
source code represent the actual IP behind the product, so they're kept in a
private working copy rather than this repo. What's shown here is meant to
demonstrate the hardware/embedded work, not to be a buildable copy of it.
