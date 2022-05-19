---
## Front matter
title: "Отчет по лабораторной работе №11"
subtitle: "Операционные системы"
author: "Ничипорова Елена Дмитриевна"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Изучить основы программирования в оболочке ОС UNIX. Научится писать болеесложные командные файлы с использованиемлогических управляющих конструкцийи циклов


# Выполнение лабораторной работы



1. Используя команды getopts grep,написала командный файл,который анализирует командную строку с ключами:iinputfile—прочитатьданные из указанного файла;ooutputfile—вывести данные в указанный файл;pшаблон—указать шаблон для поиска;C—различать большие и малые буквы;n—выдавать номера строк.Для данной задачи создала фaйл prog1.sh(рис. [-@fig:001]) и написала следующие алгоритмы(рис. [-@fig:002])

![создание файла](image/1.png){ #fig:001 width=70% }

![скрипт №1](image/2.png){ #fig:002 width=70% }

- проверила работу написанного скрипта, используя различные опции, предварительно добавив права на выполнение(рис. [-@fig:003]) и создав два файла, которые необходимы для выполнения программы. Скрипт работает корректно(рис. [-@fig:004])

![предоставление прав доступа](image/3.png){ #fig:003 width=70% }

![проверка работы программы](image/4.png){ #fig:004 width=70% }

2. Написала на языке Си программу,которая вводит число и определяет,является ли оно больше нуля,меньше нуля или равно нулю.Затем программа завершается с помощью функции exit(n),передавая информацию в о коде завершения в оболочку.Командный файл должен вызывать эту программу и,проанализировав с помощью команды$?,выдать сообщение о том,какое число было введено.Для данной задачи я создала 2 файла(рис. [-@fig:005]) и написала соответствующие скрипты (рис. [-@fig:006])(рис. [-@fig:007])

![создание файлов](image/5.png){ #fig:005 width=70% }

![работа с файлом chislo.c](image/6.png){ #fig:006 width=70% }

![работа с файлом chislo.sh](image/7.png){ #fig:007 width=70% }

- Проверила работу написанных скриптов. Скрипты работаеют корректно(рис. [-@fig:008])

![Проверка скрипта №2](image/8.png){ #fig:008 width=70% }

3. Написала командный файл,создающий указанное число файлов,пронумерованных последовательно от 1 до 𝑁(например1.tmp,2.tmp,3.tmp,4.tmpит.д.).Число файлов,которые необходимо создать,передаётся в аргументы командной строки.Этот же командный файл должен уметь удалять все созданные им файлы (если они существуют).Для данной задачи я создала новый файл (рис. [-@fig:009]) и написала соответсвующий скрипт(рис. [-@fig:0010])

![создание файла](image/9.png){ #fig:009 width=70% }

![скрипт №3](image/10.png){ #fig:0010 width=70% }

- Прверила работу написанного скрипта, предварительно добавиви право на исполнение(рис. [-@fig:0011])

![Проверка скрипта №3](image/11.png){ #fig:0011 width=70% }

4. Написала командный файл,который с помощью команды tar запаковывает в архив все файлы в указанной директории.Модифицировала его так,чтобы запаковывалисьтолько те файлы,которые были изменены менее недели тому назад (использовать команду find). Для данной программы я создала новый файл (рис. [-@fig:0012]) и написала соответсвующий скрипт(рис. [-@fig:0013])

![создание файлов](image/12.png){ #fig:0012 width=70% }

![скрипт №4](image/13.png){ #fig:0013 width=70% }

- Проверила работу скрипта, предварительно добавив право на исполнение и созадала новый каталог с несколькими файлами (рис. [-@fig:0014]). Скрипт работает корректно (рис. [-@fig:0015])

![создание каталога и предоставление прав доступа](image/14.png){ #fig:0014 width=70% }

![проверка скрипта №4](image/15.png){ #fig:0015 width=70% }

# Выводы

- В ходе выполения данной лабораторной работы я изучила основы программирования в оболочке ОС UNIX. Научилась писать болеесложные командные файлы с использованиемлогических управляющих конструкцийи циклов

# Список литературы{.unnumbered}

::: {#refs}
:::
