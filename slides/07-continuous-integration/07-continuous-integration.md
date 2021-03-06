# Непрерывная интеграция

<!-- ![](./pix/) -->

Кирилл Корняков (Itseez, ННГУ)\
Ноябрь 2013

<!-- TODO
  - Написать подробнее про BuildBot
  - Рассмотреть конфиги Travis
  - Рассмотреть построение других артефактов (документация, дистрибы)
-->

# Содержание

  1. Практика непрерывной интеграции
  1. Системы непрерывной интеграции
  1. Travis CI
  1. BuildBot

# Непрерывная интеграция

> **Непрерывная интеграция (англ. Continuous Integration)** — это практика
> разработки ПО, которая заключается в выполнении частых автоматизированных
> сборок проекта для скорейшего выявления и решения интеграционных проблем.

Непрерывная сборка - это **сердцебиение** вашего проекта.

# Требования к проекту

  1. Исходный код и все, что необходимо для сборки и тестирования проекта,
     хранится в **централизованном репозитории**;
  1. Операции копирования из репозитория, сборки и тестирования всего проекта
     **автоматизированы**.

<center>![](./pix/bbot-overview.png)<center>

# Задачи выделенного сервера

  - Получение исходного кода из репозитория;
  - Сборка проекта;
  - Выполнение тестов;
  - Отправка отчетов;
  - Развёртывание готового проекта.

# Триггеры

  - На обновление состояния репозитория
  - Работа по расписанию (nightly testing)
  - Ручной запуск

# Примеры систем

  - Hudson > Jenkins
  - CruiseControl (CruiseControl.NET), TeamCity
  - Travis CI (аналог <https://drone.io>)
  - BuildBot

# Travis CI

+---------------------+------------------------------------------------------------+
|![](./pix/travis.png)| - Веб-сервис для сборки и тестирования ПО                  |
|                     |   ([open-source](<https://github.com/travis-ci/travis-ci>))|
|                     | - Важными особенностями являются интеграция с GitHub       |
|                     |   и возможность бесплатного использования                  |
|                     | - Поддерживает большое количество языков: C, C++,          |
|                     |   Clojure, Erlang, Go, Groovy, Haskell, Java,              |
|                     |   JavaScript, Perl, PHP, Python, Ruby и Scala              |
|                     | - Тестирование происходит на виртуальных Linux-машинах,    |
|                     |   запускаемых в облаке Amazon (Amazon S3)                  |
|                     | - Официальный сайт проекта: <http://travis-ci.org>         |
+---------------------+------------------------------------------------------------+

# BuildBot

+------------------------+----------------------------------------------------------+
|![](./pix/bbot-logo.png)| - Инструмент непрерывной интеграции                      |
|                        | - Используется в ряде крупных проектов: Chromium, WebKit,|
|                        |   Firefox, Python, OpenCV                                |
|                        | - Реализован на Python, как результат переносим и        |
|                        |   допускает кастомизацию (программирование билдеров)     |
|                        | - Проект разрабатывается на                              |
|                        |   [GitHub](<https://github.com/buildbot/buildbot>),      |
|                        |   тестируется при помощи                                 |
|                        |   [Travis CI](https://travis-ci.org/buildbot/buildbot/)  |
|                        | - Официальный сайт проекта: <http://buildbot.net>        |
+------------------------+----------------------------------------------------------+

# BuildBot

<center>![](./pix/bbot-overview.png)<center>

# Резюме

  1.

# Контрольные вопросы

  1.

# Ссылки

  1.

# Спасибо!

Вопросы?
