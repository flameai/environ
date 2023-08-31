# Библиотека для загрузки и использования переменных среды

## Пример использования:

```python
from common.environ.settings_class import EnvironSettings

class MySettings(EnvironSettings):
    MY_VAR: int = 1

```
при использовании в любом месте кода при старте приложения должна произойти валидация:
(TODO сделать валидацию)

requirements.txt
```text
git+https://github.com/flameai/environ.git@{tag}#common_environ
```

## Линтинг кода и код-стайл:

Установка Flake8 и Black
```sh
pip install -r ./requirements_dev.txt
```
Форматирование:
```sh
black ./common
```

Проверка:
```text
flake8 ./common
```