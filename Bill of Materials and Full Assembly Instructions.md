
Bill of Materials (BOM) 

Esp32 DevKitC(X2)- Arduino board for coding the project and bluetooth connectivity 

MG90s Servo (X2)- Servo Motor for controlling Linear Actuators 

MPU6050 Gyroscope (X1)- Gyroscope for determining head rotation 

Half-size Breadboard (X2)-Standard Solderless Breadboards for connecting electronics 
*Removed breadboard connection bumps to get a smooth rectangle to fit inside 3d prints

~15 Jumper Wires (M-M) – For wiring 

AVCOO EMS/TENS Unit (x1) -For electric muscle stimulation 

Standard EMS/TENS Unit Self-Adhesive Electrode Pads- (COMES WITH EMS DEVICE) Used to connect to EMS and apply electric pulses to body 

AA 6V battery case (X1)- Used to power the SERVO breadboard 

AAA 4.5V battery case WITH POWER SWITCH (X1)- Used to power the GYROSCOPE breadboard 
***VERY IMPORTANT- MAKE SURE THE AAA BATTERIES USED ARE LITHIUM TO MINIMIZE VOLTAGE DROP TO GET A STABLE 4.5 THROUGHOUT LIFETME AND AVOID BROWNOUTS

**Velcro strap-** -To wear the GYROSCOPE breadboard on head 

# Assembly- GYROSCOPE BOARD 

X1 Breadboard 

X1 ESP32 

X1 MPU6050 Gyroscope 

Jumper Wire 

3d printed Gyroscope case and cap 

Velcro Strap 



# Assembly- SERVO BOARD 

X1 Breadboard 

X1 ESP32 

X2 MGS90 Servos 

# **X1 AVCOO EMS/TENS Machine** 

Jumper Wires 

Micro Servo Fastners 

3d printed “PARTS” above 



3d printed Servo case and cap 



Setting up device: Master and Slave Bluetooth Coding 

# MASTER ESP32 (Gyroscope board) 

Install VSCode and get the Platform IO Extension 

Create a Project for the Master Code. 

- Project settings: board- ESP32 DevkitC and code- Arduino 

In the newly created project, install the MPU 6050 Library 

- **11520** 

- Also in the .IO file, add a monitor speed to 

Download code for Gyroscope board (ESP32 Master Code) and paste it in project. Build and upload to the ESP32 

SLAVE ESP32 (Servo board) 

Create another Project for the Slave Code 

- Same project settings 

Install the ESP32 SERVO library along with the **(FIND THE JSON BLUETOOTH LIBRARY THINGY)** 

- Again, add the **Monitor to 11520** into the .IO file 

Download code for the Slave board (ESP32 Slave Code) and paste it in project Build and upload to the ESP32 

*With both Master and Slave ESP32s done, they should be able to connect to each other, which will be signaled by a blue light appearing on both boards. 

