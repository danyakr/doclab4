# Лабораторная работа 4. Pydoc & Javadoc

Введение
Документация играет ключевую роль в разработке программного обеспечения, помогая другим разработчикам и пользователям понимать и использовать код. В этой работе необходимо научиться документировать код на Python и Java с использованием Pydoc и Javadoc, генерировать статическую HTML-документацию, публиковать её на GitHub Pages и следовать лучшим практикам написания технической документации.

Часть 1: Документирование проекта на Python с использованием Pydoc

– Описание выбранного проекта.
Этот проект представляет собой калькулятор, реализованный как Python-пакет, который включает модули для выполнения основных арифметических операций: сложение, вычитание, умножение и деление. Каждая операция выделена в отдельный модуль, что улучшает структурированность и гибкость кода. Этот подход позволяет легко поддерживать и расширять функционал, а также повторно использовать отдельные модули.

– Примеры добавленных docstring-комментариев.

```python
def add(x, y):
    """
    Возвращает сумму двух чисел.

    Args:
        x (float): Первое число.
        y (float): Второе число.

    Returns:
        float: Результат сложения x и y.
    """
    return x + y
```
```python
class Calculator:
    """
    Класс для выполнения арифметических операций с использованием модулей пакета.

    Методы:
        add(x, y): Возвращает сумму x и y.
        subtract(x, y): Возвращает разницу между x и y.
        multiply(x, y): Возвращает произведение x и y.
        divide(x, y): Возвращает результат деления x на y.
    """

    def add(self, x, y):
        return add(x, y)

    def subtract(self, x, y):
        return subtract(x, y)

    def multiply(self, x, y):
        return multiply(x, y)

    def divide(self, x, y):
        return divide(x, y)
```

– Процесс генерации и публикации документации.
![image](https://github.com/user-attachments/assets/f39e7f83-7f88-455b-8bbf-6f929d0074f8)
![image](https://github.com/user-attachments/assets/6a21ac04-4e42-475b-99f1-121c3d4f347b)
![image](https://github.com/user-attachments/assets/b1793a48-2b1f-40cf-adc6-0c9b4f99df89)


```
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Документация</title>
</head>
<body>
    <h1>Документация</h1>
    <ul>
        <li><a href="main.html">main.html</a></li>
        <li><a href="addition.html">addition.html</a></li>
        <li><a href="division.html">division.html</a></li>
        <li><a href="multiplication.html">multiplication.html</a></li>
        <li><a href="subtraction.html">subtraction.html</a></li>
    </ul>
</body>
</html>

```



– Возникшие проблемы и способы их решения.











Часть 2: Документирование проекта на Java с использованием Javadoc и Maven










https://danyakr.github.io/calcproject/
