---
## Front matter
lang: ru-RU
title: Отчёт по лабораторной работе №13
subtitle: Фильтр пакетов
author:
  - Борисенкова София Павловна
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 27 ноября 2025

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
---

# Цель работы

## Цель

Получить навыки настройки пакетного фильтра и управления брандмауэром в Linux.

# Выполнение лабораторной работы

## Получение привилегий

![Определение зоны и служб](image/1.png){ #fig:001 width=70% }

## Просмотр зон и служб

![Просмотр конфигурации зоны](image/2.png){ #fig:002 width=70% }

## Добавление службы vnc-server

![Добавление vnc-server](image/3.png){ #fig:003 width=70% }

## Добавление порта 2022/tcp

![Добавление порта 2022/tcp](image/4.png){ #fig:006 width=70% }

## Запуск firewall-config

![Настройка служб в firewall-config](image/5.png){ #fig:007 width=70% }

## Применение GUI-настроек

![Применение настроек firewall-config](image/6.png){ #fig:009 width=70% }

## Включение imap

![Добавление imap](image/7.png){ #fig:010 width=70% }
## Включение pop3

![Добавление pop3](image/8.png){ #fig:010 width=70% }

## Включение smtp

![Добавление smtp](image/9.png){ #fig:010 width=70% }

# Итоги работы

## Вывод

* Изучены механизмы управления firewall через firewall-cmd
* Получены навыки работы с временной и постоянной конфигурацией.
* Освоено добавление служб и портов.
* Применены команды и GUI-инструменты 
* Понято различие между runtime и permanent конфигурациями.
