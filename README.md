import random
import time

# methods
def diceRoll(numSides):
    roll = random.randint(1,numSides)
    return roll

#variables
wannaRoll = 'y'

#main
print("Hello, welcome to Dice Roll!")
time.sleep(1)

print ('How many sides would you like your die to have?')
sides = int(input())

while wannaRoll == 'y':

    result = diceRoll(sides)
    result = str(result)
    print ('You rolled a ' + result + ' .')
    time.sleep(1)
    print ('Would you like to roll again?(y or n)')
    wannaRoll = input()

    if wannaRoll == 'y':
        print ('Same number of sides?(y or n)')
        sidesQ = input()

        if sidesQ == 'y':
            wannaRoll = 'y'

        else:
            print('How many sides would you like your new die to have?')
            sides = input()
            sides = int(sides)
    else:
        wannaRoll = 'n'
            
print('Goodbye!')
