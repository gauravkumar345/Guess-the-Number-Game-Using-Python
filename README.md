# Guess-the-Number-Game-Using-Python
A beginner-friendly project where players try to guess a randomly generated number within a specified range. The game provides feedback on whether the guess is too high or too low, helping players to find the correct number.
 Key Features:
- Random number generation
- User input for guesses
- Feedback on guesses (too high, too low, or correct)
- Loop to allow multiple attempts until the correct number is guessed

This project is perfect for learning basic Python concepts such as loops, conditionals, and user input handling.



import random
num=random.randint(1,100)

while True:
  guess=input("Guess your number or if you want to quit enter(Q):")
  if(guess=="Q"):
    print("You Quit")
    break

  guess=int(guess)
  if(num==guess):
    print("You guess the correct number. YOU WON")
    break
  elif(num>guess):
    print("You guess the smaller number. Guess again a greater number")
  else:
    print("You guess the greater number. Guess again a smaller number")
print(".....GAME OVER.....")
  
