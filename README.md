# GPS Web Server with ESP8266

## Overview
This Arduino project creates a web server using an ESP8266 module, which displays real-time GPS data obtained from a NEO-6M GPS module. The webpage served by the ESP8266 shows latitude, longitude, date, and time obtained from the GPS module. Additionally, users can click on a link to view the location on Google Maps.

https://github.com/prathampg2003/Gps-sensor-/assets/89197939/482d07db-1c1a-43c4-ad98-4b7c59ed54e6



## Hardware Requirements
- ESP8266 module
- NEO-6M GPS module

## Software Requirements
- Arduino IDE
- Libraries: TinyGPS++, SoftwareSerial, ESP8266WiFi

## Installation and Setup
1. Connect the NEO-6M GPS module to the ESP8266 module using appropriate connections.
2. Open the Arduino IDE and install the required libraries mentioned above.
3. Copy and paste the provided code into the Arduino IDE.
4. Update the `ssid` and `password` variables in the code with your WiFi network credentials.
5. Upload the code to your ESP8266 board.

## Usage
1. Once the code is uploaded and the ESP8266 is connected to the WiFi network, open a web browser on a device connected to the same network.
2. Enter the IP address of the ESP8266 module in the address bar of the web browser and press Enter.
3. The webpage should display real-time GPS data, including latitude, longitude, date, and time.
4. If the GPS data is valid, a link will be provided to view the location on Google Maps.

## Notes
- Ensure that the NEO-6M GPS module has a clear view of the sky for accurate GPS data acquisition.
- Adjust the UTC offset in the code to match your local time zone if necessary.
- This code assumes a baud rate of 9600 for the GPS module. Modify `SerialGPS.begin(9600)` if your module operates at a different baud rate.
- Make sure to handle error cases gracefully, such as when the GPS module fails to acquire a fix or when the web server encounters errors.
