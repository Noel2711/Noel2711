
#define l1  2
#define l2  3
#define l3  4
#define l4  5
void setup() 
{
  pinMode(l1, INPUT);
  pinMode(l2, INPUT);
  pinMode(l3, INPUT);
  pinMode(l4, INPUT);
}
void loop() 
{
  int d1 = digitalRead(l1);
  int d2 = digitalRead(l2);
  int d3 = digitalRead(l3);
  int d4 = digitalRead(l4);
  if (d1 == LOW and d2 == LOW and d3 == LOW and d4 == LOW) 
  {
    Serial.print("chạy thẳng");
  } 
  else if (d1 == LOW and d2 == LOW  and d3 == HIGH and d4 == LOW) 
  {
    Serial.print("trái");
  } 
  else if (d1 == LOW and d2  == LOW and d3 == LOW and d4 == HIGH) 
  {
    Serial.print("trái");
  } 
  else if (d1 == LOW and d2 == HIGH and d3 == LOW and d4 == LOW) 
  {
     Serial.print("phải");
  } 
  else if (d1 == HIGH and d2 == LOW and d3 == LOW and d4 == LOW) 
  {
     Serial.print("phải");
  } 
  else if (d1 == HIGH and d2 == HIGH and d3 == LOW and d4 == LOW) 
  {
    Serial.print("phải");
  } 
  else if (d1 == LOW and d2 == HIGH and d3 == HIGH and d4 == LOW) 
  {
     Serial.print("chạy thẳng");
  }
  else if (d1 == LOW and d2 == LOW and d3 == HIGH and d4 == HIGH) 
  {
    Serial.print("trái");
  }
  else if (d1 == HIGH and d2 == HIGH and d3 == HIGH and d4 == LOW) 
  {
    Serial.print("chạy thẳng");
  }
  else if (d1 == HIGH and d2 == HIGH and d3 == HIGH and d4 == LOW) 
  {
    Serial.print("chạy thẳng");
  }
  else if (d1 == HIGH and d2 == HIGH and d3 == LOW and d4 == HIGH) 
  {
    Serial.print("phải");
  }
  else if (d1 == HIGH and d2 == LOW and d3 == HIGH and d4 == HIGH) 
  {
    Serial.print("phải");
  }
  else if (d1 == LOW and d2 == HIGH and d3 == HIGH and d4 == HIGH) 
  {
    Serial.print("trái");
  }
  else if (d1 == HIGH and d2 == HIGH and d3 == HIGH and d4 == HIGH) 
  {
    Serial.print("chạy thẳng");
  }
  else 
  {
    Serial.print("dừng");
  }
}
