---
## Front matter
lang: ru-RU
title: Отчет по лабораторной работе №14
author: Перелыгин Сергей Викторович

## Formatting
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
toc: false
slide_level: 2
theme: metropolis
aspectratio: 43
section-titles: true
---

# Цель работы

## Цель лабораторной работы

Приобрести простейшие навыки разработки, анализа, тестирования и отладки приложений в ОС типа UNIX/Linux на примере создания на языке  программирования С калькулятора с простейшими функциями.

# Выполнение лабораторной работы

## Выполнение лабораторной работы

В ходе выполнения ЛР я создал примитивный калькулятор, способный складывать, вычитать, умножать и делить, возводить число в степень, брать квадратный корень, вычислять sin, cos, tan. Для этого понадобилось заранее создать три файла (calculate.h, calculate.c, main.c)

![Создание 3 файлов для калькулятора](images/2.png){ #fig:001 width=70% }

## Выполнение лабораторной работы

Затем я скомпиллировал программу с помощью gcc. После этого я создал Makefile и при помощи отладчика GDB выполнил отладку программы.

![Makefile](images/8.png){ #fig:002 width=70% }

---

![Запуск программы](images/12.png){ #fig:003 width=70% }

## Выполнение лабораторной работы

Также я научился устанавливать точки останова и удалять их.

![Точка останова](images/16.png){ #fig:004 width=70% }

---

![Удаление точки останова](images/21.png){ #fig:005 width=70% }

## Выполнение лабораторной работы

С помощью утилиты splint проанализировал коды файлов calculate.c и main.c., предварительно установив данную утилиту с помощью команд «sudo apt update» и «sudo apt install splint».

![splint calculate.c](images/22.png){ #fig:022 width=50% }

---

![splint main.c](images/23.png){ #fig:023 width=70% }


# Выводы

## Выводы

В ходе выполнения данной лабораторной работы я приобрел простейшие навыки разработки, анализа, тестирования и отладки приложений в ОС типа UNIX/Linux на примере создания на языке программирования С калькулятора с простейшими функциями.

---
Спасибо за внимание!