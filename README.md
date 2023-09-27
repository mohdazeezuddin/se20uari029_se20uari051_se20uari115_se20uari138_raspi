# se20uari029_se20uari051_se20uari115_se20uari138_raspi
REPORT:
RASPI ASSIGNMENT

Sensor Used: IR Sensor
IR sensors are used in motion detectors. Some of the advantages of this sensor are low power consumption, simple design and useful features.

Working of Code:
 This code continuously reads the state of an IR sensor connected to GPIO pin 16 on the Raspberry Pi and prints the state (1 for detected, 0 for not detected) to the console. It runs indefinitely until you manually stop it, at which point it cleans up the GPIO settings before exiting.
 
1)Sensor Setup: We specify that the IR sensor is connected to GPIO pin 16 on the Raspberry Pi.

2)GPIO Configuration: We configure the GPIO pin as an input pin, which means it will be used to read signals from the IR sensor.

3)Continuous Reading: Our code enters an infinite loop, where it continually checks the state of the IR sensor.

4)State Detection: Within the loop, we use GPIO.input(IR_sensor) to read the state of the IR sensor. It will return either 0 (LOW) or 1 (HIGH) based on whether the sensor detects an infrared signal or not.

5)Print State: The script then prints the state of the IR sensor to the console, allowing us to see whether the sensor is currently detecting an infrared signal or not.

6)Delay: After each sensor reading, there is a 0.1-second delay (time.sleep(0.1)) to ensure that the script doesn't read the sensor too rapidly.

7)Keyboard Interrupt Handling: We've included an exception handler to catch a KeyboardInterrupt (triggered by pressing Ctrl+C). When this occurs, the script will clean up GPIO resources, ensuring that they are properly released.

8)In essence, our code continuously monitors the IR sensor's state and reports it in real-time. This can be useful for various applications such as detecting the presence of objects, receiving input from an IR remote control, or any other situation where we need to know whether the sensor is active or not. 

Team Members:
Azeezuddin Mohammed (se20uari029)
T Eshaan Singh (se20uari051)
Kautilya pothineni (se20uari115)
Shahilul Alam Tapadar (se20uari138)
