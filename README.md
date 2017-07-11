# Here-were-are
/*
 Control de posición de servo usando  un potenciómetro (resistor variable)
 by Sergio, Yenny, Michel, Marco.
*/
#include <Servo.h>
Servo servo1; 
Servo servo2;// crear objeto servo para controlar un servo
void setup() {
servo1.attach(10); 
servo2.attach(9);// Fija el servo en el pasador 9 al objeto servo
//leds1
pinMode(13, OUTPUT);  pinMode(12, OUTPUT); pinMode(11, OUTPUT);
//leds2
pinMode(7, OUTPUT);  pinMode(6, OUTPUT); pinMode(5, OUTPUT);
}
