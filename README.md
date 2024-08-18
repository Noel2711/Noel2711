
#define led1 = A0
#define led2 = A1
#define led3 = A2
#define led4 = A3
#define led5 = A4
void setup() {
  pinMode(led1, INPUT);
  pinMode(led2, INPUT);
  pinMode(led3, INPUT);
  pinMode(led4, INPUT);
  pinMode(led5, INPUT);
}

void loop() {
  int d1 = digitalRead(led1);
  int d2 = digitalRead(led2);
  int d3 = digitalRead(led3);
  int d4 = digitalRead(led4);
  int d5 = digitalRead(led5);
  if(d3==HIGH)
  {
      moveForward();
  }
  else if(d2==HIGH and d4==HIGH)
  {
      Stop();
  }
  else if(d1==HIGH and d2==HIGH)
  {
      turnLeft();
  }
  else if(d4==HIGH and d5==HIGH)
  {
      turnRight();
  }
  else
  {
      Stop();
  }
}
