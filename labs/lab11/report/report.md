---
## Front matter
title: Лабораторная работа
subtitle: Номер 11
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

Целью данной работы является проведение подготовительных мероприятий по подключению локальной сети организации к Интернету.

# Выполнение лабораторной работы

На схеме предыдущего проекта размещаем необходимое оборудование для сети провайдера и сети модельного Интернета.
Присваиваем названия размещённым в сети провайдера и в сети модельного Интернета объектам согласно модельным предположениям и схеме L1 (Рис. 1.1).

![Схема сети с выходом в Интернет](image/3-4.png){height=60%}

В физической рабочей области добавляем здание провайдера и здание, имитирующее расположение серверов модельного Интернета. Присваиваем им соответствующие названия (Рис. 1.2).

![Схема сети в физической рабочей области Packet Tracer](image/5.png){height=60%}

Переносим из сети «Донская» оборудование провайдера и модельной сети Интернета в соответствующие здания (Рис. 1.3), (Рис. 1.4).

![Оборудование в здании сети провайдера](image/6.png){height=60%}

![Оборудование в здании сети модельного Интернета](image/6.1.png){height=60%}

На медиаконвертерах заменяем имеющиеся модули на PT-REPEATER-NM-1FFE и PT-REPEATER-NM-1CFE для подключения витой пары по технологии Fast Ethernet и оптоволокна соответственно (Рис. 1.5).

![Медиаконвертер с модулями PT-REPEATER-NM-1FFE и PT-REPEATER-NM-1CFE](image/7.png){height=60%}

Проводим соединение объектов согласно скорректированной схеме L1 (Рис. 1.6).

![Соединение объектов согласно схеме L1](image/8.png){height=60%}

Прописываем IP-адреса серверам согласно табл. (Рис. 1.7).

![Прописывание IP-адресов](image/9.png){height=60%}

Прописываем сведения о серверах на DNS-сервере сети «Донская» (Рис. 1.8).

![Сведения о серверах на DNS-сервере сети «Донская»](image/10.png){height=60%}

# Выводы

В результате выполнения лабораторной работы мною были проведены подготовительные мероприятия по подключению локальной сети организации к Интернету.

# Список литературы{.unnumbered}
