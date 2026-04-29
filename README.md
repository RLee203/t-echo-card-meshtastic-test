# T-Echo-Card Meshtastic Test Build

This repo contains an early development/test build of Meshtastic for the LilyGO T-Echo-Card.

This is not an official Meshtastic release and it may still contain bugs.

## Quick Notes

- Works with the official Meshtastic app
- Sending and receiving messages works
- On-device button navigation works
- Button C controls the onboard LED flashlight levels
- BLE pairing works with the normal Meshtastic pairing flow

## Latest Build Updates

- Small-screen menu overlays were adjusted to fit the T-Echo Card OLED more cleanly
- Boot screen was simplified so the tiny OLED shows only the Meshtastic logo
- GPS/compass screen is using a simplified ultra-small layout for the card display

## Install

1. Put the T-Echo-Card into UF2 bootloader mode.
2. Copy `t_echo_meshtastic.uf2` to the device's UF2 drive.
3. Wait for the device to reboot into Meshtastic.

## Button Behavior

- Button A / B: used for on-device navigation
- Button C: cycles the 3 onboard LEDs / flashlight brightness

## LED Behavior

Button C cycles the 3 onboard LEDs through:
- off
- low
- medium
- high
- back to off

## BLE

BLE pairing works with the official Meshtastic app.

This build uses the normal Meshtastic BLE pairing behavior by default. If users want fixed-pin pairing instead, they can change that in the Bluetooth settings inside the app.

## Current Test Status

What has been tested so far:
- Device boots into Meshtastic
- Screen is working with a simplified small-screen layout
- Menu popups now fit the small OLED better
- Boot screen now shows a logo-only splash on startup
- Button navigation is working
- Works with the official Meshtastic app
- Settings can be changed through the app
- BLE pairing works
- Sending messages works
- Receiving messages works
- GPS/compass display is working in a simplified view
- Button C cycles the onboard LEDs / flashlight brightness

## Notes

- This is still a development build.
- Some display/UI polish may still be needed.
- Additional hardware behavior may still need testing.
- Please expect bugs and report what you find.
