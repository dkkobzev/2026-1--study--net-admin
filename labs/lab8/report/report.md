---
## Front matter
title: Лабораторная работа
subtitle: Номер 8
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

Целью данной работы является приобретение практических навыков по настройке динамического распределения IP-адресов посредством протокола DHCP (Dynamic Host Configuration Protocol) в локальной сети.

# Выполнение лабораторной работы

В логическую рабочую область проекта добавляем сервер dns и подключаем его к коммутатору msk-donskaya-sw-3 через порт Fa0/2, не забыв активировать порт при помощи соответствующих команд на коммутаторе. В конфигурации сервера указываем в качестве адреса шлюза 10.128.0.1, а в качестве адреса самого сервера — 10.128.0.5 с соответствующей маской 255.255.255.0 (Рис. 1.1).

![Логическая схема локальной сети с добавленным DNS-сервером](image/1.png){height=60%}

Настраиваем сервис DNS: (рис. 8.2):
– в конфигурации сервера выбираем службу DNS, активируйте ее;
– в поле Type в качестве типа записи DNS выбираем записи типа A;
– в поле Name указываем доменное имя, по которому можно обратиться, например, к web-серверу — www.donskaya.rudn.ru, затем указываем его IP-адрес в соответствующем поле 10.128.0.2;
– нажав на кнопку Add , добавляем DNS-запись на сервер;
– аналогичным образом добавляем DNS-записи для серверов mail, file, dns согласно распределению адресов (Рис. 1.2).

![Окно настройки сервиса DNS](image/2.png){height=60%}

Настраиваем DHCP-сервис на маршрутизаторе, используя приведённые команды для каждой выделенной сети: указываем IP-адрес DNS-сервера; затем переходим к настройке DHCP; задаем название конфигурируемому диапазону адресов (пулу адресов), указываем адрес сети, а также адреса шлюза и DNS-сервера; задаем пулы адресов, исключаемых из динамического распределени (Рис. 1.3).

![Настройка DHCP](image/3.png){height=60%}

![Информация о пулах DHCP и информация об привязках выданных адресов](image/4.png){height=60%}

На оконечных устройствах заменяем в настройках статическое распределение адресов на динамическое (Рис. 1.5).

![Замена распределения адресов на оконечных устройствах](image/5.png){height=60%}

Проверяем, какие адреса выделяются оконечным устройствам, а также доступность устройств из разных подсетей (Рис. 1.6).

![Проверка адресов на оконечных устройствах и доступность устройств из разных подсетей](image/6.png){height=60%}

# Выводы

В результате выполнения лабораторной работы мною были приобретены практические навыки по настройке динамического распределения IP-адресов посредством протокола DHCP (Dynamic Host Configuration Protocol) в локальной сети.

# Список литературы{.unnumbered}
