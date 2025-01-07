# ML Business Application HW

Домашняя работа по предмету "Бизнес-применение машинного обучения"

## Задача:

Используя ранее созданные `features.py` `metric.py` `model.py` и другие файлы выполнить следующин шаги:

### Шаг 1

Доработав `features.py` создайте сервис по генерации сообщений.
После каждой итерации сервиса features в файле metric_log.csv должна появляться новая запись с соответствующим идентификатором, истинным ответом, предсказанием и ошибкой.

### Шаг 2

Далее добавьте в ваше приложение логирование метрик.

### Шаг 3

Добавьте к вашей архитектуре ещё один сервис — plot. Скрипт с его кодом назовите plot.py. Данный сервис должен в бесконечном цикле читать таблицу metric_log.csv и строить график распределения (гистограмму) абсолютных ошибок. График должен записываться в файл logs/error_distribution.png.

## Инструкци по запуску

- Убедиться ,что установлен docker и docker-compose
- Скачать репозиторий
- Перейти в директорию
- запустить docker-compose up

для фонового запуска можно использовать `docker-compose up -d`

для остановки:

- запустить docker-compose down

Если внесли изменения в код:

- docker-compose up --build --force-recreate
