// IoT Week 1 - Hello Sensor 

# Project Overview
This project is my first step into the Internet of Things (IoT).  
It uses an **ATmega328P microcontroller** programmed with **Microchip Studio (Atmel Studio)** to measure temperature and humidity from a **DHT22 sensor**, printing values to the UART terminal every 10 seconds.

# Hardware
- ATmega328P (or similar AVR microcontroller)
- DHT22 temperature & humidity sensor
- Breadboard + jumper wires
- USBasp / Atmel ICE programmer
- Power supply (USB or external)

# Software
- Microchip Studio (formerly Atmel Studio)
- AVR-GCC toolchain
- DHT22 driver code (C implementation)
- GitHub for version control and documentation

# Setup Instructions
1. Connect the DHT22 sensor to the ATmega328P:
   - VCC → 5V (or 3.3V depending on your setup)
   - GND → GND
   - Data → PD2 (INT0 pin, configurable)
2. Open Microchip Studio and create a new AVR GCC project.
3. Add the DHT22 driver code to your project.
4. Compile and flash the firmware using USBasp or Atmel ICE.
5. Open a UART terminal (e.g., PuTTY) at **9600 baud** to see live readings.

## Example Output


## Next Steps
- Week 2: Send sensor data over UART → MQTT gateway.
- Week 3: Store data in a cloud database.
- Week 4: Visualize readings with Grafana.
