---
## Front matter
title: Лабораторная работа
subtitle: Номер 10
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

Целью данной работы является освоение настройки прав доступа пользователей к ресурсам сети.

# Выполнение лабораторной работы

В рабочей области проекта подключаем ноутбук администратора с именем admin к сети к other-donskaya-1 с тем, чтобы разрешить ему потом любые действия, связанные с управлением сетью. Для этого подсоединяем ноутбук к порту 24 коммутатора msk-donskaya-sw-4 и присваиваем ему статический адрес 10.128.6.200, указав в качестве gateway-адреса 10.128.6.1 и адреса DNS-сервера 10.128.0.5  (Рис. 1.1).

![Размещение ноутбука администратора в сети other-donskaya-1](image/0.png){height=60%}

Настраиваем доступ к web-серверу по порту tcp 80.
Добавляем список управления доступом к интерфейсу.
Настраиваем дополнительный доступ для администратора по протоколам Telnet и FTP (Рис. 1.2).

![Настройка доступов](image/1-3.png){height=60%}

Убеждаемся, что с узла с ip-адресом 10.128.6.200 есть доступ по протоколу FTP (Рис. 1.3)

![Проверка доступа к web-серверу по протоколу FTP с устройства администратора](image/3.png){height=60%}

Настраиваем доступ к файловому серверу.
Настраиваем доступ к почтовому серверу.
Настраиваем доступ к DNS-серверу.
Разрешаем icmp-запросы (Рис. 1.4).

![Настройка доступов к серверам](image/4-7.png){height=60%}

Проверяем доступность web-сервера (Рис. 1.5).

![Проверка доступности web-сервера](image/6.png){height=60%}

Настраиваем доступ для сети Other.
Настраиваем доступ администратора к сети сетевого оборудования (Рис. 1.6).

![Настройка доступов](image/8-9.png){height=60%}

Проверяем корректность установленных правил доступа, попытавшись получить доступ по различным протоколам с разных устройств сети к подсети серверов и подсети сетевого оборудования (Рис. 1.7).

![Проверка корректности установленных правил доступа](image/s1.png){height=60%}

Разрешаем администратору из сети Other на Павловской действия, аналогичные действиям администратора сети Other на Донской. (Рис. 1.8).

![Разрешения для администратора из сети Other на на Павловской](image/s2.png){height=60%}

# Выводы

В результате выполнения лабораторной работы мною была освоена настройка прав доступа пользователей к ресурсам сети.

# Список литературы{.unnumbered}
