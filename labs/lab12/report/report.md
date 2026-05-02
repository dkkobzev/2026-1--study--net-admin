---
## Front matter
title: Лабораторная работа
subtitle: Номер 12
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

Целью данной работы является приобретение практических навыков по настройке доступа локальной сети к внешней сети посредством NAT.

# Выполнение лабораторной работы

Выполняем первоначальную настройку маршрутизатора provider-gw-1 (Рис. 1.1).

![Первоначальная настройка маршрутизатора provider-gw-1](image/1.png){height=60%}

Выполняем первоначальную настройку коммутатора provider-sw-1 (Рис. 1.2).

![Первоначальная настройка коммутатора provider-sw-1](image/2.png){height=60%}

Настраиваем интерфейсы маршрутизатора provider-gw-1 (Рис. 1.3).

![Настройка интерфейсов маршрутизатора provider-gw-1](image/3.png){height=60%}

Настраиваем интерфейсы коммутатора provider-sw-1 (Рис. 1.4)

![Настройка интерфейсов коммутатора provider-sw-1](image/4.png){height=60%}

Настраиваем интерфейсы маршрутизатора msk-donskaya-gw-1 (Рис. 1.5).

![Настройка интерфейсов маршрутизатора msk-donskaya-gw-1](image/5.png){height=60%}

Настраиваем пул адресов и список доступа для NAT (Рис. 1.6).

![Настройка пула адресов и списка доступа для NAT](image/6-7.png){height=60%}

Настраиваем  Port Address Translation и интерфейсы для NAT (Рис. 1.8).

![Настройка NAT](image/8.png){height=60%}

Настраиваем доступ из Интернета для веб, файлового и почтового серверов и доступ по RDP (Рис. 1.9).

![Настройка доступа из Интернета](image/9.png){height=60%}

# Выводы

В результате выполнения лабораторной работы мною были приобретены практические навыки по настройке доступа локальной сети к внешней сети посредством NAT.

# Список литературы{.unnumbered}
