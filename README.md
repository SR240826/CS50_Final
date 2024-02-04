Project Title: Fill The Reserver

Video Demo: https://youtu.be/S8npqgbP1SY

**About the project**: The project titled "Fill The Reservoir" represents a dynamic and versatile game model showcasing the implementation of algorithms and code structures. It serves as a demonstration of the developer's proficiency in procedural and object-oriented coding. The game revolves around a player-controlled character tasked with collecting water droplets scattered across the environment and returning them to an empty reservoir within a specified time limit.

**Project details**: As mentioned above, the project is a generic game model or more specifically quest. User will control a character to collect waterdrops and return to an empty reserver to refill it within time limit. The elements of the game will keep changing for each reloads. Resizing the window will also result a reload of the game. This project's main focus was the implementation of procedural and object oriented code that can be used in any other project in future or store in a library. This way of coding provides an advantage of getting a boarder range of results. For example, in this project, everytime a new game starts, the position of elements will be changed.. This dynamic nature enhances the replayability of the game, providing users with a unique experience in each session. Additionally, the project's code structure is designed with reusability in mind, allowing developers to easily integrate the algorithms and structures into future projects or store them in a library. It is also possible to use more than one map or quest for games this way where the developers are not required to start from scrach saving a vast amount of time and resources. 

Using object oriented methods in javascript, it was easy to call one function multiple time without defining variables repeatedly. Even though this project is built upon javascript, the rendering is done with HTML canvas. At first I wanted to use pure HTML, but while I was viewing at different functions of javascripts as well as DOM structures, canvas was not so tough to learn. Canvas leverages GPU acceleration, making it well-suited for rendering multiple elements simultaneously, enhancing the overall visual experience. For the loop function in javascript, requestAnimationFrame() method is used which is tricky to use with canvas as well as reloads. There might be memory leak occurance if not used properly with the combination of cancelanimationframe method. On the other hand, as the object positions are changed with each reload of windows, it is required to keep a record of positions with a temporary variable and call the object creation function with those temporary variables inside animation functions. Otherwise each frame will change the position of game elements.

The program  contains player creations, image creations, collition between two object types, movement control, random spawn mechanisms and so on. Instead of producing same result repeatedlt, this procedural and object oriented data structure will keep producing different scenario for the player each time. The model included in ths project contains the bellow features:

1. createPlayer.js: 
    1) The `Player` class consists of 3 core functions and 2 helper functions. The first constructor function create and spawn character to random position inside the canvas boundary. This class consists two update functions one of which is for movement velocity and other is to change position based on coditions such as avoiding obstacles. Developer need to spacify parameters of canvas, canvas context, color, width and height when creating a new character. The core update `function` uses velocity along x and y axis for introducing movement. When using `updatePosition` to change position, the x and y coordinates are needed to be included in this that will immedietly change the position. And the `draw` function is to draw the character over the canvas.


    2) The `Image` class can be used to produce background images or other static objects. It has a `clone` function that will create a clone of the introduced image which helps to change position based on collision. It also as an `update` function to change the position which is not for the movement.

2. keys.js: 
    1) The `keys` class three core functions which control the movement of character. As any other class in javascript, it has constructor function which introduces the keys to use as well as velocity.
    2) the `control(event)` function is used to trigger the key pressed. It was made in such way that a simple keyup function setting to `false` in core javascript script can be used to stop the movement.
    3) The `checkCollision` function is one of the core component that takes an array of obstacle elements and iterate over that array repeatedly to check the distance between character and obstacle elements. It also has collition to the boundary of canvas.

3. canvas_project.js:
    This javascript file contains the whole game structure such as the position, size, events and all game controlable elements. 

**Project usag**e: Click `"A", "D", "W", "S"` to move the character left, right, up and down respectively. Collect all the `water` and bring to `reserver` to fill before time ends!

**Known Issues**: 
1. The obstacles (trees/stones) bounding box has an area of rectangular shape that exceeds its thinner parts. Thus those part collide with player before reaching those obstacles.
2. The waterdrops sometime spawn upon unreachable obstacles. In that case the page needs to be refreshed.
3. If the character collide from top or down of obstacle, the movement along x axis might get slowed or stuck. Try moving oposite of collision.

"Fill The Reservoir" is not just a game; it's a comprehensive showcase of coding expertise, offering an enjoyable and dynamic gaming experience for users while providing a solid foundation for future projects and endeavors.
