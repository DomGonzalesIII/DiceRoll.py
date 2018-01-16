import random

wannaRoll = 'y'

print("Hello, welcome to Dice Roll!")

while wannaRoll == 'y':
    print ('How many sides would you like your die to have?')
    sides = int(input())

    result = random.randint(1,sides)
    result = str(result)
    print ('You rolled a ' + result + ' .')
    print ('Would you like to roll again?(y or n)')
    wannaRoll = input()
            
print('Goodbye')
