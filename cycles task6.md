### Задание6
### Написать программу. Пользователь вводит два числа. Данные числа
### определяют числовой диапазон, для которого надо найти все числа, которые делятся
### нацело на 3, 5, 9 Например диапазон 1 - 20, количество чисел, которые делятся на 3 – 6, 5
### – 4, 9 - 2 Важно учесть, что пользователь может ввести числа в обратном порядке,
### например 37 и 16

```
d = (int(input("введите первое число ")))
f = (int(input("введите второе число ")))


if d > f:
    g=[f,d]
else:
    g=[d,f]
list1=[]
while g[0] < g[1]:
    g[1] = g[1]-1
    list1.append(g[1])

list2=[]
list3=[]
list4=[]
for i in list1:
    if i % 3 == 0:
        list2.append(i)
    elif i % 5 == 0:
        list3.append(i)
    elif i % 9 == 0:
        list4.append(i)
print(list2)
print(list3)
print(list4)

```