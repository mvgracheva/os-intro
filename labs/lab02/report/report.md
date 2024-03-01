---
## Front matter
title: "Лабортаорная работа"
subtitle: "Настройка git"
author: "Грачева Мария Валерьевна"

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


Изучить идеологию и применение средств контроля версий.
Освоить умения по работе с git.



# Выполнение лабораторной работы

!Некоторые пункты опущены, так как выполнялись в прошлом семестре (например, создание SSH-ключа). Данный отчёт будет прикреплен отдельным файлом,

Зададим имя и email владельца репозитория Настроим utf-8 в выводе сообщений git : (рис. @fig:001)

![Настройка имени и email владельца репозитория](image/2.png){#fig:001 width=70%}

Настроим верификацию и подписание коммитов git

Зададим имя начальной ветки (будем называть её master), параметр autocrlf, параметр safecrlf:(рис. @fig:002)

![имя начальной ветки, autocrlf, safecrlf](image/9.png){#fig:002 width=70%}


SSH-ключ был сделан в прошлом семестре (рис. @fig:003)

![SSH-ключ](image/7.png){#fig:003 width=70%}

Создаю ключи pgp

Генерируем ключ (рис. @fig:004), (рис. @fig:005)

![Генерация ключа](image/12.png){#fig:004 width=70%}

![Генерация ключа 2](image/13.png){#fig:005 width=70%}


Выводим список ключей и копируем отпечаток приватного ключа (рис. @fig:006)

![Вывод списка](image/14.png){#fig:006 width=70%}


Создание репозитория курса на основе шаблона (рис. @fig:007), (рис. @fig:008)

![Создание репозитория](image/15.png){#fig:007 width=70%}

![Создание репозитория 2](image/16.png){#fig:008 width=70%}
 
 
Итог  (рис. @fig:009)

![Итог](image/17.png){#fig:009 width=70%}

# Выводы

Изучила идеологию и применение средств контроля версий.
Освоила умения по работе с git

# Список литературы{.unnumbered}

::: {#refs}
:::
