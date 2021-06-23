# controlling-the-servo-moto
Power electronics section - first task

This project is considered as required by smart methods company in cooperative training for the year 2021 
controlling servo motor 

Tinkercad is the website that used to create servos motor circuit

The objective to move the motors at an angle of 90 degrees

componets 

Name	      Quantity      	Component
 U1	            1	         Arduino Uno R3
                           
SERVO1 
SERVO2
SERVO3        5           Positional Micro Servo
SERVO5
SERVO6	 


the code 

#include <Servo.h>

int servosignal = 2; 
int servosignall = 3; 
int servosignalll = 4; 
int servosignallll = 5; 
int servosignalllll = 6; 

Servo servo1;
Servo servo2;
Servo servo3;
Servo servo4;
Servo servo5;

void setup()
{

  servo1.attach(2, 500, 2500);

  servo2.attach(3, 500, 2500);

  servo3.attach(4, 500, 2500);

  servo4.attach(5, 500, 2500);

  servo5.attach(6, 500, 2500);

  }

void loop()
{

  servosignal= 2;
  for (servosignal = 1; servosignal <= 89; servosignal += 1) {
    servo1.write(servosignal);
 delay(17);

  }
  

  servosignall = 3;
  for (servosignall = 1; servosignall <= 89; servosignall += 1) {
    servo2.write(servosignall);
 delay(17);
  }
  
   servosignalll = 4;
  for (servosignalll = 1; servosignalll <= 89; servosignalll += 1) {
    servo3.write(servosignalll);
 delay(17);
  }
  servosignallll = 5;
  for (servosignallll = 1; servosignallll <= 89; servosignallll += 1) {
    servo4.write(servosignallll);
 delay(17);
  }
   servosignalllll = 6;
  for (servosignalllll = 1; servosignalllll <= 89; servosignalllll += 1) {
    servo5.write(servosignalllll);
 delay(17);
  }
  servo1.write(90);
  servo2.write(90);
  servo3.write(90);
  servo4.write(90);
  servo5.write(90);
  
  delay (17);
 
    
 }

tinkercad link 

https://www.tinkercad.com/things/l7nLEOY9QLn-servo-motor/editel

