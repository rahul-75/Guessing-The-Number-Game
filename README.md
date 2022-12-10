# Guessing-The-Number-Game

import random

print()
print()
print()
print("__________________________________________________________________GUESS THE NUMBER GAME_______________________________________________________________________")
print()
print()
print()
print("                                                             YOU WILL BE GIVEN 3 CHANCES                                                                  ")
print()
print("                   YOU HAVE TO GUESS THE NUMBER WHICH IS SELECTED RANDOMLY BY US IN THESE 3 GUESSES FROM   / 1  2  3  4  5  6  7  8  9  10  /                 ")
print()
print("ALL THE BEST")

ans="yes"
p=0
while ans=="yes":
    print()
    print("ARE YOU READY???????")
    print()
    print()
    ans=input()
    print()
    print("OKEY WE HAVE SELECTED THE NUMBER ITS TIME FOR YOUR GUESS ")
    print()
    n=random.randrange(1,11)
    for i in range(3):
        print()
        a=int(input("TYPE IN YOUR GUESS="))
        if i==0:
            if a<n:
                print("YOUR GUESS WAS TOO SMALL")
                print("YOU HAVE TWO MORE TRY !!")
            elif a>n:
                print("YOUR GUESS WAS TOO HIGH")
                print("YOU HAVE TWO MORE TRY !!")
            elif a==n:
                print("CONGRATSSSS !!!!!!!!!!!!!!!!!")
                print()
                p=p+10
                print("you got 10 points")
                break

        if i==1:
            if a<n:
                print("YOUR GUESS WAS TOO SMALL")
                print("YOU HAVE ONE MORE TRY !!")
            elif a>n:
                print("YOUR GUESS WAS TOO HIGH")
                print("YOU HAVE ONE MORE TRY !!")
            elif a==n:
                print("CONGRATSSSS !!!!!!!!!!!!!!!!!")
                print()
                p=p+10
                print("you got 10 points")
                break

        if i==2:
            if a<n:
                print("YOUR GUESS WAS TOO SMALL")
                print("ITS WAS YOUR LAST TRY !!!!!!!!")
            elif a>n:
                print("YOUR GUESS WAS TOO HIGH")
                print("ITS WAS YOUR LAST TRY !!!!!!!!")
            elif a==n:
                print("CONGRATSSSS !!!!!!!!!!!!!!!!!")
                print()
                p=p+10
                print("you got 10 points")
                break
    print()
    print()
    print("                                                   YOUR CURRENT SCORE IS =",p)
    print()
    print()
    ans=input("DO YOU WANT TO CONTINUE YES/NO=")
print()
print()
print("________________________________________________________________YOUR FINAL SCORE IS=",p,"______________________________________________________________________")
print()
print()
print()
print("__________________________________________________________________THANK YOU FOR PLAYING________________________________________________________________________")
    
        
        
        
    
