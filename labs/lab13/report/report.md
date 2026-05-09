---
## Front matter
title: Лабораторная работа
subtitle: Номер 13
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

Целью данной работы является проведение подготовительных мероприятий по организации взаимодействия через сеть провайдера посредством статической маршрутизации локальной
сети с сетью основного здания, расположенного в 42-м квартале в Москве,
и сетью филиала, расположенного в г. Сочи.

# Выполнение лабораторной работы

На схеме предыдущего проекта размещаем необходимое оборудование (Рис. 1.1).

![Размещение необходимого оборудования на схеме](image/2.png){height=60%}

Присваиваем названия размещённым объектам (Рис. 1.2).

![Присваивание названий размещенным объектам](image/3.png){height=60%}

На медиаконвертерах заменяем имеющиеся модули на модули для подключения витой пары по
технологии Fast Ethernet и оптоволокна соответственно (Рис. 1.3).

![Замена модулей на медиаконвертерах](image/4.png){height=60%}

На маршрутизаторе msk-q42-gw-1 добавляем дополнительный интерфейс NM-2FE2W (Рис. 1.4)

![Дополнительный интерфейс на маршрутизаторе msk-q42-gw-1](image/5.png){height=60%}

В физической рабочей области Packet Tracer добавляем в г. Москва здание 42-го квартала, присваиваем ему соответствующее название (Рис. 1.5).

![Здание 42-го квартала в физической рабочей области](image/6.png){height=60%}

В физической рабочей области Packet Tracer добавляем город Сочи и в нём здание филиала, присваиваем ему соответствующее название (Рис. 1.6).

![Город Сочи и филиал в физической рабочей области](image/7.png){height=60%}

Переносим из сети «Донская» оборудование сети 42-го квартала и сети филиала в соответствующие здания (Рис. 1.7).

![Оборудование сети 42-го квартала и сети филиала](image/8.png){height=60%}

Проводим соединение объектов согласно скорректированной схеме L1 (Рис. 1.8).

![Соединение объектов согласно схеме](image/9.png){height=60%}

Выполняем первоначальную настройку маршрутизатора msk-q42-gw-1 (Рис. 1.9).

![Первоначальная настройка маршрутизатора msk-q42-gw-1](image/2.1.png){height=60%}

Выполняем первоначальную настройку коммутатора msk-q42-sw-1 (Рис. 1.10).

![Первоначальная настройка коммутатора msk-q42-sw-1](image/2.2.png){height=60%}

Выполняем первоначальную настройку маршрутизирующего коммутатора msk-hostel-gw-1 (Рис. 1.11).

![Первоначальная настройка маршрутизирующего коммутатора msk-hostel-gw-1](image/2.3.png){height=60%}

Выполняем первоначальную настройку коммутатора msk-hostel-sw-1 (Рис. 1.12)

![Первоначальная настройка коммутатора msk-hostel-sw-1](image/2.4.png){height=60%}

Выполняем первоначальную настройку коммутатора sch-sochi-sw-1 (Рис. 1.13).

![Первоначальная настройка коммутатора sch-sochi-sw-1](image/3.1.png){height=60%}

Выполняем первоначальную настройку маршрутизатора sch-sochi-sw-1 (Рис. 1.14).

![Первоначальная настройка маршрутизатора sch-sochi-gw-1](image/3.2.png){height=60%}

# Выводы

В результате выполнения лабораторной работы мною были проведены подготовительные мероприятия по организации взаимодействия через сеть провайдера посредством статической маршрутизации локальной сети с сетью основного здания, расположенного в 42-м квартале в Москве, и сетью филиала, расположенного в г. Сочи.

# Список литературы{.unnumbered}
