# Number-guessing-game
Basic number guessing game using python
import random
question=input("Wanna play a game??[Y/N]: ")
if question=='y':
    random_number=random.randint(0,100)
    guess=int(input('Guess a nummber between 0 and 100: '))
    c=0
    while random_number!=guess:
        if random_number<guess:
            guess=int(input("Try again! Enter a smaller number:"))
            c=c+1
        if random_number>guess:
            guess=int(input("Try again!Enter a higher number: "))
            c=c+1
    if random_number==guess:
        print("Hurray!You got it!")
if question=='n':
    print("ohh! okay :(")
