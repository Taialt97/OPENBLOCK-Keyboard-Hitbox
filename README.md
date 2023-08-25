
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)]( https://opensource.org/licenses/MIT ) [![Version: 2.0.0](https://img.shields.io/badge/Version-2.0.0-blue.svg)]( https://github.com/your-repo-link )
 

# Introduction
This project is in development, focusing on a universal fight-stick (Hit Box) layout. With the Arduino Pro Micro and the option of using either the Pro Micro mega32u4 chip or the GP2040 chip, the design aims for open-source, modular, and accessible customization.

![top](https://github.com/Taialt97/mini-hitbox-pcb/assets/45160819/a9b5a59a-0500-422f-be36-5845a719662f)
![bot](https://github.com/Taialt97/mini-hitbox-pcb/assets/45160819/0649b3d5-1120-448b-bb93-668e5914f3f8)

## Chip Compatibility
- **Pro Micro mega32u4 chip**: A more budget-friendly option.
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

1. [Elite-C V4 - USB-C Pro Micro Replacement ATmega32u4](https://keeb.io/collections/diy-parts/products/elite-c-low-profile-version-usb-c-pro-micro-replacement-atmega32u4) 
2. [Elite-Pi - USB-C Pro Micro Replacement RP2040 Controller](https://keeb.io/collections/diy-parts/products/elite-pi-usb-c-pro-micro-replacement-rp2040)
3. [SparkFun Pro Micro - 5V/16MHz ](https://www.sparkfun.com/products/12640)
4. [SparkFun Qwiic Pro Micro - USB-C (ATmega32U4)](https://www.sparkfun.com/products/15795)
5. [SparkFun Pro Micro - 3.3V/8MHz](https://www.sparkfun.com/products/12587)
6. [SparkFun Pro Micro - RP2040](https://www.sparkfun.com/products/18288)

### Parts List
To ensure affordability, I've listed essential parts and some alternatives:

- PCB | $8 (without shipping)
- (optional) Hot-swappable PCB socket | $3
- Keycaps | $5-$15 (depends on quality)
- Switch | $5-$50 (depends on the manufacturer and "quality" of the switch)
- Pro Micro | $4-$30 (ensure the chip is **atmega32u4**)

### Recommended
- KESTER SOLDER | $35-$60 (quality soldering wire)
- PINECIL – Smart Mini Portable Soldering Iron (Version 2) | $25.99-$35.99

# Features
- **Comprehensive Design Files**: Includes PCB design, STL, and Fusion 360 files for the plate and case.
- **Connectivity**: Offers both direct and hot-swap connectivity for flexibility in assembly.
- **Compatibility**: Compatible with Pro Micro, and more microcontrollers to be added in the future.

# Note
This project is an open-source initiative, designed for modularity and ease of understanding. Contributions and suggestions from the community are welcome, fostering collaboration and growth.

