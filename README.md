import time
import random
# story's lists
weapons = ["gun",  "sniper", "shoutgun"]
forest_monsters = ["scp-096 monster", "slender man", "siren head monster"]
cave_monsters = ["ghost", "giant cobra", "zombie"]
# play again fanction  


def play_again():
    print("do you want play again ?")
    play_again= input ("To play again enter 1 \nTo exit game enter 2 :")
    while(play_again) != "1" and (play_again) != "2": 
        print("error")
        play_again= input ("To play again enter 1  \nTo exit game enter 2 :")
    if play_again == "1":
        print("fantastic!!..... \n u will try again")
        main_game()
        check()
        tree()
        shout()
        cave()
    elif play_again == "2":
        print("okay , we hope you enjoy playing our game")
        print("see u later \nHave a Good day")
# main game fanction
 
 
def main_game():        
# Welcome massage
    print("welcome to our adventure & horror game")
    time.sleep(1)
    Name = input ("To start , please enter your name \n")
    while len (Name) == 0:
        print("error")
        Name = input ("To start , please enter your name \n")
#how to win
    print("ok,now you will start playing ")
    print("and you will face some monestrs and hurdels ")
    print("so you must scape form here to win")
    time.sleep(5)
# game's story
    print("one day you  decided to go on trip ")
    print("to camb at the forest that located in deserted tropical island .")
    time.sleep(5)
    print("it is said that there are some monsters and ghosts on this island")
    print("but you are a person who does not believe in these myths")
    print("and you wanted to confirm for your self , especially .")
    time.sleep(5)
    print("since this has some pictures on the internet that highlight")
    print("then beauty of island, including the beach and trees. ")
    time.sleep(5)
    print(" well , you arrived on the island .")
    print("you cheacked the place and found it quiet .")
    print("you set up your tent , and the night fell upon you .")
    print("you let a fire and decided to sleep .")
    time.sleep(5) 
    print(" at midnight.......")
    time.sleep(1)
    print("what is this ?!.... there is a sound coming from outside your tent")
    print("it sound very terrifying and disturbing")
    time.sleep(1)
    print("if you want to go out your tent enter 1")
    print("if you want to still your place enter 2")
# check the place


def check():
    check = input ("enter 1 or 2 : ")
    while True:
        if check == "1":
            print("well , you now exit your tent carefully")
            print("with torch in your hand in front of you is a large tree ")
            print("if you want to hide behind it ,enter 1")
            print("continue to discovery the source of the sound enter 2 ")
            break
        elif check == "2":
            print("u have decided to continue sleeping and ignore this sound")
            time.sleep(2)
            print("10 minutes later......")
            time.sleep(1)
            print("you wake up to the sound of footsteps")
            print("that seemed to be those of one of the giants.")
            print("you are think that they were an elephant but WAIT!!")
            print("you are hearing the same terrifying sound again!! so...")
            print("you decided to check out side  ")
            time.sleep(2)
            print("be carefull")
            print("wow!! what a giant tree")
            time.sleep(2)
            print("if you want to hide behind the tree ,enter 1")
            print("to continue to discovery the source of the sound enter 2 ")
            break
        else:
            print("wrong")
            check = input ("enter 1 or 2 :")
#desapper


def tree():
    tree = input ("enter 1 or 2 : ")
    while True:
        if tree == "1":
            print("you are hidding behind the tree....oh!?")
            time.sleep(1)
            print ("what is this sound....")
            print("oh! ..how lucky you are?! this is a... ")
            print( random.choice(weapons) + " under your hand take it quickly")
            print("what is this!!... u turn to see who is behaind you and...")
            print("oops!!")
            time.sleep(4)
            print("it's a "+random.choice(forest_monsters))
            print("to shout the monster enter 1 , to scape 2")
            break
        elif tree == "2":
            print("well")
            time.sleep(1)
            print("go on your way carefully")
            time.sleep(2)
            print("hshhhhhhh... what is this")
            time.sleep(2)
            print("oh! ..how lucky you are?! this is a... ")
            print( random.choice(weapons) + " under your leg take it quickly")
            time.sleep(4)
            print("what is this!!... u turn to see who is behaind you and....")
            print("oops!!")
            time.sleep(4)
            print("it's a "+random.choice(forest_monsters))
            print("to shout the monster enter 1 , to scape 2")
            break
        else:
            print("wrong")
            tree = input ("enter 1 or 2 :")
