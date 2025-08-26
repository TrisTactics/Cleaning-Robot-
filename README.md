Gather Your Components
You’ll need:
- Arduino Uno board
- L298N motor driver or Adafruit Motor Shield
- 2 DC motors + wheels
- Ultrasonic sensor (HC-SR04)
- Servo motor (for cleaning brush)
- HC-05 Bluetooth module
- Battery pack (7.4V or 12V)
- The outer structure
- Jumper wires, breadboard, glue, screws
2. Assemble the Chassis
- Mount the motors on the chassis and attach the wheels.
- Fix the Arduino board and motor driver securely.
- Place the ultrasonic sensor at the front for obstacle detection.
- Attach the servo motor with a brush or mop mechanism.
3. Wire the Components
- Connect motors to the motor driver (OUT1–OUT4).
- Connect motor driver to Arduino (IN1–IN4, ENA, ENB).
- Wire ultrasonic sensor:
- Trig → pin 9
- Echo → pin 10
- Connect servo to pin 6.
- HC-05 Bluetooth module:
- TX → RX (pin 0)
- RX → TX (pin 1)
- VCC → 5V
- GND → GND
4. Upload the Code
- Open Arduino IDE.
- Paste the code we wrote.
- Select the correct board and port.
- Upload the sketch.
5. Test Autonomous Navigation
- Power up the robot.
- Place it in an open area.
- Watch it move forward and avoid obstacles using the ultrasonic sensor.
- The servo should activate the cleaning brush while moving.
6. Test Bluetooth Control
- Pair your phone with HC-05.
- Use a Bluetooth controller app (like “Bluetooth Serial Controller”).
- Send commands:
- F → Forward
- B → Backward
- L → Left
- R → Right
- S → Stop
- C → Clean
- X → Stop cleaning
