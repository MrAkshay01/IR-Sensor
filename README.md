
int pirsensor=0;
void setup()
{
  pinMode(12,OUTPUT);
  pinMode(13,OUTPUT);
  pinMode(2,INPUT);
}
void loop()
{
  pirsensor=digitalRead(2);
  if(pirsensor==HIGH)
  {
    digitalWrite(13,HIGH);
    tone(12,500,500);
  }
  digitalWrite(13,LOW);
}
