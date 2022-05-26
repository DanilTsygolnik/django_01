## Подготовка

### Настройка окружения

Работа производится в ОС Manjaro Linux (Arch-based).

В ОС должен быть установлен python версии 3.3+, тогда не придется дополнительно устанавливать дополнительный пакет [python-virtualenv](https://archlinux.org/packages/?name=python-virtualenv).

Убеждаемся в наличии:
```
$ python3 --version
Python 3.10.4

$ python3 -m venv --help
usage: venv ...

$ pip3 --version
pip 22.1.1 from /home/username/.local/lib/python3.10/site-packages/pip (python 3.10)
```

Перед работой с виртуальным окружением проводим апргрейд `pip`:[^pip-usage] 
```
$ python3 -m pip install --upgrade pip
```

Настраиваем виртуальное окружение для проекта:
```bash
# создаем виртуальное окружение django_env
$ python3 -m venv /home/user/path/to/django_env

# активируем виртуальное окружение
$ source /home/user/path/to/django_env/bin/activate

# устанавливаем django
(django_env)$ python -m pip install django
```



[^pip-usage]: https://note.nkmk.me/en/python-pip-usage/
