# DC-motor
### connect DC motor with H-bridge to arduino simulation using tinkercad
* Connect the DC Motor to the Arduino:
   - Connect the positive terminal of the DC motor to a digital pin on the Arduino.
   - Connect the negative terminal of the DC motor to the ground (GND) of the Arduino.
   - You may also need to use a transistor or an H-bridge circuit to provide enough current to drive the motor.

* Write the Arduino Code:
   - In the setup() function, set the digital pin connected to the motor as an output:
  ex git :
```  
C++

     pinMode(motorPin, OUTPUT);
```
 
   - In the loop() function, use the analogWrite() function to control the speed of the motor:
   ex Git :
 ```  
C++

     analogWrite(motorPin, motorSpeed);
```


### code 
ex Git:
```
// C++ code

void setup()
{
  pinMode(11, OUTPUT);
  pinMode(9, OUTPUT);
}

void loop()
{
  digitalWrite(11, HIGH);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(9, LOW);
  delay(1000); // Wait for 1000 millisecond(s)
```
![image](https://github.com/user-attachments/assets/0e679a60-6312-4afd-93e2-aeee3ac17456)

