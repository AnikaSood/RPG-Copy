# Fantasy Text-Based Role-Playing Game
You are stuck in an unknown world, Hyperion! A text based rpg where the player will need to fight monsters and bosses in order to escape from a mysterious world. The player can interact with the game by typing in specified keys to venture around the world. Be careful when figting enemies though! If you lose to much health - the game will end.

Team Members:

Kayla Tran: https://github.com/kayla-tran

Anika Sood: https://github.com/AnikaSood 

Angelina Guzman http://github.com/linaguz020 

Krish Shah: https://github.com/KrishShah1


 # Why is it important or interesting to you?

We find a text-based game an interesting idea because it grants us the creative freedom to formulate a story and mechanics. Additionally, this project idea gives us the opportunity to explore project development with an emphasis on user experience. Building this game also calls for the implementation of many technical tools that we have learned in previous computer science courses. This will help us become proficient coders as we practice real world applications of these high-level concepts.  


# What languages/tools/techniques do you plan to use?
We plan to code in C++. As the developers, implementing a text-based game will help us practice and exercise our knowledge of data structures, object-oriented programming, and github flow.


# What will be the input/output of your project? What are the features that the project provides?
The basic idea is that the game will be a single player open world role-playing game (RPG). The player will traverse the “world” fighting monsters to become stronger with the goal being to escape a mysterious world in order to return back to real life. One key feature that the game will provide is a “choose your own path” story progression. Certain decisions will decide different outcomes. There will be multiple endings that can be reached depending on how the player chooses to traverse the world.


# Class Diagram
![image](https://user-images.githubusercontent.com/58012195/166180508-0dda33fe-1c9d-4bed-84d3-53d4bcd5454d.png)

We have 3 main classes: Item, Player and NPC. The "Item" class will be the super class of the "Weapons," "Potions," and "Armor" classes. These will be items the user can pick up and use throughout the game. These items can be stored in the Player's inventory, which is an attribute of the Player class. The "Weapons," "Potions," and "Armor" will contain the attributes for each respective item. 

Additionally,  the "Player" class will have the attributes and functions, "name," "stats," and setter and getter functions for all of the stat values. The purpose of the "Player" class and its subclasses is to keep track of a character's attributes. A user will select their character at the start of the game. The player will extend to the subclasses of "Mage", "Warrior", "Healer", and "Assassian". These specific classes will have unique special powers. 

Finally we have the NPC class which extends "Friend" and "Enemy" which both are characters the player will encounter. They will have an array of items stored which will dropped when they are defeated. 
 
 
# Design Pattern 
We are using a composite design pattern for our project to implement the Display class. The display is our interface that all of the data will be shown to the player/ client. Using a composite pattern will make it easier to connect the display with the backend functions/composite parts of our game. 


# Updated Class Diagram
![CS100 Final](https://user-images.githubusercontent.com/59896479/171794902-f5b1f171-2d6a-47a6-a7d1-231c4d4f3e1a.jpeg)
All of the text that is included in red shows revisions and changes that we have made compared to our original class diagram. This class diagram also showcases our design pattern explained above.


# How to Use
To play our wonderful game, you need to follow a few steps. All you need to do is to clone this repository and create an executable file to run the game. To do so, run "cmake3 ." then afterwards run "make". Then after you run these two and they compile, reun the command, "./display". Once the game is loaded, there will be instructions and a tutorial provided if needed to play the game.

To run the unit tests, run the executable ./test.  
 
Here are a few screenshots of what the game should look like:

Start Scene Screen:

<img width="309" alt="Screen Shot 2022-06-03 at 1 49 20 PM" src="https://user-images.githubusercontent.com/59896479/171950881-8c6e981e-f7b2-4cce-8180-93502db86c9f.png">

Upgrade Weapon or Armor Scene Screen - Interaction with an NPC:

<img width="887" alt="Screen Shot 2022-06-03 at 1 51 01 PM" src="https://user-images.githubusercontent.com/59896479/171950985-ddf33a8e-be6a-4bd4-91de-225368800bf0.png">


Fight Scene Screen:

<img width="1019" alt="Screen Shot 2022-06-03 at 1 52 01 PM" src="https://user-images.githubusercontent.com/59896479/171951021-574055f2-8fdf-4525-b3da-74fdd5458037.png">

End Scene Screen:

<img width="1329" alt="Screen Shot 2022-06-03 at 1 52 47 PM" src="https://user-images.githubusercontent.com/59896479/171951062-6a725dc3-11ed-4a08-aa40-503712c95655.png">

# Testing Process
We tested and validated our project by using the googletest submodule and creating unit tests for our functions and dynamically ran the tests as we created more functions. For testing, we went through and tested each class in the project individually. We ensured that each one and all of its functions ran without error. Then we integrated each one into the main body of code and checked it again. Also to ensure we had to outlying errors, we ran Valgrind with full leak checks to find and debug any errors.
