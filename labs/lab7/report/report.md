---
## Front matter
title: Лабораторная работа
subtitle: Номер 7
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

Целью данной работы является получение навыков работы с физической рабочей областью Packet Tracer, с учетом физических параметров сети.

# Выполнение лабораторной работы

Открываем проект предыдущей лабораторной работы.
Переходим в физическую рабочую область Packet Tracer. Присваиваем название городу — Moscow (Рис. 1.1).

![Физическая рабочая область Packet Tracer](image/1.png){height=60%}

Щёлкнув на изображении города, видим изображение здания. Присваиваем ему название Donskaya. Добавляем здание для территории Pavlovskaya (Рис. 1.2).

![Изображение зданий в физической рабочей области Packet Tracer](image/2.png){height=60%}

Щёлкнув на изображении здания Donskaya, перемещаем изображение, обозначающее серверное помещение, в него (Рис. 1.3).

![Пример размещения в физической рабочей области Packet Tracer серверной с подключением оконечных устройств](image/3.png){height=60%}

Щёлкнув на изображении серверной, видим отображение серверных стоек (Рис. 1.4).

![Отображение серверных стоек в Packet Tracer](image/4.png){height=60%}

Перемещаем коммутатор msk-pavlovskaya-sw-1 и два оконечных устройства dk-pavlovskaya-1 и other-pavlovskaya-1 на территорию Pavlovskaya,
используя меню Move физической рабочей области Packet Tracer (Рис. 1.5).

![Территория Pavlovskaya](image/5.png){height=60%}

Вернувшись в логическую рабочую область Packet Tracer, пингуем с коммутатора msk-donskaya-sw-1 коммутатор msk-pavlovskaya-sw-1. Убеждаемся в работоспособности соединения (Рис. 1.6).

![Проверка работоспособности соединения](image/6.png){height=60%}

В меню Options , Preferences во вкладке Interface активируем разрешение на учёт физических характеристик среды передачи (Рис. 1.7).

![Активация разрешения на учет физических характеристик среды передачи](image/7.png){height=60%}

В физической рабочей области Packet Tracer размещаем две территории на расстоянии более 100 м друг от друга  (Рис. 1.8).

![Размещение двух территорий на расстоянии более 100м друг от друга](image/8.png){height=60%}

Вернувшись в логическую рабочую область Packet Tracer, пингуем с коммутатора msk-donskaya-sw-1 коммутатор msk-pavlovskaya-sw-1. Убеждаемся в неработоспособности соединения (Рис. 1.9).

![Проверка неработоспособности соединения](image/9.png){height=60%}

Удаляем соединение между msk-donskaya-sw-1 и msk-pavlovskaya-sw-1. Добавляем в логическую рабочую область два повторителя. Присваиваем им соответствующие названия msk-donskaya-mc-1 и msk-pavlovskaya-mc-1. Заменяем имеющиеся модули на PT-REPEATER-
NM-1FFE и PT-REPEATER-NM-1CFE для подключения оптоволокна и витой пары по технологии Fast Ethernet (Рис. 1.10).

![Добавление повторителей](image/10.png){height=60%}

Перемещаем msk-pavlovskaya-mc-1 на территорию Pavlovskaya (Рис. 1.11).

![Перемещение msk-pavlovskaya-mc-1 на территорию Pavlovskaya](image/11.png){height=60%}

Подключаем коммутатор msk-donskaya-sw-1 к msk-donskaya-mc-1 по витой паре, msk-donskaya-mc-1 и msk-pavlovskaya-mc-1 — по оптоволокну, msk-pavlovskaya-sw-1 к msk-pavlovskaya-mc-1 — по витой паре (Рис. 1.12).

![Подключение повторителей](image/12.png){height=60%}

Убеждаемся в работоспособности соединения между msk-donskaya-sw-1 и msk-pavlovskaya-sw-1 (Рис. 1.13).

![Проверка работоспособности соединеия](image/13.png){height=60%}

# Выводы

В результате выполнения лабораторной работы мною были получены навыки работы с физической рабочей областью Packet Tracer, с учетом физических параметров сети.

# Список литературы{.unnumbered}
