---
# Front matter
lang: ru-RU
title: 'Отчёт по лабораторной работе 2'
subtitle: 'Тема лабораторной работы: Markdawn'
author:
- "Студент: Румянцева Александра Сергеевна, 1132223493"
- "Группа: НПМмд-02-22"
- "Преподаватель: Кулябов Дмитрий Сергеевич,"
- "д-р.ф.-м.н., проф."
date: "Москва 2022"

# Formatting
toc-title: 'Содержание'
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: lualatex
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text

  - \usepackage{titling}
  - \setlength{\droptitle}{-9em}
  - \pretitle{\begin{center}
      \textbf{РОССИЙСКИЙ УНИВЕРСИТЕТ ДРУЖБЫ НАРОДОВ}\\
      \textbf{Факультет физико-математических и естественных наук}\\
      \textbf{Кафедра прикладной информатики и теории вероятностей}
      \vspace{9cm}
      \LARGE\\}
  - \posttitle{\vskip 1em \Large \emph{\textit{Дисциплина$:$ Научное программирование}} \end{center}}
  - \preauthor{\vskip 3em \begin{flushright} \large \begin{tabular}[t]{c}}
  - \postauthor{\end{tabular}\par\end{flushright} \vfill \vskip 5em}
---

# Цель работы

Научиться оформлять отчёты с помощью легковесного языка разметки Markdown.

# Задание

Сделать отчёт по предыдущей лабораторной работе в формате Markdown. В качестве отчёта предоставить отчёты в 3 форматах: pdf, docx и md (в архиве, поскольку он должен содержать скриншоты, Makefile и т.д.)

# Теоретическое введение

Вся теоретическая часть по использованию языка разметки Markdown была взята из инструкции по лабораторной работе №2 на сайте ТУИС РУДН [1].

# Выполнение лабораторной работы

1. Я изучила инструкцию для выполнения работы.

2. Для данной работы я создавала отчёт по лабораторной работе по дисциплине "Математические основы защиты и нформации и информационной безопасности".

Разберём основные моменты, которые были мною написаны с помощью Markdawn для создания отчета.

На рис. 1 показано оформление титульного листа, а именно: заголовка, подзаголовка, указание автора и его харакетистик, указание даты выполнения работы.

   ![Рис. 1. Оформление титульного листа отчета.](images/1.jpg){ #fig:001 width=60% }

На рисунке 2 видим автоматическое создание раздела содержаниеи и списков рисунков и таблиц (для пдф), а также указание к оформлению текста (шрифт, отступ, шрифты  и тп), указаны используемые языки в тексте отчета, и способ конвентаризации в пдф (через lualatex).

   ![Рис. 2. Указания к оформлению файлов и форматированию текста.](images/2.jpg){ #fig:002 width=60% }

На рис. 3 интересен второй абзац, который добавляет оформление к титульному листу для конвертированного в пдф файла.

   ![Рис. 3. Техническая информация и указания к оформлению.](images/3.jpg){ #fig:003 width=60% }

На рис. 4 начинается описание самой работы. Видно применение создания заголовков для глав работы, например, цели работы и задачи, которые обозначения знаком "#". Далее на рис. 4 приненено полужирное начертание текста с помощью двайных звёздочек в начале и в конце фраз, которые было необходимо выделить. А в главах задач и в теоретической части видно оформление пронумерованного списка.

   ![Рис. 4. Оформнение основной части работы с применением заголовков глав текста, полужирного шрифта, нумерационного списка.](images/4.jpg){ #fig:004 width=60% }

На рис. 5  начинается описание практической части работы. Видно применение создания заголовков разных уровней, то есть глав и их подглав, например, "Выполнение лаборатоной раборы" - это глава, а "Маршрутное шифрование" и "Метод решеток", обозначенные "##" - её подглавы. Далее на рис. 5 приненено курсивное начертание текста с помощью одинарной звёздочки в начале и в конце фраз, которые было необходимо выделить. На рисунке 5 также показано как добавлять рисунок/картинку в отчет: через ![название рисунка](путь к рисунку для его нахождения){#fig: порядковый номер рисунка в отчете width=размер/разрешение рисунка%}

   ![Рис. 5. Оформление практической работы с использованием заголовков разных уровнений, курсивного текста, добавлления рисунков.](images/5.jpg){ #fig:005 width=60% }

Оформление ссылок показано на рис 6, а именно это возможно через < ссылка >

   ![Рис. 6. Оформление активных ссылок в тексте.](images/6.jpg){ #fig:006 width=60% }

3. Конфертирование в docx и pdf, просмотр результата.

Конвертировала текст с помощью командной строки используя:

pandoc --filter pandoc-crossref -o report.docx report.md

pandoc --filter pandoc-crossref -o report.pdf report.md

В папке заранее находился Makefile, файл пандок, папка с фотографиями, которые добавлялись в отчет.

- Рассмотрим ворд файл (рис. 7-10).

   ![Рис. 7. Docx файл. Титульный лист и содержание.](images/7.jpg){ #fig:007 width=60% }

   ![Рис. 8. Docx файл. Заголовок главы, полужирный шрифт, пронумерованный список.](images/8.jpg){ #fig:008 width=60% }

   ![Рис. 9. Docx файл. Заголовки разных уровней, курсивный шрифт, добавленный рисунок с подписью.](images/9.jpg){ #fig:009 width=60% }

   ![Рис. 10. Docx файл. Активные ссылки в тексте.](images/10.jpg){ #fig:010 width=60% }

Как видно, в ворд файле успешно отображается титульный лист содержание с заголовками разных уровней (что аналогично видно и в тексте), полужирный и курсивный шрифты, есть активные ссылки и нумерованные списки.

- Рассмотрим пдф файл (рис. 11-17).

   ![Рис. 11. Pdf файл. Титульный лист.](images/11.jpg){ #fig:011 width=60% }

   ![Рис. 12. Pdf файл. Содержание.](images/12.jpg){ #fig:012 width=60% }

   ![Рис. 13. Pdf файл. Список рисунков (фигур).](images/13.jpg){ #fig:013 width=60% }

   ![Рис. 14. Pdf файл. Список таблиц](images/14.jpg){ #fig:014 width=60% }

   ![Рис. 15. Pdf файл. Заголовки тем, полужиный шрифр, нумерованный список.](images/15.jpg){ #fig:015 width=60% }

   ![Рис. 16. Pdf файл. Заголовки разных уровней, курсивный шрифт, добавленный рисунок с подписью.](images/16.jpg){ #fig:016 width=60% }

   ![Рис. 17. Pdf файл. Активные ссылки в тексте.](images/17.jpg){ #fig:017 width=60% }

Как видно на рисунках, особенно на рисунке с содержанием (рис. 12), на каждая тема в пдф файле начинается с новой страницы, будь то содержание или список таблиц.

На рис. 11 видно оформление титульной страницы, а отличаи от ворд файла по правила оформления автор указан с правого края после названия, дата внизу страницы (что сказывалось в файле на рис. 1), и дополнительно на титульный лист добавись данные из рис. 3 об университете и тп. 

Далее на рис 13 видим автоматически сформированный список рисунков из отчета, а на рис. 14 - список таблиц. Он является пустым, поскольку в отчете не использовались таблицы. Далее на рисунках 15-17 аналогично файлам ворд видим успешное оформление текста различными стилями и с использованием заголовков разного уровня темами и тп.

# Библиография

1. ТУИС РУДН <https://esystem.rudn.ru/pluginfile.php/1712589/mod_resource/content/4/003-lab_markdown.pdf>

# Выводы

Я научилась оформлять отчёты с помощью легковесного языка разметки Markdown.