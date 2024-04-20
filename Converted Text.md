**IE201**

**INTERMEDIATE PROGRAMMING**

**Project Part 1**

**“Paradise Shooting”**

**Instructor: Ali Tamer Ãœnal**

**Date: 05.4.2024**

 ****

**GROUP-7**

**Metehan YalÃ§Ä±n ([2018402042](tel:2018402042))**

**Yusuf Eren Bayhan ([2022402255](tel:2022402255))**

**Yunus Emre GÃ¼neÅŸ ([2022402267](tel:2022402267))**

**Table of Contents**

1. **Brief Description of the Game**
2. **Explanation of Classes**
3. **Class Diagram/Relationships Among Classes**
4. **General Use Case Diagram and Explanations of the Use Cases**

**1. A brief description of the game**

We are planning to work on a basic tower defense game. 

There will be a main character on a base whose location is predetermined. The main character’s duty will be to protect the base from the surrounding creatures that spawn randomly. 

The creatures will have a certain amount of hp and speed. There will be two types of creatures that are called “giant” and “dwarf”. The giant’s HP and damage will be high but its speed will be low. The dwarf’s hp and damage will be low, however their speed will be high.

The weapon of the main character will have a certain attack speed and damage. By the time it flies, the creatures will get stronger, and their hp, damage, and speed increase. By destroying the creatures, the player will gain some kind of resource such as gold and it will let them upgrade their weapon.

There is no win condition. The goal is to survive as long as possible. There will be a timer that shows past time, and the ending time will be the player’s score.

**2. Explanations of the classes**

**2.1 Game**

This class manages the whole game dynamics. It includes the time past, the game progression, and the player’s shooting at creatures.

**2.2 Hero**

Our hero has a weapon that he uses to shoot at creatures. As time passes, he can improve his attack speed and weapon.

**2.3 Base**

The base has a health point (hp) which creatures try to reach and kill. 

**2.4 Weapon**

Weapon class includes the weapons our hero uses. It can be upgraded and its damage gets higher.

**2.5 Creatures**

These are the mobs that run towards our base. They try to reach us and ruin the base.

**2.5.a. Dwarf**

This is one of the types of the creatures. It has a higher speed but a lower damage and hp.

**2.5.b. Giant**

This is another type of creature. It has a lower speed but a higher damage and hp. Its main duty is to protect other faster creatures.

**3. Class Diagram and Relationships Among Classes**

(/assets/images/class_diagram.png "class diagram")

**The game** class has an aggregation relationship with the **Hero** and **Creature** classes. 

**Hero** class has an aggregation relationship with **Base** and **Weapon** classes with a likewise reasoning.

**Giant** and **Dwarf** classes have an inheritance relationship with the **Creatures** class since they are special types of the **Creatures** class.

**The Creature** class has a relation with the **Base** class because creatures like dwarfs and giants try to reach the base and kill it

**The Creature** class has a relation with the **Weapon** class because the weapon our hero uses will shoot at them.

**4. General Use Case Diagram and Explanations of the Use Cases**

**Start:** The player presses the “start button” on the starting screen and the game starts. 

**Pause/Resume:** The player presses “P” and pauses/resumes the game. By pausing, the game stops, and by resuming, the game continues.

**Exit:** Exit use case is triggered when the player clicks the quit button.

**Tick:** The tick use case controls the frame rate of the game. This use case helps functions to operate timely by including the time dimension (dt) in the game.

**Upgrade:** The user presses the key “W” to trigger an upgrade use case for weapons which results in a damage increase.

               

![](blob:https://gdoc2md.com/d3fe4456-4794-497d-8801-81ebe8c420d4)![](blob:https://gdoc2md.com/07dc342b-345c-4093-940e-70af93c55f32)
