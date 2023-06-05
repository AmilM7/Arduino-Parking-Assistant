# Arduino Parking Assistant

## Components Used

- Arduino Uno
- LCD Module With I2C Interface
- IR Proximity Sensor x 2
- Servo Motor
- Male To Male/Female Jumper Wires
- Small Adhesive Breadboard

## Code Files

### First File: `Arduino_Parking_System.ino`

#### Description

This file contains the main logic of the parking system. It initializes the LCD display, IR proximity sensors, and the servo motor. The system monitors the sensors to detect the presence of a vehicle and updates the available parking slots accordingly on the LCD display. The servo motor is used to control the parking barrier. When a vehicle enters or exits a parking slot, the servo motor adjusts the barrier accordingly.

### Second File: `I2C_Scanner.ino`

#### Description

This file is used for scanning I2C devices connected to the Arduino. It helps identify the I2C address of the LCD module with I2C interface. The information obtained from this scanning process is then used in the main code file (`Arduino_Parking_System.ino`) to establish communication with the LCD module.


## Usage

- Upon successful setup and power-up, the LCD display will show a welcome message.
- The system will monitor the IR proximity sensors to detect vehicle presence.
- As vehicles enter or exit parking slots, the available slot count will be updated on the LCD display.
- If all slots are occupied, a message indicating a full parking lot will be displayed on the LCD.
- The servo motor will adjust the parking barrier accordingly when vehicles enter or exit slots.
