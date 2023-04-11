# Обрезка ссылок с помощью Битли
Скрипт сокращает URL с помощью bitly и показывает количество кликов по битлинку.   

## Окружение
### Зависимости
Python3 должен быть уже установлен. Затем используйте pip (или pip3, есть конфликт с Python2) для установки зависимостей:

```bash
pip install -r requirements.txt
```

### Переменные окружения
- BITLY_TOKEN

1. Поместите файл `.env` рядом с `main.py`.
2. `.env` содержит текстовые данные без кавычек.

Например, если вы распечатаете содержимое `.env`, то увидите:

```bash
$ cat .env
BITLY_TOKEN=token123
```

#### Как получить
Зарегистрируйтесь на [bitly.com](https://bitly.com/) и получите токен на [app.bitly.com/settings/api](https://app.bitly.com/settings/api/)

## Как запустить
Запуск на Linux(Python 3) или Windows:

```bash
$ python main.py url
```

Вы увидите:

```
bit.ly/abc123
```
Или
```
Количество переходов по ссылке битли: 50
```

## Цель проекта
Код написан в образовательных целях на онлайн-курсе для веб-разработчиков [dvmn.org](https://dvmn.org/).