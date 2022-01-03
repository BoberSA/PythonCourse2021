https://test.pypi.org/project/sbober-fractals/

1. Создание тестов
2. Настройка CI (GitHub Actions)
3. Создание setup.py
4. Подготовка пакета
5. Загрузка в test.pypi.org
6. Установка из test.pypi.org / проверка работы

Для сборки модуля необходим пакет wheel.
Команда:
python -m setup.py bdist_wheel
или
python -m setup.py sdist bdist_wheel

Для загрузки модуля в test.pypi.org необходим пакет twine.
Команда:
twine upload --repository testpypi dist/*