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

![image](https://github.com/user-attachments/assets/6441c6cc-5673-44bb-bdf3-2d431ac43573)
![image](https://github.com/user-attachments/assets/2221da9f-b917-432d-a6fd-9c7d3182432f)




Часть 2: Документирование проекта на Java с использованием Javadoc и Maven

– Описание выбранного проекта.
Этот проект представляет собой простой калькулятор, реализованный на языке Java. Он поддерживает основные арифметические операции: сложение, вычитание, умножение и деление. Все операции реализованы в одном классе Calculator, что делает структуру проекта простой и компактной. Пользователь может использовать калькулятор для выполнения базовых математических вычислений.

Примеры добавленных Javadoc-комментариев.

```
/**
 * Класс Main для демонстрации работы калькулятора.
 * 
 * Этот класс служит точкой входа в программу и демонстрирует использование
 * класса {@link Calculator} для выполнения основных арифметических операций.
 * В методе {@link #main(String[])} выполняются примеры сложения, вычитания, 
 * умножения и деления с выводом результатов на консоль.
 */
public class Main {
```
```
/**
     * Выполняет сложение двух чисел.
     *
     * @param a Первое число.
     * @param b Второе число.
     * @return Сумма a и b.
     */
    public double add(double a, double b) {
        return a + b;
    }
```

Генерация документации с помощью Javadoc.

![image](https://github.com/user-attachments/assets/867042bf-f000-4866-b34f-02e26cb0bb56)
![image](https://github.com/user-attachments/assets/7423284a-353b-44ee-8736-bc8223a57b91)



Генерация документации с помощью Maven.
![image](https://github.com/user-attachments/assets/67f035ed-28dd-4837-a97a-85df035e7344)
![image](https://github.com/user-attachments/assets/56bc0963-7e73-4545-ba18-cf9b76858bb1)










https://danyakr.github.io/calcproject/
https://danyakr.github.io/javadocproject/
https://danyakr.github.io/javamavenproject/



https://github.com/danyakr/calcproject
https://github.com/danyakr/javadocproject
https://github.com/danyakr/javamavenproject
