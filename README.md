Project Title: Fill The Reserver

Video Demo: https://youtu.be/S8npqgbP1SY

**About the project**: The project is a generic game model where player collect objects from environment and return to a destination to complete the quest. This is not a full fledged game, rather a demonstration of the my understanding of using algorithom and implementation of code. Click here to view the project.

**Project details**: As mentioned above, the project is a generic game model or more specifically quest. User will control a character to collect waterdrops and return to an empty reserver to refill it within time limit. The elements of the game will keep changing for each reloads. Resizing the window will also result a reload of the game. This project's main focus was the implementation of procedural and object oriented code that can be used in any other project in future or store in a library. This way of coding provides an advantage of getting a boarder range of results. For example, in this project, everytime a new game starts, the position of elements will be changed. It is also possible to use more than one map or quest for games this way where the developers are not required to start from scrach saving a vast amount of time and resources.

**Project usag**e: Click `"A", "D", "W", "S"` to move the character left, right, up and down respectively. Collect all the `water` and bring to `reserver` to fill before time ends!

**Known Issues**: 
1. The obstacles (trees/stones) bounding box has an area of rectangular shape that exceeds its thinner parts. Thus those part collide with player before reaching those obstacles.
2. The waterdrops sometime spawn upon unreachable obstacles. In that case the page needs to be refreshed.
3. If the character collide from top or down of obstacle, the movement along x axis might get slowed or stuck. Try moving oposite of collision.
