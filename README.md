# Treasure_island_game_python

In this project, choices are made. The storyline of the project is to reach the island and get the treasure. The decision should be made which option should he choose. When the project starts the user chooses the path, if he chooses the wrong path game ends. He moves further and reaches the lake.

If he swims he go to next step else, he will die and ends the game. After reaching island he sees a house with three doors. He must choose one to get the treasure. Choosing wrong door leads to end the game. It is a simple game

print("Welcome to Treasure Island.\nYour Mission is to find the treasure.")

step1=input("You are at a road, Where do you want to go? Type right or left: ").lower()
if step1=="left":
    step2=input("You arrived near port, there is an island in the middle of the ocean, Type wait for boat. Type swim to swim across: ").lower()
    if step2=="wait":
        step3=input("You arrived to an island. There is a house with three door, one is red,other is white and third is black, which colour do you choose? ").lower()
        if step3=="white":
            print("Congrulations,You won a Treasure")
        elif(step3=="red"):
            print("You are caught by snake, Game over")
        elif(step3=="black"):
            print("You are attacked by Dragon, Game over")
        else:
            print("Your entered a wrong syntax")
    elif(step2=="swim"):
        print("You are eaten by shark, Game over")
    else:
        print("You entered a wrong syntax")
elif(step1=="right"):
    print("You fell into the hole, Game over")
else:
    print("Your entered a wrong syntax")

print("Game End")
