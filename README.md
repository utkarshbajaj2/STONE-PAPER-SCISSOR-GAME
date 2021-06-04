# STONE-PAPER-SCISSOR-GAME
import random
list=["stone","paper","scissor","E"]
print("WELCOME TO THE SPS GAME")
st=input("PRESS 'S' TO START THE GAME")
if st=="S":
    y=1
    while y<5:
        print("SELECT YOUR CHOICE : (STONE,PAPER,SCISSOR)")
        print("PRESS 'E' IF YPU WANT TO END THE GAME")
        yes=input()
        print("your choice : ",yes)
        if yes=="E":
            print("END OF GAME,THANK YOU FOR PLAYING")
            break

        choice=random.choice(list)
        print("computers choice:" ,choice)

        if choice==yes:
            print("draw")
        elif yes=="stone" and choice=="paper":
            print("you lost")
        elif yes=="stone" and choice=="scissor":
            print("you won")
        elif yes == "paper" and choice =="stone":
            print("you won")
        elif yes == "paper" and choice == "scissor":
            print("you lost")
        elif yes == "scissor" and choice =="stone":
            print("you lost")
        elif yes == "scissor" and choice == "paper":
            print("you won")
        
    y=y+1

else:
    print("THANK YOU")
