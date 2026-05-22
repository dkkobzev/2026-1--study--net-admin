---
## Front matter
title: Лабораторная работа
subtitle: Номер 15
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

Целью данной работы является настройка динамической маршрутизации между территориями организации.

# Выполнение лабораторной работы

Настраиваем маршрутизатор msk-donskaya-gw-1 (Рис. 1.1).

![Настройка маршрутизатора msk-donskaya-gw-1](image/1.png){height=60%}

Проверяем состояние протокола OSPF на маршрутизаторе msk-donskaya-gw-1 (Рис. 1.2).

![Проверка состояния протокола OSPF на маршрутизаторе msk-donskaya-gw-1](image/2.png){height=60%}

Настраиваем маршрутизатор msk-q42-gw-1 (Рис. 1.3).

![Настройка маршрутизатора msk-q42-gw-1](image/3.png){height=60%}

Настраиваем маршрутизирующий коммутатор msk-hostel-gw-1 (Рис. 1.4)

![Настройка маршрутизирующего коммутатора msk-hostel-gw-1](image/4.png){height=60%}

Настраиваем маршрутизатор sch-sochi-gw-1 (Рис. 1.5).

![Настройка маршрутизатора sch-sochi-gw-1](image/5.png){height=60%}

Настраиваем интерфейсы коммутатора provider-sw-1 (Рис. 1.6).

![Настройка интерфейсов коммутатора provider-sw-1](image/2.1.png){height=60%}

Настраиваем маршрутизатор msk-q42-gw-1 (Рис. 1.7).

![Настройка маршрутизатора msk-q42-gw-1](image/2.2.png){height=60%}

Настраиваем коммутатор sch-sochi-sw-1 (Рис. 1.8).

![Настройка коммутатора sch-sochi-sw-1](image/2.3.png){height=60%}

Настраиваем маршрутизатор sch-sochi-gw-1 (Рис. 1.9).

![Настройка маршрутизатора sch-sochi-gw-1](image/2.4.png){height=60%}

# Выводы

В результате выполнения лабораторной работы мною была настроена динамическая маршрутизация между территориями организации.

# Список литературы{.unnumbered}
