# Raja-game-
A number prediction game made using JavaScript. Player guesses higher or lower."import random

def number_guessing_game():
    print("🎲 Welcome to the Number Guessing Game!")
    secret_number = random.randint(1, 100)  # random number between 1 and 100
    attempts = 0

    while True:
        guess = int(input("Enter your guess (1-100): "))
        attempts += 1

        if guess < secret_number:
            print("Too low! Try again.")
        elif guess > secret_number:
            print("Too high! Try again.")
        else:
            print(f"🎉 Congratulations! You guessed it in {attempts} attempts.")
            break

number_guessing_game()
