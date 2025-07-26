# Rock-Paper-Scissors-
#its a game 
import random
def rock_paper_scissors():
    print("welcome to rock paper scissors")
    choice=["rock","paper", "scissor", ]
    player_chice =input("enter use choice :")
    if player_chice not in choice:
        print("invalid chice")
    computer_choice= random.choice(choice)
    print(f"choice of computer{computer_choice}")
    if(player_chice==computer_choice):
        print("its a draw")
    elif(player_chice=="rock" and computer_choice== "scissor")or\
        (player_chice=="paper" and computer_choice== "rock")or\
        (player_chice=="scissor" and computer_choice== "paper"):
        print("you win")
    else:
        print("you loss")

rock_paper_scissors()
