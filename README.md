# Rock_paper_scissor-game-using-python-code-
Using if else condition and randomization module I built a rock paper scissor game.
import random
rock = '''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___) 
'''
paper = '''
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
'''
scissor = '''
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
'''
game_images = [rock,paper,scissor]
user_choice = int(input("What do you choose ? 0 for a rock,1 for a paper or 2 for a scissor\n"))
print(game_images[user_choice])
computer_choice = random.randint(0,2)
print(f"Computer choose:")
print(game_images[computer_choice])
if user_choice >= 3 or user_choice < 0:
    print("your number is invalid,that means you lost")
elif user_choice == 0 and computer_choice == 2:
    print("you won")
elif computer_choice == 0 and user_choice == 2:
    print("you lost")
elif computer_choice > user_choice:
    print("you lost")
elif computer_choice == user_choice:
    print("the game is draw")

elif computer_choice < user_choice :
    print("you won")
