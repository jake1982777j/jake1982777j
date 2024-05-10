- 👋 Hi, I’m @jake1982777j
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
jake1982777j/jake1982777j is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
import random

def start_game():
    print("Welcome to the Math Game!")
    print("Choose an operation:")
    print("A) Addition")
    print("B) Subtraction")
    print("C) Multiplication")
    print("D) Exit")
    choice = input("Enter your choice: ")
    if choice.upper() == "A":
        addition_game()
    elif choice.upper() == "B":
        subtraction_game()
    elif choice.upper() == "C":
        multiplication_game()
    elif choice.upper() == "D":
        print("Goodbye!")
    else:
        print("Invalid input. Try again!")
        start_game()

def addition_game():
    num1 = random.randint(0, 9)
    num2 = random.randint(0, 9)
    answer = num1 + num2
    user_answer = int(input(f"What is {num1} + {num2}? "))
    if user_answer == answer:
        print("Correct!")
    else:
        print(f"Sorry, the correct answer is {answer}.")
    start_game()

def subtraction_game():
    num1 = random.randint(0, 9)
    num2 = random.randint(0, num1)
    answer = num1 - num2
    user_answer = int(input(f"What is {num1} - {num2}? "))
    if user_answer == answer:
        print("Correct!")
    else:
        print(f"Sorry, the correct answer is {answer}.")
    start_game()

def multiplication_game():
    num1 = random.randint(0, 9)
    num2 = random.randint(0, 9)
    answer = num1 * num2
    user_answer = int(input(f"What is {num1} * {num2}? "))
    if user_answer == answer:
        print("Correct!")
    else:
        print(f"Sorry, the correct answer is {answer}.")
    start_game()

start_game()
