# Super-Oiram

Super Oiram is a personal project I worked on to refine my skills in creating a level editor and 2D position physics in Unity. The release build contains 4 playable levels, all dynamically loaded at runtime using the bitmap level editor I created.

# Features

## Physics

- Rectangle collision algorithm
- Dynamically sized chunking algorithm to optimize collision checks
- Collisions know which side of a block it occured on

![image](https://user-images.githubusercontent.com/54965702/111892860-029bd480-89cd-11eb-9aeb-903677c7928c.png)

## Bitmap Level Editor

- Levels are dynamically loaded in by reading each pixel on an image. Pixel color determines the block or entity placed.
- Color dictionary allowing any number of new blocks/enemies to be added simply by matching a color hex code to a desired name
- Camera automatically adheres to the level bounds and follows player approrpriately regardless of level size

### Level 4 map
 
![image](https://user-images.githubusercontent.com/54965702/111892880-3a0a8100-89cd-11eb-9c78-a6b166f67553.png)

### Level 4 in game

![image](https://user-images.githubusercontent.com/54965702/111892897-5f978a80-89cd-11eb-93dd-7f2f98cd8199.png)

## State Management

- Finite state machine logic controls player and enemy behavior in game
- Multi layer state abstraction creates reusable states and state components
- Class based state pattern is highly modular and allows for new states to be added in easily
