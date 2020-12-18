# Arduino


## Fading LED



### Description
This was the first project that we did on adruino. It required coding, breadboard, arduino, wires, and a cable. The wiring didn't take much time, but the coding needed to be fixed. The coding had(**if statments**) for making the serial monitor to sync with the LED fading. 

### Evidence

[Fading LED](https://create.arduino.cc/editor/ezahid82/617ac921-1638-435e-976a-b8b7ad4c3d7a/preview)


### Image

![Fading LED image ](Pictures%20For%20Arduino/Arduino%20Wiring.jpg)

### Reflection
This was a really fun project to do. I ran into some coding problems where I coulding get the LED to fade. But I finally figured it out with some help for my teacher. I was missing some of the (**for statments**) and (**Serial.print(ln)**) I had to add those in order to get this LED fading in and out, and having the serial monitor printing what is happening while the LED is fading.




---





## Finite L.E.D.


### Description

This is the second assignement for the Arduino course. The L.E.D. turns on and off five times, then delays for 5 seconds, and repeats the process. I used new codes like (**digitalWrite**) (**Counter++**) and (**pinMode**). the counter is used to count the number of times the L.E.D. will blink, the pinMode is used to show what pin to use, digitalWrite is used to turn the L.E.D. on and off. 


### Evidence

[Finite LED](https://create.arduino.cc/editor/ezahid82/98dac722-343a-47a0-acae-11e9772d0d68/preview)


### Image

![Finite LED image ](Pictures%20For%20Arduino/FiniteLED.jpg)


### Reflection

this assignment was kind of hard at first. but I started to just code randomly with (**Counter++**) and somehow the assignment was related to that code. I contined to work on it by adding some (**if**) statements and (**digitalWrites**) which helped turn the L.E.D. on and off. 





---





## Hello Functions 


### Description

This is the third assignment for the Ardiuno course. The coding was different since I need to print out values (**Serial.print ("distance: ");**) than words. I had to make the servo spin for the value that the ultrasonic sensor produced. the servo was in a different branch of the code. It had to function separatly because they would confuse each other when a distance was print. The wiring and coding were all done on a website called (**tinkercad**) since there was a problem. 

### Evidence

.[ TinkerCAD wiring ](https://www.tinkercad.com/things/64qZtm935sM-glorious-bruticus-hillar/editel)

### Image

![Hello Function Wiring](Pictures%20For%20Arduino/Hello%20Function.png)



```C++

const int trigPin = 9;
const int echoPin = 11;
float duration, distance;
#include <Servo.h>
int servoPin = 9; 

Servo myservo;


void setup(){
{
  pinMode(trigPin, OUTPUT);
  pinMode(echoPin, INPUT);
  Serial.begin(9600);
}

{
  myservo.attach(servoPin);
  myservo.write(0);
}
}
  void loop(){
  {
    digitalWrite(trigPin, LOW);
    delayMicroseconds(2);
    digitalWrite(trigPin, HIGH);
    delayMicroseconds(10);
    digitalWrite(trigPin, LOW);

    duration = pulseIn(echoPin, HIGH);
    distance = (duration * .4);
    Serial.print("Distance: ");
    Serial.println(distance);
    delay(500);
  }
  
  {
   if (distance == 0)
   myservo.write(0);
   if (distance > 0 )
   myservo.write(duration * .4);
  }
}

```




### Reflection

This was a very confusing assignment since I ran into problems were the serial moitor wouldn't print any thing. I had to restart my chromebook many times but still no change ocurred. Then, I decided to switch to tinkerCAD were I already did the wiring and coding for testing. I decided to use tinkCAD for the rest of the Ardiuno course since it has the wiring and coding functions built in. 



---




### Description

### Evidence

.[tile](link)

### Image

![title](link)


### Reflection






---





### Description

### Evidence

.[tile](link)


### Image

![title](link)


### Reflection





---



