#include<Servo.h>
Servo myservo;
int pos ;
void setup() {
  myservo.attach(9);
}

void loop() {
  for (pos=0; pos <= 180; pos ++){
    myservo.write(pos);
    delay(15);
  }
  delay(1000);
    for (pos=180; pos >= 0; pos --){
    myservo.write(pos);
    delay(15);
    
  }
  delay(1000);

}
