import random as rd 
import game_data as g
import art as a
import os

def followers(optionA,optionB):
  fA=optionA["follower_count"]
  fB=optionB["follower_count"]
  return fA,fB
    

def check_choice(optionA,optionB):
  score=0
  while True:
    print("\n\n\n")
    print(f'Compare A: {optionA["name"]}, {optionA["description"]}, from {optionA["country"]}\n')
    print(a.vs)
    print (f'Compare B: {optionB["name"]}, {optionB["description"]}, from {optionB["country"]} \n')
    choice=input("Who has more followers? Type 'A' or 'B': ")
    A,B=followers(optionA,optionB)
    if choice=='A'and A>B:
      score+=1
      optionA,optionB=optionA,rd.choice(g.data)
    elif choice=='B' and B>A:
      score+=1
      optionA,optionB=optionB,rd.choice(g.data)
    else:
      
      print(f"Sorry wrong option chosen! \nYour score is: {score}\n")
      score=0
      break
    

while True:
    ch=input("Want to play the game? Type 'y' or 'n': ")
    if ch=='y':
      os.system("clear")
      print(a.logo)
      optionA=rd.choice(g.data)
      optionB=rd.choice(g.data)
      check_choice(optionA,optionB)

    else:
      os.system("clear")
      print("Thank you!")
      break
