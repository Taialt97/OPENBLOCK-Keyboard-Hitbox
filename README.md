# Introduction

Welcome to our custom Fight-Stick Project. This project aims to create an open-source, modular, and easy-to-understand design for a fight-stick layout using the Arduino Pro Micro as the core. Our goal is to make the project as accessible and customizable as possible, providing users with the flexibility to adapt the design to their specific needs.

## Features

- **Comprehensive Design Files**: The project includes not only the PCB design but also the STL and Fusion 360 files for the plate and case. Additionally, a comprehensive drawing with all the plate dimensions is available for your convenience.

- **Connectivity**: The PCB offers both direct and hot-swap connectivity. This allows users the choice between soldering hot-swap sockets or directly soldering switches onto the PCB, providing a great deal of flexibility in how the board is assembled.

- **Compatibility**: The PCB can be compatible with Pro Micro and TinyS3 (a board that has Bluetooth). If TinyS3 is connected, the board can be supplied from a battery.

- **On/Off Switch**: An on/off switch is included in the design, allowing for control over the Arduino's power state. This switch can be wired to the board and mounted on the case, providing flexibility in the case design.

## Implementation

The project is developed using KiCad, a mandatory software tool, to enhance accessibility. The design is a refinement of an existing KiCad project, including both the schematics and the PCB layout. The design is also optimized for production, taking into account factors such as cost and manufacturability.

We collaborate with PCBWay for the manufacturing process and provide all necessary documentation to ensure a smooth and effective production process.

## Usage

The Arduino can be mounted on the bottom side of the PCB. A double switch controls whether the Arduino is powered on or off and provides a way for the Arduino to recognize its position through a specific pin's voltage level. This can be monitored using the software.

## Diagrams and Screenshots

This README includes references to various diagrams and screenshots from the text dialogue. However, as this is a text-based README, we have replaced these graphical elements with text descriptions. Please refer to the relevant sections of the README for these descriptions.

## Note

This project is an open-source initiative. It has been made as modular as possible, making it easy to understand and modify in the future. We believe in the power of community and collaboration, and we welcome contributions and suggestions from all those interested in this project.
