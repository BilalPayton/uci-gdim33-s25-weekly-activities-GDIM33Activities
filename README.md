# GDIM 33 In-Class Activities
## W1
### Activity 1
[Inspiration Board](https://www.pinterest.com/theesilliest010/gdim-33-inspiration-board/)

1. In my inspiration sources I'm noticing that I have a lot of images relating to god-like entities
and spaces beyond the physical world aesthetics because of my favorite game being Terraria Calamity.
However because I already have a game I want to make in mind, I searched for a bunch of silly images
to give me scenario ideas for when I start making it.

2. My tablemate Alejandra is looking to build a horror game which I found intriguing because I'm taking
a Horror in Gaming class and also have recently been getting into horror games myself.

3. One of the LA's Angel talked about how he liked soulslike games which I related to because I like
playing games that are difficult and give me a challenge to overcome.


### Activity 2
<img width="1527" height="1147" alt="Screenshot 2026-04-01 193412" src="https://github.com/user-attachments/assets/efad88cf-da37-4cd7-86fe-e2b22ebb98f1" />



## W3
### Activity 1
<img width="1531" height="1143" alt="Screenshot 2026-04-15 175402" src="https://github.com/user-attachments/assets/7d5b7e77-8370-452f-8555-3800ac5d0e44" />


### Activity 2
1. It is advantageous to save the event name clickNpcEventName for the explore-to-dialogue state transitions as Scene variable
because it allows us to use and reference it throughout other Script Graphs as it is essentially a public variable, otherwise we
would not have been able to trigger the event.

2. I used a Debug.Log Node to help check if the custom event to start the Dialogue state worked. To do this, I made
it so that if the custom event triggered like it was supposed to, the Debug Log would print "Trigger Event" to the console.
While testing my code, "Trigger Event" wasn't being sent to the console when running the game and it helped me eventually solve this problem
to make sure everything worked for sure.

3. The Set Cursor Lock State could possibly be relevant in my Vertical Slice if I were to add a scenario where
the cursor needs to not be locked for the player to click on something to not lose the game, and then the cursor
would lock after they passed the scenario.

4. The concept of a game state might be relevant to my Vertical Slice. Originally I thought I would have different
states for different rounds of the game and the farther rounds would add more scenarios, but I now realize that
I don't need states to implement it. I think a better application for states would be to make a state where the game
is running and spawning scenarios and another state where scenarios stop spaawning for a brief people of time to give
the player a break after a round ends. These are also both situations that cannot run at the same time so using states
would be perfect for this.

## W4
### Activity 1
My goal for playtesting today will be to see if the gameplay is fun and not too difficult.

Right now my core mechanics of pressing keyboard keys and reacting quickly because of the timer
are in the game.

Playtest Team Members: Alejandra, Kai, Laura

Playest Notes:
- At first my playtesters struggled with the controls, but eventually got used to them
- Playtesters said the gameplay was fun
- Playtesters think the difficulty is fine so far

### Activity 2
1. A writer could add more dialogue to this setup without writing any code because the for each loop
allows every line and reply to be accessed and displayed in the game.

2. There is no limit to the number of dialogue nodes that the writer could create without writing any code.

3. The purpose of the "Regenerate Nodes" button is to be able to store information about new Node types from
your created code and allow for them to be displayed as Visual Scipting Nodes in Graphs.

## W5
### Activity 1
ScriptableObject Implementation - Items:

Discrete:
1. Create a ScriptableObject for ItemData
2. Create an Item C# Script
3. Give Player an Inventory list of ItemData ScriptableObjects
4. Store ItemData in Player Inventory when needed
5. Remove ItemData from Player Inventory if used

Detailed:
1. Create a ScriptableObject C# script to store ItemData. Test by creating a few objects and tuning them in the inspector.
2. Create a Item C# Script to store ItemData that also has child classes to easily implement Items (Inheritance & Polymorphism). Test by making a few child classes of the Item Script and making them do different things.
3. Attach Item Scripts to respective GameObjects for Items. Ex. extra life child script attached to extra life GameObject. Test by tuning ItemData ScriptableObject to match the intended Item description/function.
4. Add a collider to Items so the player can click them. Test by using OnMouseClick() method in the Items’ script if it can be clicked.
5. When an Item is clicked, add the Item’s ItemData to the Player’s inventory of ItemData ScriptableObjects. Test by printing the inventory contents to the console using Debug.Log() to check if the Item’s data is present.
6. When the player uses an Item, remove the respective Item’s ItemData from the Player’s inventory. Test by printing the inventory contents to the console using Debug.Log() to check if the used Item’s data is removed.

### Activity 2
What I accomplished in class today is that I create the ScriptableObject C# Script ItemData
and created two potential Items that I could add and tune them in the inspector.
For example, I create an ItemData ScriptableObject called Time Extender and gave it a description
that it extends the time for players to react to scenarios, or the Extra Life Item that allows the Player
to make one mistake and continue the game instead of the game automatically ending.