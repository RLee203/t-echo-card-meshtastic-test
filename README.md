# T-Echo-Card Meshtastic Test Build

This repo contains an early development/test build of Meshtastic for the LilyGO T-Echo-Card.

This is not an official Meshtastic release and it may still contain bugs.

## Install

1. Put the T-Echo-Card into UF2 bootloader mode.
2. Copy `t_echo_meshtastic.uf2` to the device's UF2 drive.
3. Wait for the device to reboot into Meshtastic.

## Current Test Status

What has been tested so far:
- Device boots into Meshtastic
- Screen is working with a simplified small-screen layout
- Button navigation is working
- Works with the official Meshtastic app
- Settings can be changed through the app
- BLE pairing works
- Sending messages works
- Receiving messages works
- GPS/compass display is working in a simplified view
- Button C cycles the onboard LEDs / flashlight brightness

## LED Behavior

Button C cycles the 3 onboard LEDs through:
- off
- low
- medium
- high
- back to off

## BLE

BLE pairing works with the official Meshtastic app.

This test build can still be configured through the Meshtastic app. If users prefer fixed-pin pairing instead of the normal screen passkey flow, they can change that in the Bluetooth settings inside the app.

## Notes

- This is still a development build.
- Some display/UI polish may still be needed.
- Additional hardware behavior may still need testing.
- Please expect bugs and report what you find.
