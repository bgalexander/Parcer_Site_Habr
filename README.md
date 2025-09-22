# Parcer_Site_Habr
Скрипт парсит страницу свежих статей Хабра — https://habr.com/ru/articles/ — и выводит в консоль только те публикации, в превью которых встречается хотя бы одно из заданных ключевых слов.

## Формат вывода:

<дата> – <заголовок> – <ссылка>

## Пример
2025-09-22 – Как мы ускорили web-сервис – https://habr.com/ru/articles/123456/
2025-09-21 – Python: практики профилирования – https://habr.com/ru/articles/654321/

## Требования

Python 3.8+
Скрипт использует from __future__ import annotations, поэтому корректно работает на 3.8–3.12.

## Пакеты:

requests

beautifulsoup4
(Опционально: lxml — для более быстрого парсинга; в текущей версии используется встроенный html.parser.)

## Установка

Рекомендуется использовать виртуальное окружение.

python -m venv .venv
Windows:
.venv\Scripts\activate

macOS / Linux:
source .venv/bin/activate

python -m pip install --upgrade pip
python -m pip install -r requirements.txt
