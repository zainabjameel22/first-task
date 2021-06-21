# first-task

#include <Servo.h>
Servo myServo1;
Servo myServo2;
Servo myServo3;
Servo myServo4;
Servo myServo5;

int pos=0;
void setup()
{
 myServo1.attach(9);
   myServo2.attach(10);
   myServo3.attach(11);
  myServo4.attach(12);
  myServo5.attach(13);
}

void loop()
{
  for(pos=0;pos<=90;pos++)
{
 myServo1.write(pos);
  delay(10);
  myServo2.write(pos);
  delay(10);
  myServo3.write(pos);
  delay(10);
  myServo4.write(pos);
  delay(10);
  myServo5.write(pos);
  delay(10);
  }
for(pos=90;pos>=0;pos--)
{
  myServo1.write(pos);
  delay(10);
  myServo2.write(pos);
  delay(10);
  myServo3.write(pos);
  delay(10);
  myServo4.write(pos);
  delay(10);
  myServo5.write(pos);
  delay(10);
}
  
}
