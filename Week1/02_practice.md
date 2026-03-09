# Week 1: Practice Exercises

Practice these exercises to reinforce the concepts. Write the code in a Python file and run it to see the output.

<details>
<summary>ru</summary>

Попрактикуйтесь в этих упражнениях, чтобы закрепить концепции. Напишите код в файл Python и запустите его, чтобы увидеть результат.

</details>

1. **Variable Assignment**: Create variables for your name, age, and favorite color. Print them in a sentence.

<details>
<summary>ru</summary>

**Присваивание переменных**: Создайте переменные для вашего имени, возраста и любимого цвета. Распечатайте их в предложении.

</details>

```python
name = input("Enter your name: ")
age = input("How old are you? ")
color = input("What is your favorite color?")
print(f"Hello, " {name} "! You color is " {color} "and you have" {age} "y.o.")
```

2. **Data Type Conversion**: Take a number as input, convert it to float, and print the result.

<details>
<summary>ru</summary>

**Преобразование типов данных**: Возьмите число в качестве входных данных, преобразуйте его в float и распечатайте результат.

</details>

```python
number = input("Enter a number: ")

try:
    number = int(number)
    print(f"The number you entered is {float(number)}")
except ValueError:
    print("Please enter a valid integer.")
```

3. **Basic Calculator**: Write a script that adds two numbers entered by the user.

<details>
<summary>ru</summary>

**Простой калькулятор**: Напишите скрипт, который складывает два числа, введенные пользователем.

</details>

```python
num_one = input("Enter the first number: ")
num_two = input("Enter the second number: ")
operations = ["+", "-", "*", "/"]
operation = input(f"Choose an operation ({', '.join(operations)}): ")
try:
    num_one = float (num_one)
    num_two = float (num_two)
    if operation == "+":
        result = num_one + num_two
    elif operation == "-":
        result = num_one - num_two  
    elif operation == "*":
        result = num_one * num_two  
    elif operation == "/":
        if num_two != 0:
            result = num_one / num_two  
        else:
            print("Error: Division by zero is not allowed.")
            result = None   
    else:
        print("Invalid operation selected.")
        result = None   
    if result is not None:
        print(f"The result of {num_one} {operation} {num_two} is: {result}")        
except ValueError:
    print("Please enter valid numbers.")
```

4. **String Manipulation**: Ask for the user's first and last name, then print their full name in uppercase.

<details>
<summary>ru</summary>

**Работа со строками**: Попросите имя и фамилию пользователя, затем распечатайте их полное имя в верхнем регистре.

</details>

```python
first_name = input("Enter you first name: ")
last_name = input("Enter you last name: ")
print(f"Full name is {first_name.upper()} {last_name.upper()}")

```

5. **Boolean Logic**: Create a variable for temperature and print whether it's above 20 degrees.

<details>
<summary>ru</summary>

**Булева логика**: Создайте переменную для температуры и распечатайте, выше ли она 20 градусов.

</details>

```python
temp_celsius = input("Enter temperature in Celsius: ")
try:
    temp_celsius = float(temp_celsius)
    temp_fahrenheit = (temp_celsius * 9/5) + 32
    print(f"{temp_celsius}°C is equal to {temp_fahrenheit}°F.")
    if temp_celsius > 20:
        print("It's a warm day!")
    elif temp_celsius < 20:
        print("It's a cold day!")
    else:
        print("It's exactly 20 degrees!")
except ValueError:
    print("Please enter a valid number for temperature.")
```
