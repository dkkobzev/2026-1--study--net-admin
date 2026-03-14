---
## Front matter
title: Лабораторная работа
subtitle: Номер 5
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

Целью данной работы является получение основных навыков по настройке VLAN на коммутаторах сети.

# Выполнение лабораторной работы

Используя приведённую последовательность команд из примера по конфигурации Trunk-порта, настраиваем Trunk-порты на соответствующих интерфейсах всех коммутаторов (Рис. 1.1), (Рис. 1.2), (Рис. 1.3), (Рис. 1.4), (Рис. 1.5)

![Настройка Trunk-портов на коммутаторе msk-donskaya-dkkobzev-sw-1](image/1.png){height=60%}

![Настройка Trunk-портов на коммутаторе msk-donskaya-dkkobzev-sw-2](image/2.png){height=60%}

![Настройка Trunk-портов на коммутаторе msk-donskaya-dkkobzev-sw-3](image/3.png){height=60%}

![Настройка Trunk-портов на коммутаторе msk-donskaya-dkkobzev-sw-4](image/4.png){height=60%}

![Настройка Trunk-портов на коммутаторе msk-pavlovskaya-dkkobzev-sw-1](image/5.png){height=60%}

Используя приведённую последовательность команд по конфигурации VTP, настраиваем коммутатор msk-donskaya-sw-1 как VTP-сервер и прописываем на нём номера и названия VLAN (Рис. 1.6).

![Настройка коммутатора msk-donskaya-sw-1 как VTP-сервер](image/6.png){height=60%}

Используя приведённую последовательность команд по конфигурации диапазонов портов, настраиваем коммутаторы msk-donskaya-sw-2 — msk-donskaya-sw-4, msk-pavlovskaya-sw-1 как VTP-клиенты и на интерфейсах указываем принадлежность к VLAN (Рис. 1.7), (Рис. 1.8), (Рис. 1.9), (Рис. 1.10).

![Настройка коммутатора msk-donskaya-sw-2 как VTP-клиент](image/7.png){height=60%}

![Настройка коммутатора msk-donskaya-sw-3 как VTP-клиент](image/8.png){height=60%}

![Настройка коммутатора msk-donskaya-sw-4 как VTP-клиент](image/9.png){height=60%}

![Настройка коммутатора msk-pavlovskaya-sw-1 как VTP-клиент](image/10.png){height=60%}

После указания статических IP-адресов на оконечных устройствах проверяем с помощью команды ping доступность устройств, принадлежащих одному VLAN, и недоступность устройств, принадлежащих разным VLAN (Рис. 1.11).

![Проверка доступности устройств](image/11.png){height=60%}

# Выводы

В результате выполнения лабораторной работы мною были получены основные навыки по настройке VLAN на коммутаторах сети.

# Список литературы{.unnumbered}
