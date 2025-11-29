# Automatic-Room-Visitor-Counter
This project uses an Arduino, two IR sensors, and an LCD display to create an automatic bidirectional visitor counter. It keeps track of how many people enter and exit a room and automatically turns the lights ON/OFF based on occupancy.  

# Automatic Room Visitor Counter with Light Control

This project is an Arduino-based visitor counter that tracks how many people enter and exit a room using two IR sensors. It automatically turns a light ON or OFF using a relay based on the number of people inside. A 16x2 LCD displays the real-time count of people in the room.

---

## Features
- Bidirectional visitor counting (IN & OUT detection)
- Automatic light control using a relay
- Real-time count display on a 16x2 LCD
- Simple and low-cost design
- Easy to build and modify

---

## Hardware Requirements
- Arduino Uno / Nano / Mega  
- 16x2 LCD Display (LiquidCrystal library)  
- 2 IR Sensor Modules  
- Relay Module (for controlling a bulb/light)  
- Breadboard & jumper wires  

---

## Pin Configuration

| Component          | Arduino Pin |
|-------------------|-------------|
| LCD RS            | 12 |
| LCD EN            | 11 |
| LCD D4            | 5 |
| LCD D5            | 4 |
| LCD D6            | 3 |
| LCD D7            | 2 |
| IR Sensor (IN)    | 8 |
| IR Sensor (OUT)   | 9 |
| Relay (Bulb)      | 10 |

---

## How It Works
1. The **IN** sensor detects a person entering and increments the counter.  
2. The **OUT** sensor detects a person leaving and decrements the counter.  
3. The current number of people inside is shown on the LCD.  
4. When the count is **zero**, the system displays "Nobody In Room" and automatically turns the light **OFF**.  
5. When the count is greater than zero, the relay keeps the light **ON**.

---

## Applications
- Smart home automation  
- Office/meeting room occupancy detection  
- Classroom or laboratory entry monitoring  
- Energy-saving lighting systems  
- Library or hall visitor counting  

---

## Future Improvements
- Add EEPROM to save count after power loss  
- Integrate WiFi/Bluetooth for IoT monitoring  
- Use ultrasonic sensors for higher accuracy  
- Add buzzer for entry/exit alerts  

---

## License
This project is open-source and free to use for personal and educational purposes.


