# Block2HW6
## task 30
```
Задача решена посредством вложенной в цикл for формулы, использующей изначальные аргументы, заданные пользователем, где условию n-1 удовлетворяет индекс i, который итерируется с нулевого индекса
```
## task 32
```
Задача решена посредством вложенного в цикл for условия проверки значения итерируемого индекса i параметрам, соответствующим диапазону, введенному пользователем (min - max)
```
## task 34
```
Декомпозиция проблемы:
1. Создан словарь гласных букв;
2. Создана функция, в которой:
  2.1. Входящая строка приводится к нижнему регистру и разделяется на массив слов;
  2.2. Вычисляется размер гласных букв входящих в отдельное слово с помощью:
      функции высшего порядка *filter* в которую вложена анонимная функция, в которой осуществяется проверка на наличие итерируемого значения элемента слова в словаре (1.)
  2.3. Размер присваивается множеству;
  2.4. Как только длина множества становится больше 1 - это означает, что у нас появилось слово, в котором количество гласных букв отлично от первоначального (или если нет гласных вообще), а значит ритма нет, программа возвращает ответ и прекращает работу, при иных других вариантах - ритм есть

```
## task 36
```
Декомпозиция проблемы:
1. Создана функция, в которой:
  2.1. Выводится на печать первая строка. Она распаковывается после создания с помощью генератора списка согласно *размеру входящего параметра столбцов* (по умолчанию), а к возвращаемому элементу (i) добавляется "1", чтобы нумерация столбцов начиналась с единицы (иначе, в дальнейшем, если мы будем использовать деление на "0" - выдаст ошибку ZeroDivisionError);
  2.2. С помощью цикла for, итерируясь со 2 строки до *размера входящего параметра строк* (по умолчанию) + "1" (чтобы соблюсти соответствие размерности строк с отражаемым на экране), выводим на печать распакованную строку, которую создаем с помощью:
    -генератора списка, который итерируется от 1 до *размера входящего параметра столбцов* (по умолчанию) + "1" (чтобы соблюсти соответствие размерности столбцов с отражаемым на экране), возвращаемым элементом которого является:
      -номер строки, если итератор столбца равен "1", иначе - результат работы функции с нашими переменными (значение столбца и значение строки), которую пользователь передаст в нашу основную функцию. 
```


кодировка UTF-8

расширение python - v2022.20.2