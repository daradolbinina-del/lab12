# Домашнее задание к работе 12
## Условие задачи
Напишите программу, которая вычисляет размер типа данных short int в байтах
## 1. Алгоритм и блок-схема
## Алгоритм
 1. Начало.
2. Инициализируем массив short_arr[2];
3. printf("размер типа данных short int в байтах: %ld\n", (char*)(&short_arr[1]) - (char*)(&short_arr[0]));
4. Возвращаем 0;
5. Конец.
   
### Блок-схема
<img width="401" height="520" alt="image" src="https://github.com/user-attachments/assets/11d130af-e380-4368-acf7-ceb571dfe629" />




## 2. Реализация программы

```
#define _CRT_SECURE_NO_DEPRECATE
#include <stdio.h>
#include <locale.h>

void main()
{
	setlocale(LC_ALL, "RUS");
	short int short_arr[2];
	printf("размер типа данных short int в байтах: %ld\n", (char*)(&short_arr[1]) - (char*)(&short_arr[0]));
	return 0;
}

```


## 3. Результаты работы программы
<img width="580" height="197" alt="image" src="https://github.com/user-attachments/assets/56f347f0-32b8-4cc8-ba8f-560e192d8564" />


