---
## Front matter
title: "Отчёт к лабораторной работе №1"
subtitle: "Основы администрирования операционных систем"
author: "Борисенкова София Павловна"

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

Целью данной работы является приобретение практических навыков работы с пользовательями в Rocky Linux.

# Последовательность выполнения работы

Определяю текущего пользователя командой whoami.
Вывожу информацию о пользователе командой id
Переключаюсь на root и снова использую id

![Определение пользователя](image/1.png){#fig:001 width=70%}

Открываю файл sudoers через visudo. В файле присутствует необходимая строка со словом wheel.

![Sudoers](image/2.png){#fig:002 width=70%}

Создадим пользователя alice в группе wheel и зададим пароль.

![Пользователь Alice](image/3.png){#fig:003 width=70%}

Аналогично из alice создадим пользователя bob

![Пользователь bob](image/4.png){#fig:004 width=70%}

Проверим параметры в файле login. 

![Параметры](image/5.png){#fig:005 width=70%}

Создадим каталоги Pictures и Documents.

![Каталоги](image/6.png){#fig:006 width=70%}

Создадим пользователя carol и проверим его.

![Пользователь carol](image/7.png){#fig:007 width=70%}

Создадим группы main и third и добавим туда пользователей

![Работа с группами](image/8.png){#fig:008 width=70%}

## Вывод

В ходе работы были получены навыки обращения с пользователями и группами в Rocky Linux

