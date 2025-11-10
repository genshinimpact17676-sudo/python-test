name: Python tests

on: [push]

jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - name: Получение кода
        uses: actions/checkout@v3

      - name: Установка Python
        uses: actions/setup-python@v4
        with:
          python-version: '3.10'

      - name: Установка зависимостей
        run: pip install pytest

      - name: Запуск тестов
        run: pytest
