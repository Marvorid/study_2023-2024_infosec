---
## Front matter
title: "Лабораторная работа №2"
subtitle: "Основы Информационной безопасности"
author: "Сабралиева Марворид"

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

Получение практических навыков работы в консоли с атрибутами фай-
лов, закрепление теоретических основ дискреционного разграничения до-
ступа в современных системах с открытым кодом на базе ОС Linux.

# Выполнение лабораторной работы

1. В установленной при выполнении предыдущей лабораторной работы
операционной системе создадим учётную запись пользователя guest (использую учётную запись администратора): useradd guest
2. Зададим пароль для пользователя guest (использую учётную запись администратора): passwd guest
3. Войдем в систему от имени пользователя guest.
4. Определим директорию, в которой мы находимся, командой pwd. Сравним её с приглашением командной строки. Определим, является ли она
нашей домашней директорией
5. Уточним имя нашего пользователя командой whoami.
6. Уточним имя нашего пользователя, его группу, а также группы, куда входит пользователь, командой id. Выведенные значения uid, gid и др. запомним. Сравним вывод id с выводом команды groups.
7. Сравним полученную информацию об имени пользователя с данными,
выводимыми в приглашении командной строки.(рис. @fig:001).

![Первичные действия в учетной записи guest](image/1.png){#fig:001 width=90%}

8. Просмотрим файл /etc/passwd командой cat /etc/passwd
Найдем в нём свою учётную запись. Определим uid пользователя. Определим gid пользователя. Сравним найденные значения с полученными в предыдущих пунктах. guest имеет те же идентификаторы (рис. @fig:002).

![команда cat](image/2.png){#fig:002 width=90%}

9. Определим существующие в системе директории командой ls -l /home/ (рис. @fig:003).
10. Проверим, какие расширенные атрибуты установлены на поддиректориях, находящихся в директории /home, командой: lsattr /home Нам не удалось увидеть расширенные атрибуты директорий других пользователей, только своей домашней директории.

![Расширенные атрибуты](image/3.png){#fig:003 width=90%}

11. Создали в домашней директории поддиректорию dir1 командой mkdir dir1
Определим командами ls -l и lsattr, какие права доступа и расширенные атрибуты были выставлены на директорию dir1.
12. Снимем с директории dir1 все атрибуты командой chmod 000 dir1 и проверим с её помощью правильность выполнения команды ls -l
13. создали в директории dir1 файл file1 командой echo "test" > /home/guest/dir1/file1. Так как ранее мы отозвали все атрибуты, то тем самым были лишины всех прав на взаимодействие с dir1

![Снятие атрибутов с директории](image/4.png){#fig:004 width=90%}

14. Заполним таблицу «Установленные права и разрешённые действия», выполняя действия от имени владельца директории (файлов), определив опытным путём, какие операции разрешены, а какие нет. Если операция разрешена, занесите в таблицу знак «+», если не разрешена, знак «-».

![Заполнение таблицы](image/5.png){#fig:005 width=90%}

1 - Создание файла
2 - Удаление файла
3 - Запись в файл
4 - Чтение файла
5 - Смена директории
6 - Просмотр файлов в директории
7 - Переименование файла
8 - Смена атрибутов файла

![Заполнение таблицы](image/6.png){#fig:006 width=90%}

![Заполнение таблицы](image/7.png){#fig:007 width=90%}

![Заполнение таблицы](image/8.png){#fig:008 width=90%}

![Заполнение таблицы](image/9.png){#fig:009 width=90%}

# Выводы

В ходе выполнения лабораторной работы были получены навыки работы с атрибутами файлов и сведения о разграничении доступа

# Список литературы{.unnumbered}

::: {#refs}
:::
