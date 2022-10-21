# Отчет №4
## Холод Егор
### Группа 8310


[Ссылка на проект.](https://www.tinkercad.com/things/5anm0WSwnMc-glorious-trug/editel?sharecode=lXckBtfWDvaD_U3-LKyWIuHgRsw1GmyUEqab3YocKVA)

![Изображение](https://user-images.githubusercontent.com/106704479/197274633-76e7dd0c-57a0-4f97-883c-e18f07848121.jpg)




//////1
```С++
#include<Keypad.h>
const byte ROWS = 4;
const byte COLS = 4;
char hexaKeys[ROWS][COLS] = {
{'D','#','0','*'}, 
{'C','9','8','7'},//3
{'B','6','5','4'}, //2
{'A','3','2','1'} //1
};
byte rowPins[ROWS] = {7, 6, 5, 4};
byte colPins[COLS] = {11, 10, 9, 8};
Keypad customKeypad = Keypad( makeKeymap(hexaKeys), rowPins, colPins, ROWS, COLS); 
void setup(){
Serial.begin(9600);
  pinMode(3, OUTPUT);
  pinMode(2, OUTPUT);
  pinMode(13, OUTPUT);
  pinMode(0, OUTPUT);
  pinMode(12, OUTPUT);
}
void loop(){
char customKey = customKeypad.getKey();
  if (customKey){
Serial.println(customKey);
} 
  if (customKey =='8' ){
digitalWrite(3, HIGH);
}
  
  if (customKey =='9' ){
digitalWrite(3, LOW);
}
  
   if (customKey =='A' ){
digitalWrite(2, HIGH);
}
  if (customKey =='B' ){
digitalWrite(2, LOW);
}
  
  
   if (customKey =='C' ){
digitalWrite(12, HIGH);
}
   if (customKey =='D' ){
digitalWrite(12, LOW);
}
     
   if (customKey =='1' ){
digitalWrite(13, HIGH);
}
  
   if (customKey =='2' ){
digitalWrite(13, LOW);
}
  
}
```

## Блок-схема
![Диограмма]()



## Пояснение


