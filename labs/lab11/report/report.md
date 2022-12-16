---
## Front matter
title: "Шаблон отчёта по лабораторной работе"
subtitle: "Простейший вариант"
author: "Дмитрий Сергеевич Кулябов"

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

Здесь приводится формулировка цели лабораторной работы. Формулировки
цели для каждой лабораторной работы приведены в методических
указаниях.

Цель данного шаблона --- максимально упростить подготовку отчётов по
лабораторным работам.  Модифицируя данный шаблон, студенты смогут без
труда подготовить отчёт по лабораторным работам, а также познакомиться
с основными возможностями разметки Markdown.

# Задание

Здесь приводится описание задания в соответствии с рекомендациями
методического пособия и выданным вариантом.

# Теоретическое введение

Здесь описываются теоретические аспекты, связанные с выполнением работы.

Например, в табл. [-@tbl:std-dir] приведено краткое описание стандартных каталогов Unix.

: Описание некоторых каталогов файловой системы GNU Linux {#tbl:std-dir}

| Имя каталога | Описание каталога                                                                                                          |
|--------------|----------------------------------------------------------------------------------------------------------------------------|
| `/`          | Корневая директория, содержащая всю файловую                                                                               |
| `/bin `      | Основные системные утилиты, необходимые как в однопользовательском режиме, так и при обычной работе всем пользователям     |
| `/etc`       | Общесистемные конфигурационные файлы и файлы конфигурации установленных программ                                           |
| `/home`      | Содержит домашние директории пользователей, которые, в свою очередь, содержат персональные настройки и данные пользователя |
| `/media`     | Точки монтирования для сменных носителей                                                                                   |
| `/root`      | Домашняя директория пользователя  `root`                                                                                   |
| `/tmp`       | Временные файлы                                                                                                            |
| `/usr`       | Вторичная иерархия для данных пользователя                                                                                 |

Более подробно об Unix см. в [@gnu-doc:bash;@newham:2005:bash;@zarrelli:2017:bash;@robbins:2013:bash;@tannenbaum:arch-pc:ru;@tannenbaum:modern-os:ru].

# Выполнение лабораторной работы

1. Откроем Midnight Commander. 

![51.png](image/51.png){ #fig:001 width=90% }

2. Создаем директорию. 

![52.png](image/52.png){ #fig:002 width=90% }

3. Создаем файл lab5-1.

![53.png](image/53.png){ #fig:003 width=90% }

4. Вводим текст программы из листинга. 

![54.png](image/54.png){ #fig:004 width=90% }

5. Вводим текст программы из листинга.

![55.png](image/55.png){ #fig:005 width=90% }

6. Создаем файл lab5-2. 

![56.png](image/56.png){ #fig:006 width=90% }

7. Изменяем код в lab5-2. 

![57.png](image/57.png){ #fig:007 width=90% }

8. Переносим текст из заданий к лабораторной работе. 

![58.png](image/58.png){ #fig:008 width=90% }

9. Вводим свои ФИО, работая в lab5-2. 

![59.png](image/59.png){ #fig:009 width=90% }

10. В файле lab5-2.asm заменим подпрограмму sprintLF на sprint. 

![510.png](image/510.png){ #fig:010 width=90% }

11. В файле lab5-2.asm заменим подпрограмму sprintLF на sprint. 

![511.png](image/511.png){ #fig:011 width=90% }

12. Создадим исполняемый файл и проверим его работу. Посмотрим, в чем разница между sprintLF и sprint.

![512.png](image/512.png){ #fig:012 width=90% }

# Самостоятельная часть лабораторной работы

13. Работаем в папке lab5-3.

![513.png](image/513.png){ #fig:013 width=90% }

14. Получим исполняемый файл и проверим его работу. На приглашение введите строку вводим свою фамилию. 

![514.png](image/514.png){ #fig:014 width=90% }

15. Копируем файл lab5-2.asm.

![515.png](image/515.png){ #fig:015 width=90% }

16. Копируем команды mov eax, buf1; mov ecx, buf1; mov edx, 80; для выполнения команды call sprintLF. 

![516.png](image/516.png){ #fig:016 width=90% }

17. Оттранслируем текст программы lab5-2.asm в объектный файл. Выполним компоновку объектного файла и запустим получившийся исполняемый файл. Программа выводит строку 'Введите строку:' и ожидает ввода с клавиатуры. На запрос введем ФИО 

![517.png](image/517.png){ #fig:017 width=90% }
# Выводы

Здесь кратко описываются итоги проделанной работы.

# Список литературы{.unnumbered}

::: {#refs}
:::
