- 👋 Hi, I’m @Nitish2222
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Nitish2222/Nitish2222 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
echo "# Python-intern-at-internspedia-" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/Nitish2222/Python-intern-at-internspedia-.git
git push -u origin main


import random

# Intro
print("Welcome to Dan's number guessing game!\n")

# Define variables
guesses = 0
number = random.randint(0, 10)

# Main program loop
while( guesses < 3 ):
    u_guess = int(input("Have a guess: "))

    if u_guess == number:
        print("Well done, you win!")
        break
    elif u_guess > number:
        print("Your guess was too high.")
        guesses = guesses + 1
    elif u_guess < number:
        print("Your guess was too low.")
        guesses = guesses + 1
    else:
        print("There was an error.")

if guesses == 3:
    print("You lose!")
    print("The number was: " + str(number))
