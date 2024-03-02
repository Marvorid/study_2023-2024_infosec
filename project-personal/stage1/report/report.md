---
## Front matter
title: "Индивидуальный проект часть 1"
subtitle: "Основы Информационной Безопасности"
author: "Сабралиева Марворид Нуралиевна"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

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
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
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

Научиться основным способам тестирования веб приложений

# Задание

Установить дистрибутив Kali Linux в виртуальную машину

# Выполнение лабораторной работы

1. Создадим виртуальную машину: тип ОС - Linux, версия - Debian(рис. @fig:001).

![Создание виртуальной машины](image/1.jpeg){#fig:001 width=90%}

2. Зададим нужные нам настройки и создадим жесткий диск (рис. @fig:002).

![Создание виртуальной машины](image/2.jpeg){#fig:002 width=90%}

3. Добавим в оптический привод ранее скачанный нами kali-linux и запустим машину(рис. @fig:003).

![Оптический привод](image/3.jpeg){#fig:003 width=90%}

4. Проведем первичную настройку машины: установим язык, регион и настроим другие параметры. После того как загрузка закончится подключим образ диска дополнительной ОС. Теперь можно полноценно пользоваться машиной(рис. @fig:004).

![Завершение установки](image/4.jpeg){#fig:004 width=90%}


# Выводы

Установили дистрибутив Kali Linux в виртуальную машину.

# Список литературы{.unnumbered}

::: {#refs}
:::
