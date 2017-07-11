# Here-we-are
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
void loop() {
/* 
digitalWrite(13, HIGH);   // Encienda el LED (HIGH es el nivel de voltaje)
delay(1000);              // Espera un segundo
digitalWrite(13, LOW);    // Apague el LED haciendo que el voltaje BAJO
delay(1000);*/
servo1.write(180);                  // Ajusta la posición del servo de acuerdo con el valor escalado
delay(150);   
/*
digitalWrite(12, HIGH);   // Encienda el LED (HIGH es el nivel de voltaje)
delay(1000);              // Espera un segundo
digitalWrite(12, LOW);    // Apague el LED haciendo que el voltaje BAJO
delay(1000);*/
servo2.write(60);                  // Ajusta la posición del servo de acuerdo con el valor escalado
delay(150);  // Espera el servo para llegar allí
servo1.write(80);                  // Ajusta la posición del servo de acuerdo con el valor escalado
delay(150);   
/*
digitalWrite(12, HIGH);   // Encienda el LED (HIGH es el nivel de voltaje)
delay(1000);              // Espera un segundo
digitalWrite(12, LOW);    // Apague el LED haciendo que el voltaje BAJO
delay(1000);*/
servo2.write(80);                  // Ajusta la posición del servo de acuerdo con el valor escalado
delay(150);  // Espera el servo para llegar allí
}
