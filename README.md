# Seven-Segment-Display-Serial-Monitor-Controling

int x = 0;

void setup()
{
  Serial.begin(9600);
  pinMode(13, OUTPUT);//A
  pinMode(12, OUTPUT);//B
  pinMode(11, OUTPUT);//C
  pinMode(10, OUTPUT);//D
  pinMode(9, OUTPUT);//E
  pinMode(7, OUTPUT);//F
  pinMode(6, OUTPUT);//G
  
}

void loop()
{
  if(Serial.available()){
    int x = Serial.read();
  
    if (x == '0'){
      digitalWrite(13,HIGH);
      digitalWrite(12,HIGH);
      digitalWrite(11,HIGH);
      digitalWrite(10,HIGH);
      digitalWrite(9,HIGH);
      digitalWrite(7,HIGH);
      digitalWrite(6,LOW);
      delay(1000);
    }
  
    else if (x == '1') {
      digitalWrite(13,LOW);
      digitalWrite(12,HIGH);
      digitalWrite(11,HIGH);
      digitalWrite(10,LOW);
      digitalWrite(9,LOW);
      digitalWrite(7,LOW);
      digitalWrite(6,LOW);
      delay(1000);
    }
    
    else if (x == '2'){
      digitalWrite(13,HIGH);
      digitalWrite(12,HIGH);
      digitalWrite(11,LOW);
      digitalWrite(10,HIGH);
      digitalWrite(9,HIGH);
      digitalWrite(7,LOW);
      digitalWrite(6,HIGH);
      delay(1000);
    }
  
    else if (x == '3') {
      digitalWrite(13,HIGH);
      digitalWrite(12,HIGH);
      digitalWrite(11,HIGH);
      digitalWrite(10,HIGH);
      digitalWrite(9,LOW);
      digitalWrite(7,LOW);
      digitalWrite(6,HIGH);
      delay(1000);
    }
  
    else if (x == '4'){
      digitalWrite(13,LOW);
      digitalWrite(12,HIGH);
      digitalWrite(11,HIGH);
      digitalWrite(10,LOW);
      digitalWrite(9,LOW);
      digitalWrite(7,HIGH);
      digitalWrite(6,HIGH);
      delay(1000);
    }
  
    else if (x == '5') {
      digitalWrite(13,HIGH);
      digitalWrite(12,LOW);
      digitalWrite(11,HIGH);
      digitalWrite(10,HIGH);
      digitalWrite(9,LOW);
      digitalWrite(7,HIGH);
      digitalWrite(6,HIGH);
      delay(1000);
    }
    
    else if (x == '6'){
      digitalWrite(13,HIGH);
      digitalWrite(12,LOW);
      digitalWrite(11,HIGH);
      digitalWrite(10,HIGH);
      digitalWrite(9,HIGH);
      digitalWrite(7,HIGH);
      digitalWrite(6,HIGH);
      delay(1000);
    }
  
    else if (x == '7') {
      digitalWrite(13,HIGH);
      digitalWrite(12,HIGH);
      digitalWrite(11,HIGH);
      digitalWrite(10,LOW);
      digitalWrite(9,LOW);
      digitalWrite(7,LOW);
      digitalWrite(6,LOW);
      delay(1000);
    }
  
    else if (x == '8'){
      digitalWrite(13,HIGH);
      digitalWrite(12,HIGH);
      digitalWrite(11,HIGH);
      digitalWrite(10,HIGH);
      digitalWrite(9,HIGH);
      digitalWrite(7,HIGH);
      digitalWrite(6,HIGH);
      delay(1000);
    }
  
    else if (x == '9') {
      digitalWrite(13,HIGH);
      digitalWrite(12,HIGH);
      digitalWrite(11,HIGH);
      digitalWrite(10,HIGH);
      digitalWrite(9,LOW);
      digitalWrite(7,HIGH);
      digitalWrite(6,HIGH);
      delay(1000);
    } 
  }
}





