
##  Wi-Fi Connected Weight Measurement System
one of semicolon startup IOT projects (My startup)

### Description

This Arduino project is a Wi-Fi-connected weight measurement system that utilizes the HX711 load cell amplifier to measure weight and sends the data to the ThingSpeak IoT platform. The system is designed to be used for various applications where remote weight monitoring is required.

### Components

- **HX711 Load Cell Amplifier**: The project uses an HX711 amplifier to interface with the load cell and convert weight measurements into digital values.

- **Wi-Fi Module (ESP8266)**: The ESP8266 Wi-Fi module is used to connect to Wi-Fi and send data to the ThingSpeak platform.

### Setup

1. Connect the HX711 load cell amplifier to the Arduino board:
   - Connect the HX711's VCC pin to 5V.
   - Connect the HX711's GND pin to GND.
   - Connect the HX711's DT (data) pin to D5 on the Arduino.
   - Connect the HX711's SCK (clock) pin to D6 on the Arduino.

2. Ensure you have the required libraries installed in your Arduino IDE:
   - HX711 Library

3. Replace the placeholders in the code with your specific configuration:
   - `apiKey`: Replace it with your ThingSpeak Write API key.
   - `ssid`: Replace it with your Wi-Fi SSID.
   - `pass`: Replace it with your Wi-Fi password.

4. Upload the code to your Arduino board.

### Usage

Once the project is set up and the Arduino is powered on, it will continuously read weight measurements from the HX711 load cell amplifier. The weight data is then sent to the ThingSpeak platform, allowing you to monitor and analyze weight data over time.

### ThingSpeak Configuration

Make sure you have set up a ThingSpeak channel with the appropriate fields to receive and display the weight data. The channel should match the fields used in the code for data upload.

### Additional Note

- A button connected to D4 is used to reset the scale to zero.
- Calibration of the scale is performed using the `calibration_factor` value.

### Contributing

Feel free to modify and extend this project to suit your specific needs. You can enhance it by adding additional sensors, data logging features, or integrating it with other IoT platforms. Contributions and improvements are welcome!

### License

This project is open-source and available under an open-source license (mention the specific license used). Please refer to the LICENSE.md file for more details.

### Author

Gehad Abdelaah 
### Acknowledgments

Special thanks to the authors and contributors of the libraries used in this project for their work in making this project possible.
