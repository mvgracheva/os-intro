---
## Front matter
title: "Отчёт по лабораторной работе №1"
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

Целью данной работы является приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.


# Выполнение лабораторной работы

 
 Перехожу в каталог /var/tmp и создаю каталог с моим именем 
 (рис. @fig:001).

![Каталог](image/1.png){#fig:001 width=70%}
  
 Задаю отображение информации о настройках VirtualBox на английском(рис. @fig:002).

![отображение информации о настройках](image/2.png){#fig:002 width=70%}

Установливаю папку для виртуальных машине в /var/tmp/имя_пользователя(рис. @fig:003).

![Установка папку](image/3.png){#fig:003 width=70%}
Поверяю, что папка виртуальных машин по умолчанию изменена: (рис. @fig:004).

![Проверка изменений](image/4.png){#fig:004 width=70%}


Следующая команда выдаст только каталог:(рис. @fig:005).

![Команда, которая выдает только каталог](image/5.png){#fig:005 width=70%}

Переношу установочный образ в папку /var/tmp/имя_пользователя/iso:(рис. @fig:006).(рис. @fig:007).

![Перенос установочного образа](image/6.png){#fig:006 width=70%}

![Перенос установочного образа 2](image/91.png){#fig:007 width=70%}


Настройка хост-клавиши

Проверяю текущую комбинацию для хост-клавиши:(рис. @fig:008).

![Проверка текущей комбинации](image/7.png){#fig:008 width=70%}

Установливаю нужную клавишу (в примере клавиша Menu):(рис. @fig:009).

![Установка нужной клавиши](image/8.png){#fig:009 width=70%}


Создание виртуальной машины

Для использования графического интерфейса запускаю менеджер виртуальных машин, введя в командной строке:(рис. @fig:010). (рис. @fig:011).

![Запуск менеджера виртуальных машин](image/9.png){#fig:010 width=70%}

![Запуск менеджера виртуальных машин 2](image/10.png){#fig:011 width=70%}

Создаю новую виртуальную машину в графическом интерфейсе или в командной строке. (рис. @fig:012), (рис. @fig:013).

![Создание новой виртуальной машины](image/11.png){#fig:012 width=70%}

![Создание новой виртуальной машины 2](image/12.png){#fig:013 width=70%}

Указываю имя виртуальной машины (ваш логин в дисплейном классе), тип операционной системы — Linux, Fedora.

Указываю размер основной памяти виртуальной машины — от 2048 МБ.(рис. @fig:014).(рис. @fig:015).

![размер основной памяти](image/14.png){#fig:001 width=70%}

![размер основной памяти 2](image/15.png){#fig:001 width=70%}

Задаю конфигурацию жёсткого диска — загрузочный, VDI (VirtualBox Disk Image), динамический виртуальный диск.

Задаю размер диска — 80 ГБ (или больше), его расположение — в данном случае /var/tmp/имя_пользователя/имя_машины/имя_машины.vdi.(рис. @fig:016).

![размер диска](image/15.png){#fig:016 width=70%}
Выбираю в VirtualBox Вашей виртуальной машины. Добавляю новый привод оптических дисков и выбираю образ.

Подключаю загрузку с DVD:(рис. @fig:017).

![загрузка с DVD](image/16.png){#fig:017 width=70%}

 Добавляю IDE-контроллер:(рис. @fig:018).

![IDE-контроллер](image/17.png){#fig:018 width=70%}

Устанавливаю созданный мной файл VDI в качестве первого виртуального жесткого диска новой виртуальной машины:(рис. @fig:019).

![файл VDI](image/18.png){#fig:019 width=70%}

Подключаю к виртуальной машине ISO-файл:(рис. @fig:020).

![ISO-файл](image/19.png){#fig:020 width=70%}

В качестве графического контроллера ставлю VMSVGA.(рис. @fig:021).

![VMSVGA](image/20.png){#fig:021 width=70%}

Включаю ускорение 3D. (рис. @fig:022).

![ускорение 3D](image/21.png){#fig:022 width=70%}

Включаю общий буфер обмена и перетаскивание объектов между хостом и гостевой ОС.(рис. @fig:023).

![общий буфер обмена](image/22.png){#fig:023 width=70%}

Включаю поддержку UEFI.(рис. @fig:024).

![UEFI](image/23.png){#fig:024 width=70%}


# Выводы

Я приобрела практические навыки установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

# Список литературы{.unnumbered}

::: {#refs}
:::
