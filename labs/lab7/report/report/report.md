---
## Front matter
title: "Лабораторная работа 7"
subtitle: "Простейший вариант"
author: "Андрей Гэинэ"

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
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
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

Научиться строить модель "Модель M|M|1|inf" с помощью xcos

# Задание

Реализуйте модель «Модель M|M|1|inf» в xcos

# Теоретическое введение

Модель M|M|1|inf — это одна из базовых моделей теории массового обслуживания, которая описывает систему с одним обслуживающим прибором (сервером), где заявки поступают согласно пуассоновскому процессу, а время обслуживания имеет экспоненциальное распределение. 

# Выполнение лабораторной работы

Зафиксируем начальные данные: λ = 0.3, µ = 0.35, z0 = 6

Суперблок, моделирующий поступление заявок

![Суперблок, моделирующий поступление заявок](image/1.png)

Суперблок, моделирующий процесс обработки заявок

![Суперблок, моделирующий процесс обработки заявок](image/2.png)

Готовая модель M|M|1|inf

![Готовая модель M|M|1|inf](image/3.png)

Результат моделирования 1

![Результат моделирования 1](image/4.png)

Результат моделирования 2

![Результат моделирования 2](image/5.png)

# Выводы

В ходе выполнения лабораторной работы научились создать модель "Модель M|M|1|inf".

# Список литературы{.unnumbered}

::: {#refs}
:::