# config

## Rest in Peace

> What is this repository about?

`config` is a Home Assistant configuration designed to reduce sleep onset latency and nighttime awakenings while helping you maintain a consistent sleep schedule. It automatically adjusts AC and lights, factoring in time and temperature so you can rest in peace.

## Setup (Planned)

> How do I set up `config`?

1. Gather the hardware you'll need to keep running:
   - [Raspberry Pi 5 16GB](https://www.raspberrypi.com/products/raspberry-pi-5)
   - [Raspberry Pi 27W USB-C Power Supply](https://www.raspberrypi.com/products/27w-power-supply) with plug for your region
   - [Raspberry Pi SSD](https://www.raspberrypi.com/products/ssd)
   - [Raspberry Pi M.2 HAT+](https://www.raspberrypi.com/products/m2-hat-plus)
   - [Broadlink RM4 Mini](https://www.broadlink.ae/product-page/broadlink-rm4-mini)
   - [Raspberry Pi Case for Raspberry Pi 5](https://www.raspberrypi.com/products/raspberry-pi-5-case)
   - USB-A power adapter for Broadlink RM4 Mini with plug for your region
   - AC unit that is controllable via infrared IR
   - [Sonoff ZBDongle-E](https://sonoff.tech/product/gateway-and-sensors/sonoff-zigbee-3-0-usb-dongle-plus-e)
   - [Sonoff SNZB-02P](https://sonoff.tech/product/gateway-and-sensors/snzb-02p)
   - [Philips Hue Tap Switch Mini Black](https://www.philips-hue.com/en-us/p/accessory-hue-tap-switch-mini-black/46677581954)
   - [Philips Hue A21 - E26 smart bulb(s) - 100 W](https://www.philips-hue.com/en-us/p/hue-white-and-color-ambiance-a21-e26-smart-bulb-100-w/046677562984)
   - Light socket(s) compatible with Philips A21 - E26 smart bulb(s) - 100 W

1. Gather the hardware you'll only need for the initial setup:
   - M.2 SSD housing
   - USB-C to USB-C cable
   - Ethernet cable
   - Mac for SSD setup and SSH access
   - iPhone for Broadlink app setup

1. Install Home Assistant on Raspberry Pi 5 16GB using [the official guide](https://www.home-assistant.io/installation/raspberrypi), but skip the micro SD card and use your Raspberry Pi SSD with the Raspberry Pi M.2 HAT+ instead, connecting it to your Mac through the M.2 SSD housing and USB-C to USB-C cable

1. Hook up all your hardware:
   1. Pop your Raspberry Pi 5 16GB into Raspberry Pi Case for Raspberry Pi 5
   1. Power up Raspberry Pi 5 16GB
   1. Connect Raspberry Pi 5 16GB to ethernet
   1. Plug Sonoff ZBDongle-E into Raspberry Pi 5 16GB
   1. Place Broadlink RM4 Mini where it has direct line of sight to the AC unit
   1. Power up Broadlink RM4 Mini
   1. Place Sonoff SNZB-02P at the height where you sleep, near your bed
   1. Place Philips Hue Tap Switch Mini Black within arm's reach from your sleeping position
   1. Install Philips Hue A21 - E26 smart bulb(s) - 100 W in the socket(s)

1. Follow [the Home Assistant onboarding guide](https://www.home-assistant.io/getting-started/onboarding)

1. Connect the Broadlink RM4 Mini to your Wi-Fi network using the Broadlink app

1. Enable SSH on your Home Assistant

1. SSH into your Home Assistant

1. Go to the `/config` directory

1. Add this repo as a remote

1. Pull the latest commit

1. Learn AC IR commands for all temperature settings in auto mode with heating and auto mode with cooling

1. Configure time ranges and their corresponding target temperatures

