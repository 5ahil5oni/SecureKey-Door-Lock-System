🔐 SecureKey: Door Lock System

An Arduino-based smart door locking system that uses a keypad interface and servo motor to allow secure access using a PIN code. The system supports EEPROM-based password storage and password change functionality, making it ideal for home and office automation.

 🚀 Features

- 🔢 4-digit PIN-based access control
- 🔄 Change password using the keypad
- 🔒 Auto-lock after inactivity (10 seconds)
- 💾 EEPROM-based password storage (retains data after power off)
- 💡 LCD feedback for user interaction
- 🔧 Servo motor for locking/unlocking mechanism

🧰 Technologies Used

- Arduino UNO
- Servo Motor (SG90)
- 4x4 Matrix Keypad
- 16x2 LCD Display
- EEPROM Library
- LiquidCrystal Library
- Keypad Library
- Servo Library

🧠 How It Works

1. On startup, system checks if password exists in EEPROM. If not, sets a default password `5555`.
2. User is prompted to enter a password.
3. On correct entry:
   - Door unlocks for 10 seconds or until user locks it manually.
   - Menu options allow changing the password.
4. On incorrect entry:
   - Access is denied and system returns to lock state.

🛠️ Setup Instructions

1. Upload `main.ino` to Arduino UNO using Arduino IDE.
2. Connect:
   - Keypad to digital pins 2–5 (rows), A0–A3 (cols)
   - Servo to pin 6
   - LCD to pins 7–12
3. Power the Arduino and test the system.

🙋‍♂️ Author

Sahil Soni 
B.Tech - Electronics and Communication  
SISTec, Bhopal
