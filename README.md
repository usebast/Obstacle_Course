# The Game Of Obstacles
C# with Unity Learning Game

Small demo game built in C# and Unity with Visual Studio Code

Basically I wrote C# scripts to controll functionality of 
-the Player, 
-the cinemachine camera behaviour (with camera following the Player behaviour)
-some objects appearing and dropping from mid-air
-handling of collisions with walls and other objects
-setup a scoring system
-setup spinning obstacles

Programming learning landmarks:
-using SerializeField to setup variables accessible in Unity GUI
-using if statements to trigger certain behaviours: 
          * setup an object falling from midait after a certain time
          * count the number of first collisions the walls and obstacles have with the Player
          * trigger a colour change on collision
          
-using callbacks by declaring variables and calling them later in the code
          * declare the serialized float x,y,zAngle of the spinners to call them back with the transform.Rotate
          * declare the hits integer variable to call in the Debug.Log to list the number of hits
          * declare the serialized float moveSpeed variable to use in translation of the Player
          * declare the  MeshRenderer and Rigidbody variables to animate the behaviour of the objects dropping from mid-air
          * declare the serialized float timeToWait variable to trigger the objects appearing and falling in the Level

Some rudimentary Game Level Design
-build a small Game Labirinth Arena
-change materials for various objects
-organize objects in prefabs for later re-use
-organize objects in groups: Player, Environment, Obstacles
