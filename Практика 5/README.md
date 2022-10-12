# Отчет №5
## Холод Егор
### Группа 8310


[Ссылка на проект.](https://www.tinkercad.com/things/lQFXhApmgRb-neat-duup-albar/editel?sharecode=KEmOuWFmRSa9RF8dlvIPBPZ8co_H_y2M2J33ZksteYQ)

![1practic](https://user-images.githubusercontent.com/106704479/195206070-5ec7d0fe-2cd0-4ea4-bda7-e6b46f97fade.jpg)
![2practic](https://user-images.githubusercontent.com/106704479/195206064-ce495b57-23ee-4264-9df5-e69bdd5a3b57.jpg)


//////1
```С++
байт я;
байт LedMin = 2;
байт LedMax = 11;
недействительная установка ()
{
  для (i=LedMin;i<=LedMax;i++)
  {
    pinMode (я, ВЫВОД);
  }
}

пустой цикл ()
{
для (i=LedMin;i<=LedMax;i++)
{
   цифровая запись (я, ВЫСОКИЙ);
   задержка(30);
}
  для (i=LedMax;i>=LedMin;i--)
  {
    цифровая запись (я, НИЗКИЙ);
   задержка(30);
  }
}
```

## Блок-схема
![Диограмма]()

//////2
```С++
байт я;
байт LedMin = 2;
байт LedMax = 11;
недействительная установка ()
{
для (i=LedMin;i<=LedMax;i=i+2)
{
pinMode (я, ВЫВОД);
}
}

пустой цикл ()
{
для (i=LedMin;i<=LedMax;i=i+2)
{
цифровая запись (я, ВЫСОКИЙ);
задержка(50);
}
для (i=LedMax;i>=LedMin;i--)
{
цифровая запись (я, НИЗКИЙ);
задержка(50);
}
}
```

//////3
```С++
байт я;
байт LedMin = 1;
байт LedMax = 11;
недействительная установка ()
{
  для (i-LedMin;i<-LedMax;i++)
  {
    pinMode (я, ВЫВОД);
  }
}

пустой цикл ()
{
для (i-LedMin;i<-LedMax;i++)
{
   цифровая запись (я, ВЫСОКИЙ);
   задержка(50);
}
  для (i_LedMin;i<_LedMax;i++)
  {
    цифровая запись (я, НИЗКИЙ);
   задержка(50);
  }
}
```

## Пояснение



# Отчет №3
## Холод Егор 
### Группа 8310


[Ссылка на проект.](https://www.tinkercad.com/things/2h2PYAX99Xw-mighty-vihelmo/editel?sharecode=JL_i5blaRzfTj0_JZVbL4Gr7MOY9x_tiIVRUqERQISQ)

![1](https://user-images.githubusercontent.com/106704479/193897719-4c1dd533-2833-404c-ac8b-276448080759.jpg)
![2](https://user-images.githubusercontent.com/106704479/193897715-20efb36d-0d07-4f91-b536-fea0845b13d4.jpg)
![3](https://user-images.githubusercontent.com/106704479/193897710-2f79733f-9d65-4a3a-96aa-1c1a571e4f14.jpg)

//////4 
```C++
int led1 = 2;
int led2 = 3;
int led3 = 4;
void setup()
{ 
pinMode(led1, OUTPUT); 
pinMode(led2, OUTPUT);
pinMode(led3, OUTPUT);
} 
void loop()
{ 
digitalWrite(led1, HIGH);
delay(9000);
digitalWrite(led2, HIGH);
delay(4000);
digitalWrite(led2, LOW);
digitalWrite(led1, LOW);
digitalWrite(led3, HIGH);
delay(4000);
digitalWrite(led3, LOW);
digitalWrite(led2, HIGH);
delay(4000);
digitalWrite(led2, LOW);
digitalWrite(led1, HIGH);
delay(9000);
digitalWrite(led2, HIGH);
delay(4000);
digitalWrite(led2, LOW);
digitalWrite(led1, LOW);
digitalWrite(led3, HIGH);
delay(4000);
digitalWrite(led3, LOW);
digitalWrite(led2, HIGH);
delay(4000);
}
```

## Блок-схема
![Диограм](https://user-images.githubusercontent.com/106704479/193923224-e884a214-7436-4b28-a09f-7624275c065e.jpg))

//////3.1 
```C++
int led1 = 2; 
int led2 = 3; 
void setup()
{ 
pinMode(led1, OUTPUT);
pinMode(led2, OUTPUT);
} 
void loop()
{ digitalWrite(led1, HIGH);
delay(4000);
digitalWrite(led1, LOW);
delay(1000); 
digitalWrite(led2, HIGH); delay(6000);
digitalWrite(led2, LOW);
delay(1000);
} 
```

//////3.2 
```C++
int led1 = 2;
int led2 = 3;
void setup() 
{ 
pinMode(led1, OUTPUT);
pinMode(led2, OUTPUT);
} 
void loop() 
{ 
digitalWrite(led2, HIGH);
digitalWrite(led1, HIGH);
delay(10000);
digitalWrite(led1, LOW);
delay(4000); 
}
```

## Пояснение
По итогам работы был сделан светофор в tinkercad 



