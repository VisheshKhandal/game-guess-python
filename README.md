# game-guess-python
import random

target  = random.randint(1,100)

while True:
    userchoice = input("suppose the number or Quiet(Q) :")
    if(userchoice == "Q"):
        break

    userchoice = int(userchoice)
    if(userchoice == target):
        print("Sucess : Correct Suppose")
        break
    elif(userchoice < target ):
        print("your number is too small.take a bigger guess... " ) 
    else:
        print("your number is too big. take a smaller guess...")    


print("----GAME OVER----")        

