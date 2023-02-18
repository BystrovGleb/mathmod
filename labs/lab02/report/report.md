---
## Front matter
title: "Отчёт по лабораторной работе №2"
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

В данной лабораторной работе мне будет необходимо изучить один из примеров построения математических моделей для выбора правильной стратегии при решении задач поиска. Рассмотрю задачу преследования браконьеров береговой охраной.

# Задание

Вариант 68

На море в тумане катер береговой охраны преследует лодку браконьеров. Через определенный промежуток времени туман рассеивается, и лодка обнаруживается на расстоянии 19,5 км от катера. Затем лодка снова скрывается в тумане и уходит прямолинейно в неизвестном направлении. Известно, что скорость катера в 3,9 раза больше скорости браконьерской лодки.

1. Запишите уравнение, описывающее движение катера, с начальными условиями для двух случаев (в зависимости от расположения катера относительно лодки в начальный момент времени).

2. Постройте траекторию движения катера и лодки для двух случаев.

3. Найдите точку пересечения траектории катера и лодки [@key-1].

# Теоретическое введение

Приведем один из примеров построения математических моделей для 
выбора правильной стратегии при решении задач поиска.

Например, рассмотрим задачу преследования браконьеров береговой 
охраной. На море в тумане катер береговой охраны преследует лодку браконьеров. Через определенный промежуток времени туман рассеивается, и лодка обнаруживается на расстоянии k км от катера. Затем лодка снова скрывается в тумане и уходит прямолинейно в неизвестном направлении. Известно, что скорость 
катера в 2 раза больше скорости браконьерской лодки.

Необходимо определить по какой траектории необходимо двигаться катеру, чтоб нагнать лодку [@key-2].

**Постановка задачи** 

Постановка задачи сформулирована на скриншотах [@key-2] (рис. @fig:001-@fig:007).

![Постановка задачи](image/1.1.png){ #fig:001 width=70%}

![Постановка задачи](image/1.2.png){ #fig:002 width=70%}

![Постановка задачи](image/1.3.png){ #fig:003 width=70%}

![Постановка задачи](image/1.4.png){ #fig:004 width=70%}

![Постановка задачи](image/1.5.png){ #fig:005 width=70%}

![Постановка задачи](image/1.6.png){ #fig:006 width=70%}

![Постановка задачи](image/1.7.png){ #fig:007 width=70%}

**Задание** 

Задание сформулировано на скриншоте [@key-2] (рис. @fig:008).

![Задание](image/1.8.png){ #fig:008 width=70%}

# Выполнение лабораторной работы

1. Вывел уравнение логарифмической спирали используя заданные условия моего варианта (рис. @fig:009-@fig:011).

![Вывод уравнения](image/1.png){ #fig:009 width=70%}

![Вывод уравнения](image/2.png){ #fig:010 width=70%}

![Вывод уравнения](image/3.png){ #fig:011 width=70%}

2. Установил Julia на ноутбук (рис. @fig:012).

![Процесс установки](image/4.png){ #fig:012 width=70%}

3. Скачал необходимые библиотеки для работы (рис. @fig:013).

![Скачивание библиотеки](image/5.png){ #fig:013 width=70%}

4. Решение для первого случая на языке Julia (рис. @fig:014).

![Первый случай](image/6.png){ #fig:014 width=70%}

5. Решение для первого случая на языке Julia (рис. @fig:015).

![Первый случай](image/7.png){ #fig:015 width=70%}

6. Решение для первого случая на языке Julia (рис. @fig:016).

![Первый случай](image/8.png){ #fig:016 width=70%}

7. Решение для первого случая на языке Julia (рис. @fig:017).

![Первый случай](image/9.png){ #fig:017 width=70%}

8. График для первого случая (рис. @fig:018).

![График](image/10.png){ #fig:018 width=70%}

9. Решение для второго случая на языке Julia (рис. @fig:019).

![Второй случай](image/11.png){ #fig:019 width=70%}

10. Решение для второго случая на языке Julia (рис. @fig:020).

![Второй случай](image/12.png){ #fig:020 width=70%}

11. Решение для второго случая на языке Julia (рис. @fig:021).

![Второй случай](image/13.png){ #fig:021 width=70%}

12. Решение для второго случая на языке Julia (рис. @fig:022).

![Второй случай](image/14.png){ #fig:022 width=70%}

13. График для второго случая (рис. @fig:023).

![График](image/15.png){ #fig:023 width=70%}

14. Отправил файлы на сервер, используя команды в Windows PowerShell [@key-3]  (рис. @fig:029).

![Отправка файлов на сервер](image/16.png){ #fig:029 width=70%}

# Выводы

В данной лабораторной работе мне успешно удалось изучить один из примеров построения математических моделей для выбора правильной стратегии при решении задач поиска, а также рассмотреть задачу преследования браконьеров береговой охраной.

# Список литературы{.unnumbered}

::: {#refs}
:::
