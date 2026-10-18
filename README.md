# Marvel-IOT-level2-final-report
# TASK 1: SMART LIVING & ENVIRONMENTAL AUTOMATION

**Objective:** Automate plant watering based on soil moisture levels.

**Learnings and Outcomes:**
    1.Connected the soil moisture sensor to the Arduino UNO and calibrated it.\
    2.Tested the sensor by observing readings in wet and dry soil conditions. 
    3.Set a threshold value of 500 to distinguish between wet and dry soil.\
    4.Connected the relay module to Arduino UNO digital pin D8.
    5.Tested the relay switching operation and verified its functionality. 
    6.Connected the solenoid valve to a 24V power supply through the relay using the COM and NO terminals.
    
**Components Used:**
Arduino UNO
Relay Module
Solenoid valve
Capacitive Soil Moisture Sensor
<iframe
  src="https://www.youtube-nocookie.com/embed/vb11eQwDkvY"
  width="560"
  height="315"
  title="Smart Plant Watering System"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  referrerpolicy="strict-origin-when-cross-origin"
  allowfullscreen>
</iframe>

![image](https://raw.githubusercontent.com/Thanu-cpu/IOT-level-2-/b7efec7edce81e3da478a28f178833e84365117c/WhatsApp%20Image%202026-10-18%20at%208.57.01%20PM.jpeg)

**Working of Solenoid Valve:**
A solenoid is a device that converts electrical energy into mechanical energy. It consists of a coil of wire wound around a conductive core, which acts as an electromagnet when electric current flows through it. When the coil is energized, the magnetic field pulls the internal plunger, allowing liquid to flow through the valve. When the coil is de-energized, a spring pushes the plunger back to its original position, stopping the flow of liquid. A 12V solenoid valve is commonly used for liquid-flow control, and its high current consumption requires a suitable driver circuit or relay for safe operation.
![image](https://raw.githubusercontent.com/Thanu-cpu/IOT-level-2-/2609ca03ba6555d89b43e3d7a2990501958aea3f/WhatsApp%20Image%202026-10-18%20at%209.00.30%20PM.jpeg)
[click here](https://github.com/Thanu-cpu/IOT-level-2-/blob/a6610fdf0f1a3031c760e8cb4938254fa73f5ac1/smart%20irrigation) to view the code.

# TASK 2: SMART PARKING SYSTEM

**Objective:** Monitor parking space availability using ultrasonic sensors.

**Learnings and Outcomes:**
I completed the necessary connections between the ESP32 and the ultrasonic sensor to detect the presence of a vehicle in a parking slot. I then programmed the ESP32 and integrated the system with the Blynk IoT platform to monitor the parking status in real time. The sensor readings were displayed on the Blynk application, making it easy to identify whether the parking slot was occupied or vacant. Through this task, I gained practical knowledge of connecting hardware with an IoT application and displaying real-time sensor data.

**Components Used:**
Esp32
Ultrasonic sensor
<iframe
  src="https://www.youtube-nocookie.com/embed/bApcDXk3APQ"
  width="560"
  height="315"
  title="Smart Plant Watering System Demonstration"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  referrerpolicy="strict-origin-when-cross-origin"
  allowfullscreen>
</iframe>

![image](https://raw.githubusercontent.com/Thanu-cpu/IOT-level-2-/40c6df1f8cedd5b21f160b0502f552a244979c79/WhatsApp%20Image%202026-10-18%20at%209.29.58%20PM.jpeg)
[click here](https://github.com/Thanu-cpu/IOT-level-2-/blob/d0af77a20d6163da4cdd14d658b9eb0ec53eea28/smart%20parking) to view the code.

**Blynk IOT:**
Blynk IoT is a cloud-based platform that connects hardware devices like ESP32 to mobile applications for real-time monitoring and control.
![image](https://raw.githubusercontent.com/Thanu-cpu/IOT-level-2-/68acce1e10f541774d0b3f2fbecbe1c0868b8cd9/Smart%20Parking%20System%20Flow%20Diagram.png)

# TASK 3: INTRO TO RFID AND ATTENDANCE LOGGER
**Objective:** Understand RFID technology and learn to log data on cloud platforms.

## PART i – Introduction to RFID
1. RFID stands for Radio Frequency Identification, a wireless technology used to identify and track objects using radio waves.
2. An RFID system consists of three main components: an RFID tag, an RFID reader, and a processing system.
3. RFID tags contain a microchip and an antenna that enable them to store identification data and communicate with a reader.
4. The RFID reader generates a radio-frequency electromagnetic field to communicate with nearby tags.
5. Passive RFID tags obtain the energy required for communication from the reader's electromagnetic field, whereas active tags use an internal power source.
6. When a tag enters the reader's detection range, it responds by transmitting its stored information through radio-frequency communication.
7. The reader captures the transmitted data, decodes it, and sends it to a microcontroller or computer for processing.
8. The MFRC522 RFID-RC522 module operates at 13.56 MHz and commonly communicates with microcontrollers using the SPI protocol.
9. The ESP32 can interface with the RFID-RC522 module to read card identifiers and perform access-control operations.
10. Each RFID tag has a unique identifier (UID), which can be used to distinguish one tag from another.
11. Certain RFID cards, such as MIFARE Classic 1K, provide 1 KB of EEPROM memory for storing data in addition to identification information.
12. The MIFARE Classic 1K memory is organized into 16 sectors, each containing four blocks of 16 bytes, with the last block of each sector reserved for sector trailers.
13. RFID systems can support reading and writing operations, depending on the tag type, memory permissions, and authentication requirements.
14. RFID-based access-control systems compare scanned card identifiers against authorized records to grant or deny access to a secured location.
15. RFID technology is widely used in attendance systems, public transportation, inventory management, library systems, and contactless access control.
![image](https://raw.githubusercontent.com/Thanu-cpu/IOT-level-2-/d0d0b076c9fca1e057f71f47c080eb7c5c93b95c/Screenshot%202026-10-18%20220018.png)

## Part ii – Attendance Logger
**Components Used:**
ESP32
RC522 RFID Card and reader
Software tools: Google sheet & Google Apps script

**Steps involved:**
1. Connected the RC522 RFID reader to the ESP32 using SPI communication.
2. Installed the MFRC522 library in Arduino IDE.
3. Uploaded the RFID test code and verified the card UID in the Serial Monitor.
4. Created a Google Sheet with columns for Card ID, Date, and Time.
5. Opened Google Apps Script and wrote the code to record attendance data.
6. Deployed the script as a web application and copied the web app URL.
7. Connected the ESP32 to a mobile hotspot using Wi-Fi.
8. Uploaded the integration code to send the RFID card UID to Google Apps Script.
9. Scanned the RFID card and checked the attendance records in Google Sheets.
 <iframe
  src="https://www.youtube-nocookie.com/embed/BH5k1zVYoMQ"
  width="560"
  height="315"
  title="RFID Attendance Logger Tutorial"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  referrerpolicy="strict-origin-when-cross-origin"
  allowfullscreen>
</iframe>

![image](https://raw.githubusercontent.com/Thanu-cpu/IOT-level-2-/b6edd1f8306f69c8dd619f3206d52e1599c50fda/WhatsApp%20Image%202026-10-18%20at%2010.15.21%20PM.jpeg)
[click here](https://github.com/Thanu-cpu/IOT-level-2-/blob/2b990c5abf79ed4f0c72144bc80b43ede1f6f782/rfid%20attendance%20logger) to view the code.

# TASK 4: SMART STREET LIGHTING WITH NODE-RED DASHBOARD
**Objective:** Create a Smart Street Lighting System and get real-time operational data using a Node-RED dashboard.

**Learnings & Outcomes:**
ESP32 to process analog input from an LDR (Light Dependent Resistor) connected to GPIO 34 and digital input from a PIR (Passive Infrared) motion sensor connected to GPIO 27. Based on ambient light intensity and motion detection, the ESP32 controls a relay through GPIO 26 to switch the LED streetlight ON or OFF. Sensor readings and lighting status are transmitted over Wi-Fi using HTTP POST requests in JSON format to Node-RED, where the incoming data is parsed and processed for real-time IoT monitoring through a dashboard.

**Components Used:**
ESP32
Led
Relay Module
LDR(Light Dependent Resistor)
PIR(Passive Infrared) motion sensor
<iframe src="https://www.youtube-nocookie.com/embed/dP8D0J6negc" width="560" height="315" title="YouTube Video" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

![image](https://raw.githubusercontent.com/Thanu-cpu/IOT-level-2-/94bc77770947e8499cc982ba38eacb16548e66c2/WhatsApp%20Image%202026-10-18%20at%2010.36.25%20PM%20(1).jpeg)

![image](https://raw.githubusercontent.com/Thanu-cpu/IOT-level-2-/56bbaf8133d609eebb7eb8bdaac62f129cd1b4d3/WhatsApp%20Image%202026-10-18%20at%2010.44.30%20PM.jpeg)
[click here](https://github.com/Thanu-cpu/IOT-level-2-/blob/3039b3637af59f3925509c17184e0bd10b0f2571/node%20red) to view the code.
**Working of LDR and PIR sensor:**
## LDR:
LDR (Light Dependent Resistor): An LDR operates on the principle of photoconductivity, where its resistance decreases with increasing light intensity and increases in darkness. The ESP32 reads the corresponding voltage variation through an ADC pin to measure ambient light levels.
## PIR Motion Sensor:
PIR (Passive Infrared Sensor): A PIR sensor detects changes in infrared radiation emitted by warm objects, such as humans, using a pyroelectric element. It produces a digital HIGH or LOW output based on detected motion, which the ESP32 processes to control the connected device.
![image](https://raw.githubusercontent.com/Thanu-cpu/IOT-level-2-/7bfed5825ff0b411dc017286697860bb1989d4b9/WhatsApp%20Image%202026-10-18%20at%2010.53.20%20PM.jpeg)

# TASK 5: CREATING YOUR OWN HOME ASSISTANT
**Objective:** Implement voice-controlled home automation.

**Learnings and Outcomes:**
The task is to develop a voice-controlled automation system with AI integration using Python and ESP32. The Speech Recognition library captures voice commands through a microphone and converts them into text. Python processes the recognized commands and communicates with the ESP32 through serial communication to control the LED using GPIO pins and operate the servo motor using PWM signals, rotating it by 90° to open or close. For AI-based queries, the user can say “Hey Alexa” followed by a question, which is processed using an AI model through the OpenRouter API. The AI-generated response is then converted into audible speech using the pyttsx3 text-to-speech library, enabling natural voice-based interaction with the assistant.

**Component Used:**
Esp32
Led
Servomotor
Software language: Python
Execution Environment: Command Prompt
AI integration: OpenRouter API
Libraries: Speechrecognition & pyttsx3
<iframe src="https://www.youtube-nocookie.com/embed/d6gxF80-aiM" width="560" height="315" title="YouTube Video" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

![image](https://raw.githubusercontent.com/Thanu-cpu/IOT-level-2-/5f19a97efd4396c502d5d477c64473d5d4560a86/WhatsApp%20Image%202026-10-18%20at%2011.25.42%20PM.jpeg)
![image](https://raw.githubusercontent.com/Thanu-cpu/IOT-level-2-/857761965114e628036fe8f56c7d68b173de3be6/WhatsApp%20Image%202026-10-18%20at%2011.26.05%20PM.jpeg)
[click here](https://github.com/Thanu-cpu/IOT-level-2-/blob/3a026da43c1fdf764f934e37c31b3d5677375c3d/home%20assistant)to view the python code.

# TASK 6: HOUSE SECURITY SYSTEM
**Objective:** Create a security system to detect motion, capture intruder images, and trigger an alert.

**Learnings and Outcomes:**
The home security system uses a PIR sensor to detect intruders and trigger the ESP32-CAM to capture images. The captured images are uploaded to ImgBB cloud storage through an API using Wi-Fi. The ImgBB API enables image uploading and generates a URL to access the stored images. The Blynk IoT app is integrated to provide real-time notifications and remote monitoring, allowing users to view captured images on their smartphones. A buzzer generates an audible alarm when motion is detected.
<iframe
  src="https://www.youtube-nocookie.com/embed/VamCexA9STk"
  width="560"
  height="315"
  title="ESP32-CAM Security System"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  referrerpolicy="strict-origin-when-cross-origin"
  allowfullscreen>
</iframe>

![image](https://raw.githubusercontent.com/Thanu-cpu/IOT-level-2-/748f11bc2fe515ae702c9f753e75b8b8c0def769/WhatsApp%20Image%202026-10-18%20at%2011.49.18%20PM.jpeg)
[click here](https://github.com/Thanu-cpu/IOT-level-2-/blob/921b95d5777905fdde830e104e886cdc2e40c972/house%20security) to view the code.

## Esp32 CAM
Technical Specifications of ESP32-CAM

1. Camera: Supports the OV2640 camera module for image capture.
2. Wi-Fi: Supports 2.4 GHz Wi-Fi for wireless communication.
3. Wi-Fi Sensitivity: Approximately -90 dBm to -70 dBm, depending on the data rate.
4. Operating Voltage: Supports 5V or 3.3V power input, depending on the board.
5. Power Consumption: Approximately 180 mA at 5V with flash off.
6. Flash Power: Approximately 310 mA at 5V with flash at maximum brightness.
7. Sleep Modes: Supports deep-sleep, light-sleep, and modem-sleep modes to reduce power consumption.
8. Dimensions: Approximately 40.5 × 27 × 4.5 mm.
9. GPIO Pins: Used to connect external sensors and devices.
10. Serial Pins: GPIO 1 (TX) and GPIO 3 (RX) support serial communication. Connecting GPIO 0 to GND during reset enables flashing mode.
![image](https://raw.githubusercontent.com/Thanu-cpu/IOT-level-2-/458c949c22bf889f3c7536fbdadd698277f0da30/Screenshot%202026-10-19%20000209.png)
            
# THANK YOU!!!!
