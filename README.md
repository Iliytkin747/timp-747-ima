# TiMP

# Практическая работа №1

Задание 1
Написать программу, печатающую в stdout фразу “Hello, World!” на отдельной строке.

Задание 2
Написать программу, принимающую на вход два числа, разделённые пробелом, и суммирующую их. Ввод чисел производить из stdin, вывод результата - в stdout.

Задание 3
Написать программу, принимающую на вход числа x и y, разделённые пробелом, и вычисляющую x в степени y.

# Практическая работа №2
## Варианты и задания
### Вариант 7. Количество отрицательных чисел. 
На вход подаётся
число 𝑛 ∈ N : 𝑛 ≤ 2147483647, а также 𝑛 чисел 𝑥𝑖 ∈ Z : |𝑥𝑖
| ≤ 2147483647
для любого целого 𝑖 от 1 до 𝑛. Вывести количество чисел 𝑥𝑖
: 𝑥𝑖 < 0.
### Вариант 17. Разность сумм чётных и нечётных квадратов. На
вход подаётся число 𝑛 ∈ N : 𝑛 ≤ 2147483647, а также 𝑛 чисел 𝑥𝑖 ∈
Z : |𝑥𝑖
| ≤ 2147483647 для любого целого 𝑖 от 1 до 𝑛. Вывести значение
∑︁𝑛
𝑖=1
(−1)𝑖
· 𝑥
2

## Ход работы
1. Был написан код для каждого из задания.
2. Каждый файл с кодом был скомпилирован и запущен для проверки:

```
$ gcc 07_proga1.c -o 07_proga1
$ ./07_proga1
$ gcc 17_proga2.c -o 17_proga2 -lm
$ ./17_proga2
```
3. Файлы были загружены на удалённый репозиторий pr2
```
$ git add .
$ git commit
$ git push -u origin pr2
```
## Результаты работы
Скриншоты работы программ представленны ниже.

***Количество отрицательных чисел.***
На вход были введены 5 чисел (2 из нах отрецательные). В результате программа выдала число 2.

