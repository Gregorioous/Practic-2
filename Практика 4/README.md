# Отчет №4
## Холод Егор
### Группа 8310


[Ссылка на проект.](https://www.tinkercad.com/things/2i03aAlebtP-fantabulous-fyyran-borwo/editel?sharecode=8a_zmcaWLKsZsKvost0YCYEPri4OQ52j2v2OXFAneQY)

![Изображение](https://user-images.githubusercontent.com/106704479/195460431-6909cf73-c73f-4e9a-9b3a-16c57269bcd6.jpg)



//////1
```С++
int buttonState = 0;

int lastButtonState = 0;

int buttonPushCounter = 0;

int  PIN_BUTTON = 2;

int buttonStote = digitalRead(PIN_BUTTON);

int counter;

void setup()
{
  pinMode(5, OUTPUT);
  pinMode(6, OUTPUT);
  pinMode(7, OUTPUT);
  pinMode(9, OUTPUT);
  pinMode(2, INPUT);
  pinMode(10, OUTPUT);
}

void loop()
{
  digitalWrite(5, LOW);
  digitalWrite(6, LOW);
  digitalWrite(7, HIGH);
  digitalWrite(9, HIGH);
  Serial.println(buttonStote);
    delay(50);
  buttonState = digitalRead(2);
  if (buttonState == HIGH) {
    delay(600); 
    digitalWrite(7, LOW);
    digitalWrite(6, HIGH);
    digitalWrite(5, LOW);
    delay(3000); 
    digitalWrite(7, LOW);
    digitalWrite(6, LOW);
    digitalWrite(5, HIGH);
    delay(1000); 
    digitalWrite(9, LOW);
    digitalWrite(10, HIGH);
    delay(10000); 
    digitalWrite(10, LOW);
    for (counter = 0; counter < 10; ++counter) {
      digitalWrite(9, HIGH);
      delay(500); 
      digitalWrite(9, LOW);
      delay(500); 
    }
    digitalWrite(9, LOW);
 
    
  }
  
  }

```

## Блок-схема
![Диограмма](https://user-images.githubusercontent.com/106704479/196049649-f369c786-0073-408b-a7b7-650e697d3552.png)



## Пояснение



