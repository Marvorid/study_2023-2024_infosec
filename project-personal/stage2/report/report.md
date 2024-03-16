---
## Front matter
title: "Индивидуальный проект этап2"
subtitle: "Основы информационной безопасности"
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

Установите DVWA в гостевую систему к Kali Linux.

# Теоретическое введение

   
    Некоторые из уязвимостей веб приложений, который содержит DVWA:
Брутфорс: Брутфорс HTTP формы страницы входа - используется для тестирования инструментов по атаке на пароль методом грубой силы и показывает небезопасность слабых паролей.
Исполнение (внедрение) команд: Выполнение команд уровня операционной системы.
    Межсайтовая подделка запроса (CSRF): Позволяет «атакующему» изменить пароль администратора приложений.
    Внедрение (инклуд) файлов: Позволяет «атакующему» присоединить удалённые/локальные файлы в веб приложение.
    SQL внедрение: Позволяет «атакующему» внедрить SQL выражения в HTTP из поля ввода, DVWA включает слепое и основанное на ошибке SQL внедрение.
   Небезопасная выгрузка файлов: Позволяет «атакующему» выгрузить вредоносные файлы на веб сервер.
    Межсайтовый скриптинг (XSS): «Атакующий» может внедрить свои скрипты в веб приложение/базу данных. DVWA включает отражённую и хранимую XSS.
    Пасхальные яйца: раскрытие полных путей, обход аутентификации и некоторые другие.
DVWA имеет три уровня безопасности, они меняют уровень безопасности каждого веб приложения в DVWA:
    Невозможный — этот уровень должен быть безопасным от всех уязвимостей. Он используется для сравнения уязвимого исходного кода с безопасным исходным кодом.
    Высокий — это расширение среднего уровня сложности, со смесью более сложных или альтернативных плохих практик в попытке обезопасить код. Уязвимости не позволяют такой простор эксплуатации как на других уровнях.
    Средний — этот уровень безопасности предназначен главным образом для того, чтобы дать пользователю пример плохих практик безопасности, где разработчик попытался сделать приложение безопасным, но потерпел неудачу.
    Низкий — этот уровень безопасности совершенно уязвим и совсем не имеет защиты. Его предназначение быть примером среди уязвимых веб приложений, примером плохих практик программирования и служить платформой обучения базовым техникам эксплуатации.


# Выполнение лабораторной работы

Установим DVWA в гостевую систему к Kali Linux с помощью клонирования из гитхаба и проведем дальнейшую установку

![Процесс установки](image/1.jpg){#fig:001 width=90%}

![Процесс установки](image/2.jpg){#fig:002 width=90%}

![Процесс установки](image/3.jpg){#fig:003 width=90%}

![Процесс установки](image/4.jpg){#fig:004 width=90%}

![Процесс установки](image/5.jpg){#fig:005 width=90%}

![Процесс установки](image/6.jpg){#fig:006 width=90%}

![Процесс установки](image/7.jpg){#fig:007 width=90%}

![Процесс установки](image/8.jpg){#fig:008 width=90%}

![Процесс установки](image/9.jpg){#fig:009 width=90%}

![Процесс установки](image/10.jpg){#fig:010 width=90%}

# Выводы

В ходе выполнения данного этапы мы установили DVWA в гостевую систему к Kali Linux

# Список литературы{.unnumbered}

::: {#refs}
:::
