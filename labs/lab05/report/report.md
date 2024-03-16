---
## Front matter
title: "Отчёт по лабораторной работе №5"
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

Выполнить лабораторную работу

# Выполнение лабораторной работы

Менеджер паролей pass

Установка
Fedora

pass

dnf install pass pass-otp
gopass

dnf install gopass

Настройка
Ключи GPG

Просмотр списка ключей:

gpg --list-secret-keys
Если ключа нет, нужно создать новый:

gpg --full-generate-key
Инициализация хранилища

Инициализируем хранилище:

pass init <gpg-id or email>
Синхронизация с git

Создадим структуру git:

pass git init
Также можно задать адрес репозитория на хостинге (репозиторий необходимо предварительно создать):

pass git remote add origin git@github.com:<git_username>/<git_repo>.git
Для синхронизации выполняется следующая команда:

pass git pull
pass git push
Прямые изменения

Следует заметить, что отслеживаются только изменения, сделанные через сам gopass (или pass).
Если изменения сделаны непосредственно на файловой системе, необходимо вручную закоммитить и выложить изменения:

cd ~/.password-store/
git add .
git commit -am 'edit manually'
git push
Проверить статус синхронизации модно командой

pass git status



Настройка интерфейса с броузером
Для взаимодействия с броузером используется интерфейс native messaging.
Поэтому кроме плагина к броузеру устанавливается программа, обеспечивающая интерфейс native messaging.
Плагин browserpass

Репозиторий: https://github.com/browserpass/browserpass-extension
Плагин для брoузера
Плагин для Firefox: https://addons.mozilla.org/en-US/firefox/addon/browserpass-ce/.
Плагин для Chrome/Chromium: https://chrome.google.com/webstore/detail/browserpass-ce/naepdomgkenhinolocfifgehidddafch.
Интерфейс для взаимодействия с броузером (native messaging)

Репозиторий: https://github.com/browserpass/browserpass-native
Gentoo:

emerge www-plugins/browserpass
Fedora

dnf copr enable maximbaz/browserpass
dnf install browserpass

Сохранение пароля
Добавить новый пароль

Выполните:

pass insert [OPTIONAL DIR]/[FILENAME]
OPTIONAL DIR: необязательное имя каталога, определяющее файловую структуру для вашего хранилища паролей;
FILENAME: имя файла, который будет использоваться для хранения пароля.
Отобразите пароль для указанного имени файла:

pass [OPTIONAL DIR]/[FILENAME]
Замените существующий пароль:

pass generate --in-place FILENAME

# Выводы

Я выполнила лабораторную работу

# Список литературы{.unnumbered}

::: {#refs}
:::
