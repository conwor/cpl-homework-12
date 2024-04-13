# Домашнее задание №12 - Поиск подмассива в массиве (1 балл)

Прочитать с клавиатуры два числа `N` и `M` типа `size_t`. Затем прочитать `N` чисел и сохранить их
в VLA-массив `A1` длины `N` в автоматической памяти. Затем прочитать `M` чисел и сохранить их в 
VLA-массив `A2` длины `M` в автоматической памяти.

Вывести индекс первого вхождения массива `A2` в массив `A1`, либо `-1`, если такого вхождения нет.

Поиск подмассива в массиве должен быть выделен в функцию, возвращающую не индекс, а адрес нулевого
элемента, с которого начинается вхождение, либо константу `NULL`, если вхождения нет.
Преобразование адреса в индекс должно осуществляться адресной арифметикой (вычитанием из адреса
элемента адреса начала массива).

Программа должна работать корректно с массивами длины 0. Массив длины 0 является подмассивом
любого массива (в том числе длины 0), входящим в него по индексу 0. Другие подмассивы в массив
длины 0 входить не могут. Учтите, что создание VLA-массивов длины 0 запрещено санитайзерами,
используемыми при проверке решений.

Если какое-либо из чисел `N` и `M` больше 1000, нужно вывести сообщение об ошибке `Incorrect input`
и прервать выполнение программы.

## Пример

### Входные данные

```
10 3
1 2 1 2 1 2 3 1 2 3
1 2 3
```

### Выходные данные

```
4

```
