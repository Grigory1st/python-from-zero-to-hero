# Week 2: Practice Exercises

<details>
<summary>ru</summary>

Неделя 2: Практические упражнения

</details>

1. **Age Classifier**: Write a program that classifies age into child, teen, adult based on input.

<details>
<summary>ru</summary>

**Классификатор возраста**: Напишите программу, которая классифицирует возраст на ребенка, подростка, взрослого на основе входных данных.

</details>

```python
while True:
    age = input("Enter your age: ")

    try:
        age = int(age)

        if age < 0 or age > 120:
            print("Age is not realistic")
            continue

        if age <= 12:
            print("You are child")
        elif age <= 18:
            print("You are teenager")
        else:
            print("You are already adult")

        break

    except ValueError:
        print("Enter a valid age please")
```

2. **Number Guessing Game**: Generate a random number (use `import random; random.randint(1,10)`) and let user guess until correct.

<details>
<summary>ru</summary>

**Игра в отгадывание числа**: Сгенерируйте случайное число (используйте `import random; random.randint(1,10)`) и позвольте пользователю угадывать, пока не угадает правильно.

</details>

```python
#Number Guessing game

import random
exit_game = False # to track if the user wants to quit

while True:   # outer loop: new game
    number = random.randint(1,100)
    count = 0   

    while True:   # inner loop: user guesses the number
        user_number = input('Guess the number from 1 to 100 (or type "exit" to quit): ')
        
        if user_number.lower() == "exit":
            exit_game = True
            break

        try:
            user_number = int(user_number)
            if not 1 <= user_number <= 100:     # check that the number is within the valid range
                print("The number must be between 1 and 100.")
                continue
            count += 1
            
            if user_number > number:
                print("Less:")
            elif user_number < number:
                print("More:")
            else:
                print(f"You win! It is {number}. You guessed it in {count} {'try' if count == 1 else 'tries'}!")
                break   # exit from the inner loop to generate a new random number
        except ValueError:
            print("Please enter only numbers.")

    if exit_game:
        print("Game exited. Good luck and have fun!")
        break

    # ask the user if they want to play again
    play_again = input("Play again? (y/n):").lower()
    if play_again != "y":
        print("Thanks for playing!")
        break
```

3. **Even/Odd Checker**: Loop through numbers 1-10 and print if even or odd.

<details>
<summary>ru</summary>

**Проверка четности/нечетности**: Пройдитесь циклом по числам 1-10 и распечатайте, четный или нечетный.

</details>

```python
for i in range (1,11)
    print(i,"even" if i % 2 == 0 else "odd")    
```

4. **Password Validator**: Check if password is at least 8 characters and contains a digit.

<details>
<summary>ru</summary>

**Валидатор пароля**: Проверьте, что пароль содержит не менее 8 символов и содержит цифру.

</details>

```python
# Password Validator: Check if password is at least 8 characters and contains a digit.
password = input("Enter the password (at least 8 characters and at least one digit): ")

if len(password) >= 8 and any(char.isdigit() for char in password):
    print("Good password")
else:
    print("Password must be at least 8 characters long and contain at least one digit")
```

5. **Menu System**: Use a loop to display a menu and respond to user choices.

<details>
<summary>ru</summary>

**Меню системы**: Используйте цикл для отображения меню и реагирования на выбор пользователя.

</details>

```python
while True:
    print("\n===== MENU =====")
    print("1. Say Hello")
    print("2. Add two numbers")
    print("3. Exit")
    print("==================")
    
    choice = input("Enter your choice (1-3): ").strip()  # убираем лишние пробелы

    if choice == "1":
        print("\nHello!\n")
    elif choice == "2":
        # Проверяем, что пользователь ввёл числа
        try:
            a = int(input("Enter first number: "))
            b = int(input("Enter second number: "))
            print("Sum:", a + b, "\n")
        except ValueError:
            print("Please enter valid numbers.\n")
    elif choice == "3":
        print("Exiting... Goodbye!")
        break
    else:
        print("Invalid choice. Please enter 1, 2, or 3.\n")
```
