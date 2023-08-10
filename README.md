### Introduction

THE PROJECT IS STILL IN DEVELOPMENT. I'M WORKING HARD TO MAKE A VERSION THATE WILL WORK FOR EVERYONE.

Welcome to our custom Fight-Stick Project. This project aims to create an open-source, modular, and easy-to-understand design for a fight-stick (Hit Box) layout using the Arduino Pro Micro as the core. My goal is to make the project as accessible and customizable as possible, providing everyone with the flexibility to adapt the design to their specific needs.

![Bottom](https://github.com/Taialt97/mini-hitbox-pcb/assets/45160819/bd3939f3-17c9-43e0-8987-4a9b61269e5a)

### Features

- **Comprehensive Design Files**: The project includes not only the PCB design but also the STL and Fusion 360 files for the plate and case.
    
- **Connectivity**: The PCB offers both direct and hot-swap connectivity. This allows users the choice between soldering hot-swap sockets or directly soldering switches onto the PCB, providing a great deal of flexibility in how the board is assembled.
    
- **Compatibility**: The PCB can be compatible with Pro Micro and nice!nano (a board that has Bluetooth). If nice!nano is connected, the board can be supplied from a battery.
    
- **On/Off Switch**: An on/off switch is included in the design, allowing for control over the Arduino's power state. This switch can be wired to the board and mounted on the case, providing flexibility in the case design.

### Planned

- [ ] Reduce size of mounting holes
- [ ] Increase quantity of mounting holes
- [ ] Adjust placement of R3 and C3 to allow for flush mounting
- [ ] Updated Fusion 360 files
- [ ] Updated STL files
- [ ] In-depth explanation of the board's capabilities and operations
- [ ] One-click purchase option (via PCBWays or JLCPCB)
- [ ] Essential Component List Including Microcontrollers
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

  // Setup rows as outputs and set them high (they are active low)
  for (byte r = 0; r < ROW_NUM; r++) {
    pinMode(pin_rows[r], OUTPUT);
    digitalWrite(pin_rows[r], HIGH);
  }

  // Setup columns as inputs with internal pull-up resistors
  for (byte c = 0; c < COL_NUM; c++) {
    pinMode(pin_column[c], INPUT_PULLUP);
  }
}

void loop() {
  char key = keypad.getKey();
  if (key) {
    Serial.println(key);
  }
}
```

### Note

This project is an open-source initiative. It has been made as modular as possible, making it easy to understand and modify in the future. I believe in the power of community and collaboration, and welcome contributions and suggestions from all those interested in this project.
