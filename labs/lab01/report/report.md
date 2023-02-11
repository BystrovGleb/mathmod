---
## Front matter
title: "Отчёт по лабораторной работе №1"
subtitle: "дисциплина: Математическое моделирование"
author: "Быстров Глеб Андреевич"

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

В данной лабораторной работе мне будет необходимо вспомнить как работать с git и разметкой Markdown для формирования отчётов по
лабораторным работам модифицируя готовый шаблон.

# Задание

Создать и настроить рабочее пространство для лабораторных работ для данной дисциплины.

# Теоретическое введение

Git («гит») — это распределённая система управления версиями. Проект был создан Линусом Торвальдсом для управления разработкой ядра Linux, первая версия выпущена 7 апреля 2005 года. На сегодняшний день его поддерживает Джунио Хамано [@key-3].

Среди проектов, использующих Git — ядро Linux, Swift, Android, Drupal, Cairo, GNU Core Utilities, Mesa, Wine, Chromium, Compiz Fusion, FlightGear, jQuery, PHP, NASM, MediaWiki, DokuWiki, Qt, ряд дистрибутивов Linux.

Программа является свободной и выпущена под лицензией GNU GPL версии 2. По умолчанию используется TCP порт 9418.

Необходимо выполнить следующие команды, чтобы git узнал имя и
электронную почту. Если git уже установлен, можно переходить к разделу окончания строк [@key-1].

git config --global user.name "Your Name"

git config --global user.email "your_email@whatever.com"

Markdown («маркда́ун») — облегчённый язык разметки, созданный с целью обозначения форматирования в простом тексте, с максимальным сохранением его читаемости человеком, и пригодный для машинного преобразования в языки для продвинутых публикаций (HTML, Rich Text и других) [@key-4].

Чтобы создать заголовок, используйте знак (#), например:
#This is heading 1

##This is heading 2

###This is heading 3

####This is heading 4

Чтобы задать для текста полужирное начертание, заключите его в
двойные звездочки:
This text is ** bold **.

Чтобы задать для текста курсивное начертание, заключите его в
одинарные звездочки:
This text is * italic *.

Чтобы задать для текста полужирное и курсивное начертание, заключите его в тройные звездочки:
This is text is both *** bold and italic ***  [@key-2].

# Выполнение лабораторной работы

1. Выполнил вход в свой аккаунт на GitHub (рис. @fig:001).

![Страница сайта GitHub](image/1.png){ #fig:001 width=70%}

2. Создал каталоги со следующей структурой: ~/work/study/2022-2023/Математическое моделирование/mathmod/ (рис. @fig:002).

![Структура каталогов](image/2.png){ #fig:002 width=70%}

3. Создал репозиторий на основе шаблона (рис. @fig:003).

![Создание репозитория](image/3.png){ #fig:003 width=70%}

4. Запустил Windows PowerShell и установил менеджер пакетов с интерфейсом командной строки Chocolatey (рис. @fig:004).

![Процесс установки Chocolatey](image/4.png){ #fig:004 width=70%}

5. Установил make для компиляции программ (рис. @fig:005).

![Процесс установки make](image/5.png){ #fig:005 width=70%}

6. Установил систему управления версиями git (рис. @fig:006).

![Процесс установки git](image/6.png){ #fig:006 width=70%}

7. Создал SSH-ключ используя команду в Windows PowerShell (рис. @fig:007).

![Генерация ключа](image/7.png){ #fig:007 width=70%}

8. Добавил закрытый SSH-ключ используя команду в Windows PowerShell (рис. @fig:008).

![Добавление закрытого ключа](image/8.png){ #fig:008 width=70%}

9. Добавил SSH-ключ на сайте https://github.com/ (рис. @fig:009).

![Добавление ключа](image/9.png){ #fig:009 width=70%}

10. Создал рекурсивный клон репозитория используя команду в Windows PowerShell (рис. @fig:010).

![Клонирование репозитория](image/10.png){ #fig:010 width=70%}

11. Установил универсальную утилиту для работы с текстовыми форматами Pandoc (рис. @fig:011).

![Установка Pandoc](image/11.png){ #fig:011 width=70%}

12. Создал каталоги для отчетов и презентаций к лабораторным работам и поместил в них файлы из шаблона (рис. @fig:012).

![Структура каталогов](image/12.png){ #fig:012 width=70%}

13. Установил необходимые пакеты для Python (рис. @fig:013).

![Установка пакетов](image/13.png){ #fig:013 width=70%}

14. Ввел команду make для генерации отчета в двух форматах (рис. @fig:014).

![Отработка команды make](image/14.png){ #fig:014 width=70%}

15. Проверил отчет в формате .docx (рис. @fig:015).

![Отчет в .docx](image/15.png){ #fig:015 width=70%}

16. Установил TeX Live для генерации файлов в формат .pdf (рис. @fig:016).

![Процесс загрузки TeX Live](image/16.png){ #fig:016 width=70%}

17. Ввел команду make для генерации отчета в двух форматах и удостоверился, что отчет также успешно создаётся в формате .pdf (рис. @fig:017).

![Отчет в .pdf](image/17.png){ #fig:017 width=70%}

18. Удалил лишний файл package.json (рис. @fig:018).

![Каталог дисциплины](image/18.png){ #fig:018 width=70%}

19. Отправил файлы на сервер, используя команды в Windows PowerShell (рис. @fig:019).

![Отправка файлов на сервер](image/19.png){ #fig:019 width=70%}

20. Удостоверился, что данные в репозитории были обновлены (рис. @fig:020).

![Страница репозитория на сайте](image/20.png){ #fig:020 width=70%}

# Выводы

В данной лабораторной работе мне успешно удалось создать и настроить рабочее пространство для лабораторных работ.

# Список литературы{.unnumbered}

::: {#refs}
:::
