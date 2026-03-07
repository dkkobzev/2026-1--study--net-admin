---
## Front matter
title: Лабораторная работа
subtitle: Номер 4
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

Целью данной работы является проведение подготовительной работы по первоначальной настройке коммутаторов сети.

# Выполнение лабораторной работы

В логической рабочей области Packet Tracer размещаем коммутаторы и оконечные устройства согласно схеме сети L1 и соединяем их через соответствующие интерфейсы (Рис. 1.1).

![Размещение коммутаторов и оконечных устройств согласно схеме сети L1](image/1.png){height=60%}

Используя типовую конфигурацию коммутатора, настраиваем все коммутаторы, изменяя название устройства и его IP-адрес согласно плану IP (Рис. 1.2), (Рис. 1.3), (Рис. 1.4), (Рис. 1.5), (Рис. 1.6).

![Первоначальная настройка коммутатора msk-donskaya-dkkobzev-sw-1](image/2.png){height=60%}

![Первоначальная настройка коммутатора msk-donskaya-dkkobzev-sw-2](image/3.png){height=60%}

![Первоначальная настройка коммутатора msk-donskaya-dkkobzev-sw-3](image/4.png){height=60%}

![Первоначальная настройка коммутатора msk-donskaya-dkkobzev-sw-4](image/5.png){height=60%}

![Первоначальная настройка коммутатора msk-donskaya-dkkobzev-sw-1](image/6.png){height=60%}

# Выводы

В результате выполнения лабораторной работы мною была проведена подготовительная работа по первоначальной настройке коммутаторов сети.

# Список литературы{.unnumbered}
