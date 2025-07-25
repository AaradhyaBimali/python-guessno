import random
comp= random.randint(1, 100)
while True:
    print("Guess a number 1-100")
    n= input()
    try:
        guess = int(n)
        if comp == guess:
            print("You guessed it!")
            break
        elif comp < guess<= 100:
            print("Too high!")
        elif comp > guess>=0:
            print("Too low!")
        elif guess < 1 or guess > 100:
            print("Invalid input, please enter a number between 1 and 100.")
            break
    except ValueError:
        print("Invalid input, please enter a number between 1 and 100.")
