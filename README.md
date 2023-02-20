# :notes: pi-midi-host-no-bt

> Setup a Raspberry Pi as a headless MIDI USB host, with auto-connection and MIDI merging of all sources.

Optimized for headless configuration on a device without Bluetooth

## Usage

1. Use [Raspberry Pi Imager](https://www.raspberrypi.com/software/) to install Raspberry Pi OS Lite. Make sure to use Advanced Options (the gear menu) to enable SSH and create a user account. 
1. SSH into your Pi and run this command: `bash <(curl -Ls https://raw.githubusercontent.com/dmessent/pi-midi-host-no-bt/main/setup.sh)`
1. Reboot

> Note: setup.sh currently includes many commented-out steps involving Bluetooth and setting the filesystem to read-only. These were either unnecessary or seemed to cause problems with a headless pi zero. If you're interested in Bluetooth, check out the original https://github.com/sinedied/pi-midi-host project

### Aliases

Use these alias to quickly manage your midi setup:
- `midi`: show connected midi devices
- `connect`: reconnect all midi devices

## Credits

This is a fork of https://github.com/sinedied/pi-midi-host project:

> Most of this work was based on instructions from [this post](https://neuma.studio/rpi-midi-complete.html).
> 
> Additions:
> - All-in-one script to setup a new Pi
> - MIDI in/out filters for specific devices
> - Bluetooth device connection instructions
> - Commands aliases
> - Drivers for M-Audio MIDISPORT 2x2
>
