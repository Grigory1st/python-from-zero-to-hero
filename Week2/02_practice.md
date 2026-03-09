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
# Your code here
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
# Your code here
```

4. **Password Validator**: Check if password is at least 8 characters and contains a digit.

<details>
<summary>ru</summary>

**Валидатор пароля**: Проверьте, что пароль содержит не менее 8 символов и содержит цифру.

</details>

```python
# Your code here
```

5. **Menu System**: Use a loop to display a menu and respond to user choices.

<details>
<summary>ru</summary>

**Меню системы**: Используйте цикл для отображения меню и реагирования на выбор пользователя.

</details>

```python
# Your code here
```
