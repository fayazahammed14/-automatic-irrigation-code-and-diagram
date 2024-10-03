int RelayPin = 13;  
int sensorPin = 0;  
int val; 
void setup() { 
pinMode(13,OUTPUT);//connect the (SIGNAL PIN)of relay to (13PIN) 
of arduino 
pinMode(0,INPUT);//connect the (SIGNAL PIN)of SENSOR to (0PIN) of 
arduino 
} 
void loop() {  
val = digitalRead(0);  
if(val == LOW) { 
digitalWrite(13,LOW);//if sensor give LOW value send LOW value to 
relay 
} 
else{ 
digitalWrite(13,HIGH);//if sensor give HIGH value send HIGH value to 
relay 
}}
