
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)]( https://opensource.org/licenses/MIT ) [![Version: 2.0.0](https://img.shields.io/badge/Version-2.0.0-blue.svg)]( https://github.com/your-repo-link )
 

# Introduction
This project aims to create an open-source, modular, and easy-to-understand design for a Hit Box layout using the Raspberry Pi (RP2040) as the core. My goal is to make the project as accessible and customizable as possible, providing everyone with the flexibility to adapt the design to their specific needs.

![downImg(2)](https://github.com/Taialt97/The-Fighter-Mini-Hitbox-PCB-Guide/assets/45160819/33555f3e-2cb2-453c-9b36-5af131ce8e13)

## Chip Compatibility
- **GP2040 chip**: Offers higher compatibility with PC, PS4, PS3, Switch, and Xbox.

| ProMicro (Mega32U4) | RespbarryPie (GP2040) | NameOfSwitch | Action      | PlayStation   | Xbox   |
|---------------------|-----------------------|--------------|-------------|---------------|----------------|
| 6                   | 6                     | MX10         | Up         | Dpad Up   | Dpad Up             |            |                |
| 14                  | 20                    | MX2          | Down        |Dpad Down   | Dpad Down           |            |                |
| 16                  | 23                    | MX1          | Left        | Dpad Left   | Dpad Left           |            |                |
| 15                  | 22                    | MX3          | Right       | Dpad Right       | Dpad Right          |            |                |
| 21                  | 29                    | MX4          | Light Punch | Square        | X              |            |                |
| 5                   | 5                     | MX11         | Light Kick  | X             | A              |            |                |
| 4                   | 4                     | MX5          | Medium Punch| Circle        | B              |            |                |
| 20                  | 28                    | MX12         | Medium Kick | Triangle      | Y              |            |                |
| 18                  | 26                    | MX6          | Heavy Punch | L1            | LB             |            |                |
| 19                  | 27                    | MX13         | Heavy Kick  | R1            | RB             |            |                |
| 2                   | 2                     | MX7          | Triple Punch| L2            | LT             |            |                |
| 3                   | 3                     | MX14         | Triple Kick | R2            | RT             |            |                |
| 8                   | 8                     | MX8          | Select 1    | Select        | Back           |            |                |
| 7                   | 7                     | MX9          | Select 2    | Start         | Start          |            |                |

# Costs
The cost to build the fight-stick will depend on parts, shipping, and tools. Below is a breakdown:

1. PCB (minimum order of 5) without shipping: **$8**. Shipping will vary by location and method.
2. Parts for PCB assembly: **$25** (hot swap sockets, keys, switches, Pro Micro, and IC Sockets).
3. Tools: Varies widely, but a cost-effective approach is possible.

## Part List
### Micro Chips List
Below is a list of top-tier microcontrollers that I've found to be the best in the market. While more cost-effective alternatives are available from sites like Aliexpress (which I've personally tested and found satisfactory), the following options are slightly more expensive but come with a guarantee of proper functionality.

If you're using a different 12-pin microcontroller that you think should be included here, feel free to leave a comment!

1. [Elite-Pi - USB-C Pro Micro Replacement RP2040 Controller](https://keeb.io/collections/diy-parts/products/elite-pi-usb-c-pro-micro-replacement-rp2040)
2. [SparkFun Pro Micro - RP2040](https://www.sparkfun.com/products/18288)

### Parts List
To ensure affordability, I've listed essential parts and some alternatives:

- PCB | $8 (without shipping)
- (optional) Hot-swappable PCB socket | $3
- Keycaps | $5-$15 (depends on quality)
- Switch | $5-$50 (depends on the manufacturer and "quality" of the switch)
- Pro Micro | $4-$30 (ensure the chip is **RP2040**)

### Recommended
- KESTER SOLDER | $35-$60 (quality soldering wire)
- PINECIL – Smart Mini Portable Soldering Iron (Version 2) | $25.99-$35.99

# Code

Upon connecting the microcontroller to your computer, a new drive will appear. 
- Drag the `nuke.h` file into this drive; the microcontroller will disconnect and then reconnect.
- Drag the `OpenBlock.h` file into the drive. You'll hear a sound indicating that the drive has disconnected and reconnected.
To test your controller, visit the [Gamepad Tester Website](https://hardwaretester.com/gamepad).
For modifying the code or creating new code, go to the [GP2040-CE](https://gp2040-ce.info/#/) website.
There, you'll find all the resources you need to customize or create new code. If you have any questions, refer to our [Discord channel](https://discord.gg/kJDAZVwU) — they're awesome!


# Features
- **Comprehensive Design Files**: Includes PCB design, STL, and Fusion 360 files for the plate and case.
- **Connectivity**: Offers both direct and hot-swap connectivity for flexibility in assembly.
- **Compatibility**: Compatible with Pro Micro, and more microcontrollers to be added in the future.

# Note
This project is an open-source initiative, designed for modularity and ease of understanding. Contributions and suggestions from the community are welcome, fostering collaboration and growth.

# Sponsorship
This repository is proudly sponsored by [PCBWay](https://www.pcbway.com/).
[![PCBWay](https://www.pcbway.com/img/logo2.png)](https://www.pcbway.com/)
PCBWay specializes in manufacturing high-quality PCBs. They offer a range of services including PCB prototyping, assembly, and much more. We are grateful for their support in making this project possible.
For more information, visit their [website](https://www.pcbway.com/).

