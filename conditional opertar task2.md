### Задание2
### Напишите программу, которая у пользователя запрашивает два числа. Находит
### произведение чисел, если оба числа четные. Находит сумму двух чисел если оба числа
### нечетные. Находит максимум из двух чисел если одно число нечетное, а другое четное.
### Находит деление двух чисел, если одно число является делителем второго числа.
### Результат вывести на экран

```
a = (int(input("введите первое число :    ")))
b = (int(input("введите второе число :    ")))

f=[a,b]
f.sort()

if a % 2 ==0 and b % 2 ==0:
    print("произведение ",a*b)
elif a % 2 >0 and b % 2 >0:
    print("сумма ",a+b)
elif a % 2 == 0 and b % 2 >0:
    print("макс число ", f[1])
elif a % 2 > 0 and b % 2 == 0:
    print("макс число ", f[1])

if a % b == 0:
    print( "деление",a / b)
elif b % a == 0:
    print( "деление",b / a)

```   