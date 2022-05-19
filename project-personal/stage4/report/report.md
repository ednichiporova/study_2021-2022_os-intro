---
## Front matter
title: "Отчет по 4 этапу персонального проекта"
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

Добавить к созданному ранее сайту ссылки на научные и библиографические ресурсы, написать 2 поста: по прошлой неделе и на одну тему по выбору


# Выполнение лабораторной работы

- В папке blog запускаем hugo командой "~/bin/hugo server"

- Переходим в каталог ~/work/blog/content/autors/admin(рис. [-@fig:001])

![Содержимое каталога](image/1.png){ #fig:001 width=70% }

- Добавляем туда ссылки на научные и библеометрические ресурсы (рис. [-@fig:002])

![Изменение информации в файле маркдаун](image/2.png){ #fig:002 width=70% }

- Вот так это выглядит на моем сайте (рис. [-@fig:003])

![Ссылки на сайте](image/3.png){ #fig:003 width=70% }

- Выходим из каталога home и заходим в каталог blog, чтобы сделать два поста

- Добавляем два новых поста: о прошлой неделе(рис. [-@fig:004]) и о лекговесных языках разметки(рис. [-@fig:005])

![Пост о пролой неделе ](image/4.png){ #fig:004 width=70% }

![Пост о оформлении отчета ](image/5.png){ #fig:005 width=70% }

- После завершения всех измененийв папке blog запускаем ~/bin/hugo (рис. [-@fig:006])

![запуск hugo](image/6.png){ #fig:006 width=70% }

- Далее сохраняем все изменения как в папке blog(рис. [-@fig:007]), так и в папке public(рис. [-@fig:008])

![Сохранение изменений в blog](image/7.png){ #fig:007 width=70% }

![Сохранение изменений в public](image/8.png){ #fig:008 width=70% }



# Выводы

После выполнения данного этапа персонального проекта я научилась добавлять информацию о себе на сайт, а также написала два поста

# Список литературы{.unnumbered}

::: {#refs}
:::
