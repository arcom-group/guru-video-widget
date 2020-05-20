# Скрипт интеграции видео контента 24guru.by

Виджет для вывода онлайн видео с продажей для сайта

![Logo](docs/logo.jpeg)

Данное решение основано на технологиях компании [Arcom Group](https://arcom.group) и портала города [24guru](https://24guru.by).

Вопросы/советы/замечания отправляйте на support@arcom.group
Также вы можете обратиться через форму обратной связи на сайте [Arcom Group](https://arcom.group).

Если вы обнаружили какие-то ошибки или опечатки, вы можете написать о них на почту либо сделать пулл-реквест с исправлением. Заранее спасибо!

## Как выглядит

![Screenshot](docs/demo.png)

## Интеграция

Для вывода в iframe

        <iframe src="https://webgate.24guru.by/widgets/video?limit=6&lang=ru" height="300px" width="100%" frameborder="" allowfullscreen></iframe>

Применяемые параметры ссылки для конфигурации вывода:

1. lang - язык, по умолчанию `ru`
2. limit - лимит на количество, целое число, по умолчанию `6`
3. center - включить центрирование, 1 или 0, по умолчанию `1`
4. style - стиль, по умолчанию `default`
5. performanceId - фильтр по мероприятияю, по умолчанию не заполнено
6. objectId - фильтр по обьекту, по умолчанию не заполнено
7. premium - выводить только премиум контент, 1 или 0, по умолчанию `0`
8. contractId - фильтр по контракту, по умолчанию не заполнено


## Примеры

1. Воводы всех видео по определенной площадке

        <iframe src="https://webgate.24guru.by/widgets/video?objectId=1" height="300px" width="100%"></iframe>

2. Вовод только премиум контента для определенной площадки

        <iframe src="https://webgate.24guru.by/widgets/video?objectId=1&premium=1" height="300px" width="100%"></iframe>

3. Ограничить вывод количества видео

        <iframe src="https://webgate.24guru.by/widgets/video?limit=10" height="300px" width="100%"></iframe>

4. Изменить стиль контента

        <iframe src="https://webgate.24guru.by/widgets/video?style=arcom" height="300px" width="100%"></iframe>

    Для применения собственной стилистики, необходимо разработать css файл, и передать его менеджерам компании, для загрузки на CDN сервер. После этого, можно будет использовать собственный стиль. 

## Ссылки

* [Сайт компании Arcom Group](https://arcom.group)
* [Сайт 24guru в Беларуси](https://24guru.by)

<p align="center"><img src="https://arcom.group/img/logo.svg" width="10%"></p>