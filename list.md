### Задача 1 Дан список некоторых целых чисел, найдите значение 20 в нем и, если оно
### присутствует, замените его на 200 Обновите список только при первом вхождении числа
### 20

```

list1=[10,20,30,40,50,200,240,250,220]
index = list1.index(20)
list1[index]=200
print(list1)

```

### Задача 2 Поменять местами самый большой и самый маленький элементы списка

```

print(list1)

a= min(list1)
b= max(list1)

c = list1.index(a)
d = list1.index(b)

list1[c],list1[d] = list1[d],list1[c]

print(list1)

```
### Задача 3 Найти ошибку в программе и исправить

### list1 = [1, 2, 3]
### list2 = [4, 5, 6]
### list1.append(list2)
### print(list1)
### Результат программы должен быть таким [1, 2, 3, 4, 5, 6]
### Категория задач – средней сложности:

```
list1 = [1, 2, 3]
list2 = [4, 5, 6]
list1 = list1 + list2
print(list1)

```

### Задача 4 Написать программу: дан список из 10 чисел, которые задаются с помощью
### датчика случайных чисел в диапазоне 1-10. Программа находит повторяющиеся
### элементы и удаляет их из списка. Например, дан список (1,1,1,2,3,4,2,3,4) результат
### (1,2,3,4)

```
import random
list=[random.randint(1, 10) for _ in range(10)]
list1=[]
for i in list:
    if list1.count(i)==0:
        list1.append(i)

print(list1)

```

### Задача 5 Написать программу: дан список из 10 чисел, которые задаются с помощью
### датчика случайных чисел. Программа находит повторяющиеся элементы и считает
### количество повторений. Например дан список (1,1,1,2,3,4,2,3,4) результат число 1
### повторяется 3 раза, число 2 – 2раза, число 3 - 2 раза, число 4 – 2 раза

```
import random
list=[random.randint(1, 10) for _ in range(10)]
list1=[]
for i in list:
    if list1.count(i)==0:
        list1.append(i)

print(list1)

for i in list1:
    print("число", i, "повторяется", list.count(i), "раз")

```

### Задача 6 Сжатие списка - дан список целых чисел. Требуется “сжать” его, переместив все
### ненулевые элементы в левую часть списка, не меняя их порядок, а все нули - в правую
### часть. Порядок ненулевых элементов изменять нельзя, дополнительный список
### использовать нельзя, задачу нужно выполнить за один проход по списку. Распечатайте
### полученный список.
### Входные данные
### Вводится список чисел. Все числа списка находятся на одной строке.
### Выходные данные
### Выведите ответ на задачу.
### Примеры
### входные данные
### 4 0 5 0 3 0 0 5
### выходные данные
### 4 5 3 5 0 0 0 0

```
list=[4,0,5,0,3,0,0,5]

for i in list:
    if i == 0:
        list.remove(i)
        list.append(0)

print(list)

```

### Задача 7 Дан список в виде списка списков, например [[1,2,3],[2,6,4],[3,4,5],[6,3,7]].
### Вывести список из элементов списка – без повторения, результат– [1,2,3,6,4,5,7]. Вывести
### писков из элементов списка, которые повторяются в исходном списке, результат –
###  [2,3,4,6]

```
a=[[1,2,3],[2,6,4],[3,4,5],[6,3,7]]
c=[]
for i in a:
    c.extend(i)
d=[]
for j in c:
    if c.count(j)>1:
        d.append(j)
d=set(d)
print(d)
c=set(c)
print(c)

```
