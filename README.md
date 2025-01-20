# config

## Rest in Peace

> What is this repository about?

`config` is a Home Assistant configuration designed to reduce sleep onset latency and nighttime awakenings while helping you maintain a consistent sleep schedule. It automatically adjusts AC and lights, factoring in time and temperature so you can rest in peace.

## Setup (Planned)

> How do I set up `config`?

1. Gather the hardware you'll need to keep running:
   - Raspberry Pi 5 16GB
   - Raspberry Pi 27W USB-C Power Supply with plug for your region
   - Raspberry Pi SSD
   - Raspberry Pi M.2 HAT+
   - Broadlink RM4 Mini
   - USB-A power adapter for Broadlink RM4 Mini with plug for your region
   - AC unit that is controllable via infrared IR
   - Sonoff ZBDongle-E
   - Sonoff SNZB-02P
   - Philips Hue Tap Switch Mini
   - Philips A21 - E26 smart bulb(s) - 100 W
   - Light socket(s) compatible with Philips A21 - E26 smart bulb(s) - 100 W

2. Gather the hardware you'll only need for the initial setup:
   - M.2 SSD housing
   - USB-C to USB-C cable
   - Ethernet cable
   - Mac for SSD setup and SSH access
   - iPhone for Broadlink app setup

3. Install Home Assistant on Raspberry Pi 5 16GB using the official guide, but skip the micro SD card and use your Raspberry Pi SSD with the Raspberry Pi M.2 HAT+ instead, connecting it to your Mac through the M.2 SSD housing and USB-C to USB-C cable

4. Follow the Home Assistant onboarding guide

5. Hook up all your hardware:
   - Power up Raspberry Pi 5 16GB
   - Connect Raspberry Pi 5 16GB to ethernet
   - Plug Sonoff ZBDongle-E into Raspberry Pi 5 16GB
   - Place Broadlink RM4 Mini where it has direct line of sight to the AC unit
   - Power up Broadlink RM4 Mini
   - Place Sonoff SNZB-02P at the height where you sleep, near your bed
   - Place Philips Hue Tap Switch Mini within arm's reach from your sleeping position
   - Install Philips A21 - E26 smart bulb(s) - 100 W in the socket(s)

6. Connect the Broadlink RM4 Mini to your Wi-Fi network using the Broadlink app

7. Enable SSH on your Home Assistant

8. SSH into your Home Assistant

9. Go to the `/config` directory

10. Add this repo as a remote

11. Pull the latest commit

12. Learn AC IR commands for all temperature settings in auto mode with heating and auto mode with cooling

13. Configure time ranges and their corresponding target temperatures