![gmt7oiiyk_e](https://user-images.githubusercontent.com/47884454/53642111-8e662b00-3c63-11e9-9a22-6f92b2825a26.jpg)

***Разность сумм чётных и нечётных квадратов.***
Были введены 4 числа (1, 2, 3, 4). Разность сумм чётных и не чётных квадратов равна 10.

![default](https://user-images.githubusercontent.com/47884454/53642200-c8cfc800-3c63-11e9-9907-8cffcd0bdac6.PNG)

# Практическая работа №3

## Односвязные списки
Необходимо используя  функции реализовать программу которая:
1. считать количество элементов ∈ N≤ 2147483647;
2.  создать пустой список, считать n элементов a, |a| ≤2147483647 и занести их в список;
3.  вывести содержимое списка используя функцию print;
4.  считать k1, k2, k3 |k| ≤ 2147483647 и вывести ‘1’ если в списке существует элемент с таким значением. ‘0’ если нет, перейти на новую строку.
5.  считать m, |m| ≤ 2147483647 и вставить его в конец списка;
6.  вывести содержимое списка используя функцию print;
7.  считать t, |t| ≤ 2147483647 и вставить его в начало списка;
8.  вывести содержимое списка используя функцию print;
9.  считать j, 0 < j ≤ 2147483647 и x, |x| ≤ 2147483647 и вставить значение x после j-ого элемента списка;
10. вывести содержимое списка используя функцию print;
11.  считать z, |z| ≤ 2147483647 и удалить первый элемент хранящий значение z из списка;
12. вывести содержимое списка используя функцию print;
13.  очистить список.


## Ход работы
С помощью текстового блокнота **nano** были созданы исходный код программы. Код был скомпилирован и проверен на заданных примерах.


|  input     | output           |
|:----------:|:----------------:|
|3           |                  |
|1 2 3       | 1 2 3            |
|4 2 3       | 0 1 1            |
|5           | 1 2 3 5          |
|6           | 6 1 2 3 5        |
|4 8         | 6 1 2 3 8 5      |
|6           | 1 2 4 8 5        |

В ходе работы были использованы следующие функции:


<a href="https://imgbb.com/"><img src="https://i.ibb.co/VSPTtCw/1.png" alt="1" border="0"></a>



<a href="https://imgbb.com/"><img src="https://i.ibb.co/7z94tvV/2.png" alt="2" border="0"></a>



Результат выполнения программы:


<a href="https://imgbb.com/"><img src="https://i.ibb.co/RSng0hz/1.png" alt="1" border="0"></a>

## Двусвязные списки
Необходимо используя  функции реализовать программу которая:
1. считать количество элементов  ∈ N, 0 < ≤ 2147483647;
2. создать пустой список, считать n элементов a , |a | ≤
2147483647 и занести их в список;
3. вывести содержимое списка используя функцию print;
4. считать k , k , k |k | ≤ 2147483647 и вывести ‘1’ если в
списке существует элемент с таким значением. ‘0’ если нет.
перейти на новую строку.
5. считать m, |m| ≤ 2147483647 и вставить его в конец списка;
6. вывести содержимое списка используя функцию print_invers;
7. считать t, |t| ≤ 2147483647 и вставить его в начало списка;
8. вывести содержимое списка используя функцию print;
9. считать j, 0 < j ≤ 2147483647 и x, |x| ≤ 2147483647 и вставить
значение x после j-ого элемента списка;
10. вывести содержимое списка используя функцию print_invers;
11. считать u, 0 < u ≤ 2147483647 и y, |y| ≤ 2147483647 и
вставить значение y перед u-ым элементом списка;
12. вывести содержимое списка используя функцию print;
13. считать z, |z| ≤ 2147483647 и удалить первый элемент
хранящий значение z из списка;
14. вывести содержимое списка используя функцию print_invers;
15. считать r, |r| ≤ 2147483647 и удалить последний элемент
хранящий значение r из списка;
16. вывести содержимое списка используя функцию print;
17. очистить список.


## Ход работы
С помощью текстового блокнота **nano** были созданы исходный код программы. Код был скомпилирован и проверен на заданных примерах.


|  input     | output           |
|:----------:|:----------------:|
|3           |                  |
|1 2 3       | 1 2 3            |
|1 6 4       | 1 0 0            |
|7           | 7 3 2 1          |
|8           | 8 1 2 3 7        |
|3 9         | 7 3 9 2 1 8      |
|2 6         | 8 6 1 2 9 3 7    |
|9           | 7 3 2 1 6 8      |
|2           | 8 6 1 3 7        |

В ходе работы были использованы следующие функции:


<a href="https://imgbb.com/"><img src="https://i.ibb.co/VSPTtCw/1.png" alt="1" border="0"></a><br />

<a href="https://imgbb.com/"><img src="https://i.ibb.co/7z94tvV/2.png" alt="2" border="0"></a><br />

<a href="https://imgbb.com/"><img src="https://i.ibb.co/8rhHn7Y/3.png" alt="3" border="0"></a><br />



Результат выполнения программы:


<a href="https://imgbb.com/"><img src="https://i.ibb.co/WsL2kQn/2.png" alt="2" border="0"></a><br />

# Практическая работа №4 ***"Бинарное дерево поиска"***

## Задание

Используя функции, реализовать программу, которая:
1. создать пустое дерево, считать 4 элементов a, |a| ≤2147483647 и занести их в дерево;
2. вывести дерево, используя функцию printTree;
3. считать 3 элементов a, |a| ≤ 2147483647 и занести их в дерево;
4. вывести дерево, используя функцию printTree;
5. считать m1, |m1| ≤ 2147483647 и найти элемент с заданным значением в дереве. Вывести через пробел значение предка и потомков найденного элемента. Если элемент не найден, вывести "_", если нет значений предка или потомков, вывести’’ вместо таких значений;
6. считать m2, |m2| ≤ 2147483647 и найти элемент с заданным значением в дереве. Вывести через пробел значение предка и потомков найденного элемента. Если элемент не найден, вывести ‘-’, если нет значений предка или потомков, вывести‘_’ вместо таких значений;
7. считать m3, |m3| ≤ 2147483647 и удалить из дерева элемент с заданным значением;
8. вывести дерево, используя printTree;
9. выполнять левый поворот дерева относительно корня, пока это возможно;
10. вывести дерево, используя команду printTree;
11. выполнять правый поворот дерева относительно корня, пока это возможно;
12. вывести дерево, используя команду printTree;
13. вывести на экран количество элементов в дереве;
14. очистить дерево;
15. вывести дерево на экран, используя printTree.

## Ход работы

С помощью текстового блокнота **nano** были созданы исходный код программы. Код был скомпилирован и проверен на заданных примерах.


|  На вход   | На выход                       |
|:----------:|:-------------------------------|
| 4 7 3 2    |4                               |
|            |3 7                             |
|            |2 _ _ _                         |
| 5 9 1      |4                               |
|            |3 7                             |
|            |2 _ 5 9                         |
|            |1 _ _ _ _ _ _ _                 |
| 6          |_ _ _                           |
| 7          |4 5 9                           |
| 2          |4                               |
|            |3 7                             |
|            |1 _ 5 9                         |
|            |9                               |
|            |7 _                             |
|            |4 _ _ _                         |
|            |3 5 _ _ _ _ _ _                 |
|            |1 _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
|            |1                               |
|            |_ 3                             |
|            |_ _ _  4                        |
|            |_ _ _ _ _ _ _ 7                 |
|            |_ _ _ _ _ _ _ _ _ _ _ _ _ _ 5 9 |
|            |6                               |
|            |_                               | 

В ходе работы были использованы следующие функции:


![enter image description here](https://lh3.googleusercontent.com/3iNccdUfom4uucB5vjVzfFJnhOPs5c-Sz1bE-MoFhqCHulI4daoT-XYilcNzALqLBxxjX7UwiM36)

![enter image description here](https://lh3.googleusercontent.com/oXYssMbdxnDYJGVw0c8-lyKR1eGbIcAXqMK4T1i_1n2abJ8_WN-LXeEXGYc2Ix1vfer84II7FWFI)

![enter image description here](https://lh3.googleusercontent.com/HWeZ_e5hepQSYswcQwP4pfOXlx2wSipP_nSYPW1KsHwOlBqb2bJRsy_jfJRW6BftWA0dv4V4eLoP)









Результат выполнения программы:

![enter image description here](https://i.ibb.co/BwQ8fST/4.png)

# Практическая работа №5 ***"Обход дерева"***
## Задание №1
![alt_text](https://pp.userapi.com/c850536/v850536982/f0667/WVXF5E5XroQ.jpg)
## Задание №2
![alt_text](https://pp.userapi.com/c850536/v850536982/f066f/GV4k37N8Ow8.jpg)
## Задание №3
![alt_text](https://pp.userapi.com/c850536/v850536982/f0677/1iOEqtRUipU.jpg)
## Ход работы
1. С помощью редактора кода nano был написан код для каждого задания
2. Затем код был скомпилирован с помощью компилятора gcc
3. Была создана отдельная ветка pr5 
4. Затем файлы были добавлены  на репозиторий
```
$ git checkout -b pr5
$ git add .
$ git commit -m
$ git push -u origin pr5
```
## Результаты

## Задание №1
![enter image description here](https://i.ibb.co/bQh75dX/1-5.png)
## Задание №2
![enter image description here](https://i.ibb.co/BwPqLSD/2-5.png)
## Задание №3
![enter image description here](https://i.ibb.co/QY6hmP3/3-5.png)

# **Практика 6 "Алгоритмы сортировки 1"**

## **Задание 1**

- Считать количество элементов n.
- Считать n целочисленных элементов.
- Отсортировать полученный массив сортировкой *расческой*.
-  Вывести отсортированный массив на экран через пробел.

## **Задание 2**

- Считать количество элементов n.
-  Считать n целочисленных элементов.
-  Отсортировать полученный массив сортировкой *Шелла*.
- Вывести отсортированный массив на экран через пробел.

## **Ход работы**

Сперва данные задания были реализованны на языке программирования **C**. При помощи текстового блокнота **nano** был написан исходный код для реализации данных заданий. В данных программах были реализованы  методы сортировки данных. Позже после создания кода, данные файлы были отправлены на репозитор при помощи команд:
  - git add .  
  - git commit -m
  - git push -u origin pr6
  
  ##  Результат 
  
  При помощи компилятора gcc была проверена работоспособность програм, ниже будут продемонстрирован скрин с результатами программ.
  
  ![alt text](https://i.ibb.co/wCn7z0N/6.png)
  
### Первая программа 
 
| На вход        |  На выход     | 
| -------------- |:-------------:| 
| 7              |               |
| 2 4 7 19 -1 3 5|19 7 5 4 3 2 -1|   

### Вторая программа
 
| На вход     |  На выход   | 
| ----------- |:-----------:| 
| 6           |             |
|2 1 5 -5 7 10|-5 1 2 5 7 10|

# **Практика 7 "Алгоритмы сортировки 2"**

## **Задание 1**

- Считать количество элементов n.
- Считать n целочисленных элементов.
- Отсортировать полученный массив Быстрой сортировкой.
-  Вывести отсортированный массив на экран через пробел.

## **Задание 2**

- Считать количество элементов n.
-  Считать n целочисленных элементов.
-  Отсортировать полученный массив Пирамидальной сортировкой.
- Вывести отсортированный массив на экран через пробел.

## **Ход работы**

Сперва данные задания были реализованны на языке программирования **C**. При помощи текстового блокнота **nano** был написан исходный код для реализации данных заданий. В данных программах были реализованы  методы сортировки данных. Позже после создания кода, данные файлы были отправлены на репозитор при помощи команд:
  - git add .  
  - git commit -m
  - git push -u origin pr7
  
  ##  Результат 
  
  При помощи компилятора gcc была проверена работоспособность програм, ниже будут продемонстрирован скрин с результатами программ.
  
  ![alt text](https://i.ibb.co/HCj7FPM/777.png)
  
### Первая программа 
 
| На вход         |  На выход      | 
| ----------------|:--------------:| 
| 7               |                |
|1 4 0 5 -21 89 2 |-21 0 1 2 4 5 89|   

### Вторая программа
 
| На вход      |  На выход    | 
| -------------|:------------:| 
| 6            |              |
|2 31 22 -3 0 7|-3 0 2 7 22 31|
