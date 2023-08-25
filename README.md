
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)]( https://opensource.org/licenses/MIT ) [![Version: 2.0.0](https://img.shields.io/badge/Version-2.0.0-blue.svg)]( https://github.com/your-repo-link )
 
# Introduction
This project is in development, focusing on a universal fight-stick (Hit Box) layout. With the Arduino Pro Micro and the option of using either the Pro Micro mega32u4 chip or the GP2040 chip, the design aims for open-source, modular, and accessible customization.

![top](https://github.com/Taialt97/mini-hitbox-pcb/assets/45160819/a9b5a59a-0500-422f-be36-5845a719662f)
![bot](https://github.com/Taialt97/mini-hitbox-pcb/assets/45160819/0649b3d5-1120-448b-bb93-668e5914f3f8)

## Chip Compatibility
- **Pro Micro mega32u4 chip**: A more budget-friendly option.
- **GP2040 chip**: Offers higher compatibility with PC, PS4, PS3, Switch, and Xbox.

| ProMicro (Mega32U4) | RespbarryPie (GP2040) | NameOfSwitch | Action      | PlayStation   | NameOfButton   | Xbox       | NameOfButton   |
|---------------------|-----------------------|--------------|-------------|---------------|----------------|------------|----------------|
| 6                   | 6                     | MX10         | UP          |               | UP             |            |                |
| 14                  | 20                    | MX2          | DOWN        |               | DOWN           |            |                |
| 16                  | 23                    | MX1          | LEFT        |               | LEFT           |            |                |
| 15                  | 22                    | MX3          | RIGHT       |               | RIGHT          |            |                |
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

