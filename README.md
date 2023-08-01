
### Introduction

Welcome to our custom Fight-Stick Project. This project aims to create an open-source, modular, and easy-to-understand design for a fight-stick layout using the Arduino Pro Micro as the core. Our goal is to make the project as accessible and customizable as possible, providing users with the flexibility to adapt the design to their specific needs.

![Bottom](https://github.com/Taialt97/mini-hitbox-pcb/assets/45160819/bd3939f3-17c9-43e0-8987-4a9b61269e5a)

### Features

- **Comprehensive Design Files**: The project includes not only the PCB design but also the STL and Fusion 360 files for the plate and case. Additionally, a comprehensive drawing with all the plate dimensions is available for your convenience.
    
- **Connectivity**: The PCB offers both direct and hot-swap connectivity. This allows users the choice between soldering hot-swap sockets or directly soldering switches onto the PCB, providing a great deal of flexibility in how the board is assembled.
    
- **Compatibility**: The PCB can be compatible with Pro Micro and TinyS3 (a board that has Bluetooth). If TinyS3 is connected, the board can be supplied from a battery.
    
- **On/Off Switch**: An on/off switch is included in the design, allowing for control over the Arduino's power state. This switch can be wired to the board and mounted on the case, providing flexibility in the case design.

### Implementation

The project is developed using KiCad, a mandatory software tool, to enhance accessibility. The design is a refinement of an existing KiCad project, including both the schematics and the PCB layout. The design is also optimized for production, taking into account factors such as cost and manufacturability.

We collaborate with PCBWay for the manufacturing process and provide all necessary documentation to ensure a smooth and effective production process.

### Usage

The Arduino can be mounted on the bottom side of the PCB. A double switch controls whether the Arduino is powered on or off and provides a way for the Arduino to recognize its position through a specific pin's voltage level. This can be monitored using the software.

### Diagrams and Screenshots

This README includes references to various diagrams and screenshots from the text dialogue. However, as this is a text-based README, we have replaced these graphical elements with text descriptions. Please refer to the relevant sections of the README for these descriptions.

### BOM 
| Designator | Footprint | Quantity | Value | Part # | LCSC Part # |
|------------|-----------|----------|-------|--------|-------------|
| C2 | 805 | 1 | 4.7uF | CC0805KKX7R8BB475 | C354262 |
| C3 | 805 | 1 | 0.1uF | CC0805KRX7R9BB104 | C49678 |
| D1, D10, D11, D12, D13, D14, D2, D3, D4, D5, D6, D7, D8, D9 | D_SOD-123 | 14 | 1N4448W-TP | 1N4448W-TP | C668855 |
| J1 | JST_PH_B2B-PH-K_1x02_P2.00mm_Vertical | 1 | B2B-PH-K-S(LF)(SN) | B2B-PH-K-S(LF)(SN) | C131337 |
| MX1, MX10, MX11, MX12, MX13, MX14, MX2, MX3, MX4, MX5, MX6, MX7, MX8, MX9 | Kailh_socket_MX_optional | 14 | MX_SW_solder | Kailh CPG151101D212 | C400234 |


### Code

```
#include <Keypad.h>

const byte ROW_NUM = 2; // two rows
const byte COL_NUM = 7; // seven columns

// Define the keymap
char keys[ROW_NUM][COL_NUM] = {
  {'1','2','3','4','5','6','7'},
  {'8','9','4','5','6','*','0'}
};

// Connect keypad ROW0, ROW1, ... to these Arduino pins.
byte pin_rows[ROW_NUM] = {2, 3}; // Connect to the row pinouts of the keypad
// Connect keypad COL0, COL1, ... to these Arduino pins.
byte pin_column[COL_NUM] = {16, 14, 15, 9, 10, 5, 4}; // Connect to the column pinouts of the keypad

// Create the keypad
Keypad keypad = Keypad(makeKeymap(keys), pin_rows, pin_column, ROW_NUM, COL_NUM);

void setup() {
  Serial.begin(9600);
}

void loop() {
  char key = keypad.getKey();
  if (key) {
    Serial.println(key);
  }
}
```

### Note

This project is an open-source initiative. It has been made as modular as possible, making it easy to understand and modify in the future. We believe in the power of community and collaboration, and we welcome contributions and suggestions from all those interested in this project.
