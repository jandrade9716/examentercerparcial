# examentercerparcial
int rojo, verde, azul;
int Brojo, Bverde, Bazul;
int estador, estadov, estadoa;

void setup()
{
  rojo = 11;
  verde = 13;
  azul = 12;
  
  Brojo = 2;
  Bverde = 4;
  Bazul = 3;
  
  pinMode(13, OUTPUT);
  pinMode(12, OUTPUT);
  pinMode(11, OUTPUT);
  
  pinMode(4, INPUT);
  pinMode(3, INPUT);
  pinMode(2, INPUT);
}

void loop(){
  if(digitalRead(Brojo) == HIGH){
    digitalWrite(rojo, HIGH);
    digitalWrite(verde, LOW);
    digitalWrite(azul, LOW);
  } 
  else {
    digitalWrite(verde, LOW);
    digitalWrite(azul, LOW);
    digitalWrite(rojo, LOW);
  }
    if(digitalRead(Bverde) == HIGH){
    digitalWrite(rojo, LOW);
    digitalWrite(verde, HIGH);
    digitalWrite(azul, LOW);
  }
   else {
    digitalWrite(verde, LOW);
    digitalWrite(azul, LOW);
    digitalWrite(rojo, LOW);
  }
    if(digitalRead(Bazul) == HIGH){
    digitalWrite(rojo, LOW);
    digitalWrite(verde, LOW);
    digitalWrite(azul, HIGH);
  }
   else {
    digitalWrite(verde, LOW);
    digitalWrite(azul, LOW);
    digitalWrite(rojo, LOW);
  }
}
