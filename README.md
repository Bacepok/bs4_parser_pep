# Парсер документации Python + PEP

Парсер позволяет спарсить информацию из документации Python и PEP работает в 4х режимах

## Технологии:

- Python 3.9
- requests-cache 1.0.0
- Beautiful Soup 4.9.3
- lxml 4.9.2 (парсер Beautiful Soup)
- tqdm 4.61 (прогресс-бар)


## Аргументы командной строки


```python
usage: main.py [-h] [-c] [-o {pretty,file}]
               {whats-new,latest-versions,download,pep}

Парсер документации Python

positional arguments:
  {whats-new,latest-versions,download,pep}
                        Режимы работы парсера

optional arguments:
  -h, --help            show this help message and exit
  -c, --clear-cache     Очистка кеша
  -o {pretty,file}, --output {pretty,file}
                        Дополнительные способы вывода данных
```

## Описание работы

**Парсер работает в четырёх режимах:**

1. Парсинг версий Python и их авторов - whats_new;
2. Парсинг информации о версиях - latest_versions;
3. Парсинг информации о стандартах PEP - pep;
4. Загрузка документации - download.

**Вывод информации:**

- стандартный вывод в консоли;
- вывод в консоли в виде таблицы;
- сохранение вывода в файл .csv.

## Запуск парсера
- скачайте архив
- активируйте виртуальное окружение
- установите зависимости
- в директории src запустите требуемую функцию   (whats-new | latest-versions | download | pep)
- управление выводом происходит через аргументы `-o {pretty,file}` - табличный вывод или вывод в файл
- очистка кеша аргумент `-c`
