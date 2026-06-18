---
## Front matter
title: Лабораторная работа
subtitle: Номер 16
author: "Кобзев Д. К."

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: /home/dkkobzev/pandoc/csl/gost-r-7-0-5-2008-numeric.csl

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
mainfont: Liberation Serif
romanfont: Liberation Serif
sansfont: Liberation Sans
monofont: Liberation Mono
# mathfont: Libertinus Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9

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

Целью данной работы является получение навыков настройки VPN-туннеля через незащищённое Интернет-соединение.

# Выполнение лабораторной работы

Размещаем в рабочей области проекта в соответствии с модельными предположениями оборудование для сети Университета г. Пиза. (Рис. 1.1).

![Схема сети с дополнительными площадками](image/1.png){height=60%}

В физической рабочей области проекта создаем город Пиза, здание Университета г. Пиза. Перемещаем туда соответствующее оборудование. (Рис. 1.2).

![Физическая рабочая область](image/2.png){height=60%}

Выполняем первоначальную настройку и настройку интерфейсов оборудования сети Университета г. Пиза (Рис. 1.3), (Рис. 1.4), (Рис. 1.5), (Рис. 1.6).

![Первоначальная настройка маршрутизатора pisa-unipi-gw-1](image/3.1.png){height=60%}

![Первоначальная настройка коммутатора pisa-unipi-sw-1](image/3.2.png){height=60%}

![Настройка интерфейсов маршрутизатора pisa-unipi-gw-1](image/3.3.png){height=60%}

![Настройка интерфейсов коммутатора pisa-unipi-sw-1](image/3.4.png){height=60%}

Настраиваем VPN на основе протокола GRE (Рис. 1.7), (Рис. 1.8).

![Настройка маршрутизатора msk-donskaya-gw-1](image/4.1.png){height=60%}

![Настройка маршрутизатора pisa-unipi-gw-1](image/4.2.png){height=60%}

# Выводы

В результате выполнения лабораторной работы мною были получены навыки настройки VPN-туннеля через незащищённое Интернет-соединение.

# Список литературы{.unnumbered}