#shout the monster


def shout():
    shout= input ("enter 1 or 2 : ")
    while True:
        if shout=="1":
            print("you shot the monster in his head but.....")
            time.sleep(3)
            print("he was unaffected and continued following you.... so.....")
            time.sleep(2)
            print(" ruuuuuuuun quickly he is not stop following you")
            print("there is a cave......\n quickly hide in it")
            print("10 minutes later.....")
            time.sleep(1)
            print("Hushhhh, listen.... what is this!!")
            print("it seems that the monster has moved away")
            print("the sound of his steps is barely audible... ")
            print("in this case you have 2 options :")
            print("either go out and return to your tent")
            print("Or enter the depth of the cave ")
            time.sleep(2)
            print("Warning!!")
            print(" maybe you will meet monsters into the cave")
            time.sleep(2)
            print("return to the tent enter 1")
            print("enter the depth of the cave enter 2")
            break
        elif shout == "2":
            print("Well, you have no other choice so...")
            time.sleep(2)
            print(" ruuuuuuuun quickly he is following you")
            time.sleep(4)
            print("a few moments later of running.....")
            print("there is a cave......\n quickly hide in it")
            time.sleep(2)
            print("10 minutes later.....")
            time.sleep(4)
            print("Hushhhh, listen.... what is this!!")
            print("it seems that the monster has moved away")
            print("the sound of his steps is barely audible... ")
            time.sleep(2)
            print("in this case you have 2 options :") 
            print("either go out and return to your tent")
            print("Or enter the depth of the cave ")
            time.sleep(2)
            print("Warning!!")
            print(" maybe you will meet monsters into the cave")
            time.sleep(2)
            print("return to the tent enter 1")
            print("enter the depth of the cave enter 2")   
            break
        else:
            print("wrong")
            shout= input ("enter 1 or 2 : ")
#the cave


def cave():
    cave = input ("enter 1 or 2 :")
    while True:
        if cave == "1":
            print("well , now you are leaving the cave be carfull")
            print("NOOOOOOOOOOOOO!!")
            time.sleep(2)
            print("what a bad lucky.")
            print("I wanted to tell you that there is trap in front of you")
            print("but you were hasty and fill into it") 
            print("It was made by the monster")
            print("You are lose\n Game over")
            break
        elif cave == "2":
            print("The cave seems very dark..... ")
            time.sleep(2)
            print("but fortunatelly for you")
            print("there is a torch in front of you on the wall .")
            print("Take it and continue ")
            time.sleep(2)
            print("2 minutes later")
            time.sleep(2)
            print("on your way")
            time.sleep(2)
            print("Oh my god , more options .") 
            print("you have 2 entrancs")
            print("one on the right and the other on the left")
            inter = input ("To the right enter 1 To the left enter 2 :")
            while True:
    
                if inter=="1":
                    print("well,be carful")
                    time.sleep(2)
                    print("5 minutes later...")
                    time.sleep(2)
                    print("what a bad day what a bad lucky it's a..")
                    print(random.choice (cave_monsters))
                    print(" quickly take your wepon..... ")
                    time.sleep(2)        
                    print("whattttt!!.. you are joking..where's the wepone?!")
                    time.sleep(2)
                    print("oops! the monster kille you")
                    time.sleep(2)
                    print("you are lose....")
                    print("GAME OVER")
                    break
                elif inter =="2":
                    print("well,be carful")
                    time.sleep(2)
                    print("5 minutes later...")
                    time.sleep(2)
                    print("oh my God!...")
                    time.sleep(2)
                    print("it's an entrance....but what is this ...")
                    time.sleep(2)
                    print("the cave is collapses.... ruuuuuuuuuun")
                    time.sleep(5)
                    print("oh... you miraclously survived..... look!!")
                    print("it's a boat take it quickly to scape")
                    time.sleep(2)
                    print("DONE")
                    time.sleep(2)
                    print("you are win")
                    break
                else:
                    print("wrong")
                    inter = input ("To the right prees 1 To the left prees 2 :")
            break        
        else:
            print("wrong")
            cave = input ("enter 1 or 2 :")
    play_again()
main_game()
check()
tree()
shout()
cave()
