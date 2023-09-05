# PhoneNumberParser
______
**PhoneNumberParser** - это программа предназначенная для обработки некорректно
написанных номеров телефонов, она приводит все номера к единому стилю.

Этот проект создан для людей, работающих с CRM системами и создающих рассылку 
звонков с опросами. Обычно, автоматизированный сборщик номеров собирает номера в 
разных стилях, из разных стран в таблицу или текстовый файл, моя программа
позволяет получить из такого файла отформатированные корректные данные, записанные в 
файл, при этом сортирую номера в зависимости от региона.
``` python
+7 (999) 999-99-99                ----->     +79999999999
+7 999 999 99 99 ВА               ----->     +79999999999
89999999999 бабушка               ----->     +79999999999
+7 (999) 999 99 99                ----->     +79999999999
'+7 (999) 9999999, +79999999999   ----->     +79999999999
                                             +79999999999
```
Так же программа позволяет выбрать необходимый общий стиль форматирования.
``` python
+79999999999 or +7(999)999-99-99
```

***Взаимодействие с пользователем:***

Запуская файл `GraphicalInterface.py` через IDE или консоль, будет открыт графический интерфейс:

![example](https://github.com/ArtemStriver/GraphicalInterface.py/blob/master/example.png)

В нем представлен пользователю следующий функционал:
 - Выбрать стиль форматирования номера;
 - Выбрать исходный файл, данные из которого надо отформатировать;
 - Выбрать директорию, в которую будет сохранен результат;
 - Запустить обработку.

## Установка и запуск

Для установки данной программы нужно скачать репозиторий со всеми файлами с GitHub.
Создать виртуальное окружение, но можно использовать и коренную папку, далее загрузить
туда все необходимые пакеты с помощью команды: 
``` python
pip install -r requirements.txt
```
После этого можно запустить файл `GraphicalInterface.py` и приступить к работе.

Или, если вы используете Windows с x64-битной системой, можете попробовать запустить программу через 
`exe` файл, расположенный в папке `GraphicalInterface`.

## Используемые технологии

![version](https://img.shields.io/badge/python-3.11-blue)


![package](https://img.shields.io/badge/PyQt5-5.15.9-violet)
![package](https://img.shields.io/badge/openpyxl-3.1.2-violet)
![package](https://img.shields.io/badge/pyinstaller-5.13.0-violet)


![license](https://img.shields.io/badge/license-Apache__License__V2.0-green)

## Лицензия

Проект разработан с использованием лицензии [Apache License, Version 2.0](https://opensource.org/license/apache-2-0/)
