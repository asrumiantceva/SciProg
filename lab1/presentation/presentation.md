---
## Front matter
lang: ru-RU
title: Лабораторная работа №1
subtitle: 'Управление версиями'
author: 'Румянцева Александра Сергеевна'
date: 17 сентября, 2022

## Formatting
toc: false
slide_level: 2
theme: metropolis
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Serif
monofont: PT Serif
header-includes: 
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
aspectratio: 43
section-titles: true
---

## Цели и задание на лабораторную работу

Цель: Изучить идеологию и применение средств контроля версий. Освоить умения по работе в git.

Задание: Лабораторная работа подразумевает изучение основных команд в git.

## Выполнение лабораторной работы

1. Изучила теорию и указание к лабораторной работе.

2. Создадим учётную запись на <https://github.com> (рис. 1).

   ![рис. 1. Учетная запись на Github.](images/1.jpg){ #fig:001 width=60% }

Проверила установку git (рис. 2)

   ![рис. 2. Установленная версия Git.](images/2.jpg){ #fig:002 width=60% }

---

3. Сделала предварительную конфигурацию, указав имя email владельца репрозитория (рис 3.).

   ![рис. 3. Указание владельца репрозитория.](images/3.jpg){ #fig:003 width=60% }

---

4. Следующим шагом будет создание и подключение репозитория к GitHub.

В GitHub заходим в «repository» и создаём новый репозиторий (имя «laboratory», а заголовок для файла README). Копируем в консоль ссылку на репозиторий (для дальнейшей работы с файлами):

   ![рис. 4. Создание репозитория.](images/6.jpg){ #fig:006 width=60% }

---

С помощью git добавляем файлы в репозиторий (рис. 5-7)

   ![рис. 5. Добавление файлов в репозиторий 1.](images/7.jpg){ #fig:007 width=60% }

---

  ![рис. 6. Добавление файлов в репозиторий 2.](images/8.jpg){ #fig:008 width=60% }

---

   ![рис. 7. Добавление файлов в репозиторий 3.](images/9.jpg){ #fig:009 width=60% }

   ![рис. 8. Добавленные файлы в репозиторий.](images/10.jpg){ #fig:010 width=60% }

---

## контрольные вопросы

1. Что такое системы контроля версий (VCS) и для решения каких задач они предназначаются?

​Системы контроля версий (Version Control System, VCS) применяются при работе нескольких человек над одним проектом.

2. Объясните следующие понятия VCS и их отношения: хранилище, commit, история, рабочая копия.
​ 
Хранилище (repository), или репозитарий — место хранения всех версий и служебной информации. Commit («[трудовой] вклад», не переводится) — синоним версии; процесс создания новой версии. Рабочая копия (working copy) — текущее состояние файлов проекта, основанное на версии, загруженной из хранилища (обычно на последней).

---

5. Опишите порядок работы с общим хранилищем VCS.

Для последующей идентификации пользователя на сервере репозиториев необходимо сгенерировать пару ключей (приватный и открытый):

ssh-keygen -C "Имя Фамилия work@mail"

Ключи сохраняться в каталоге~/.ssh/.

Скопировав из локальной консоли ключ в буфер обмена

cat ~/.ssh/id_rsa.pub | xclip -sel clip

вставляем ключ в появившееся на сайте поле.

---

9. Что такое и зачем могут быть нужны ветви (branches)?
​
Ветки нужны для того, чтобы программисты могли вести совместную работу над проектом и не мешать друг другу при этом. Кроме того, с помощью branches решаются следующие проблемы: нужно постоянно создавать архивы с рабочим кодом, сложно "переключаться" между архивами, сложно перетаскивать изменения между архивами, легко что-то напутать или потерять.

*более подробно на все контрольные вопросы описаны ответы в отчете

---

## Выводы

Я изучила идеологию и применение средств контроля версий. Освоила умения по работе в git.