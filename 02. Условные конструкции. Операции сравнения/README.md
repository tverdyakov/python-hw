# 2. Условные конструкции. Операции сравнения.

## Задача №1
Задачи на [hackerrank](https://www.hackerrank.com/domains/python):  
Решить задачу на hackerrank ["Python If-Else"](https://www.hackerrank.com/challenges/py-if-else/problem).  

### Решение:
https://www.hackerrank.com/profile/simple_10

---

## Задача №2
На лекции мы рассматривали пример для военкомата. Сейчас мы знаем про его рост. Расширить это приложение следующими условиями:
1. Проверка на возраст призывника.
2. Количество детей.
3. Учится ли он сейчас.

### Решение:
https://replit.com/@simple10/Python#main.py

```python
age=input('Сколько вам полных лет? Введите ответ цифрами:')
if int(age) >= 18 and int(age) < 30:
  children=input('Сколько у вас детей? Введите ответ цифрами:')
  if int(children) <= 1:
    study=input('Вы учитесь? Введите ответ (Да/Нет):')
    if study == 'да' or study == 'Да':
       print('Вы не можете служить в армии. У вас отсрочка на время обучения.')
    elif study == 'нет' or study == 'Нет':
       print('Вы можете служить в армии. Поздравляем!')
  elif int(children) > 1:
    print('Вы не можете служить в армии. У вас двое или более детей.')
elif int(age) < 18:
  print('Вы не можете служить в армии. Ваш возраст менее 18 лет.')
else:
  print('Вы не можете служить в армии. Призывной возраст с 18 до достижения 30 лет.')
```

---

## Задание №3
Разработать приложение для определения знака зодиака по дате рождения.  
Пример:  
```
Введите месяц: март
Введите число: 6

Вывод:
Рыбы
```

### Решение:
https://replit.com/@simple10/Python#main.py

```python
month=input('Введите месяц:')
day=input('Введите число:')
if (int(day)>=21 and int(day)<=31 and str(month)=='Март') or (str(month)=='Апрель' and int(day)>=1 and int(day)<=20):
  print('Овен')
elif (int(day)>=21 and int(day)<=30 and str(month)=='Апрель') or (str(month)=='Май' and int(day)>=1 and int(day)<=20):
  print('Телец')
elif (int(day)>=21 and int(day)<=31 and str(month)=='Май') or (str(month)=='Июнь' and int(day)>=1 and int(day)<=21):
  print('Близнецы')
elif (int(day)>=22 and int(day)<=30 and str(month)=='Июнь') or (str(month)=='Июль' and int(day)>=1 and int(day)<=22):
  print('Рак')
elif (int(day)>=23 and int(day)<=31 and str(month)=='Июль') or (str(month)=='Август' and int(day)>=1 and int(day)<=22):
  print('Лев')
elif (int(day)>=23 and int(day)<=31 and str(month)=='Август') or (str(month)=='Сентябрь' and int(day)>=1 and int(day)<=23):
  print('Дева')
elif (int(day)>=24 and int(day)<=30 and str(month)=='Сентябрь') or (str(month)=='Октябрь' and int(day)>=1 and int(day)<=23):
  print('Весы')
elif (int(day)>=24 and int(day)<=31 and str(month)=='Октябрь') or (str(month)=='Ноябрь' and int(day)>=1 and int(day)<=22):
  print('Скорпион')
elif (int(day)>=23 and int(day)<=30 and str(month)=='Ноябрь') or (str(month)=='Декабрь' and int(day)>=1 and int(day)<=21):
  print('Стрелец')
elif (int(day)>=22 and int(day)<=31 and str(month)=='Декабрь') or (str(month)=='Январь' and int(day)>=1 and int(day)<=20):
  print('Козерог')
elif (int(day)>=21 and int(day)<=31 and str(month)=='Январь') or (str(month)=='Февраль' and int(day)>=1 and int(day)<=18):
  print('Водолей')
elif (int(day)>=19 and int(day)<=29 and str(month)=='Февраль') or (str(month)=='Март' and int(day)>=1 and int(day)<=20):
  print('Рыбы')
```

---
