#  Project
Ghostbusters

## Description
Let's make our first game, where we will catch some ghosts.

## Topics Covered

* Pauses between events, actions and loop (wait)
* Random
* Variables
* Getting interactive with our programs

## Notes
* This project is based on Ghostbusters Project in [Code Club - Scratch Module 1](https://projects.raspberrypi.org/en/codeclub/scratch-module-1)
* This project can be completed by either following the instructions in the link above, or by following the instructions below
* The file "Ghostbusters 1.sb3" is the basic version of this project & does not include code for the Challenges listed at the end
* The file "Ghostbusters 2.sb3" is an alternate version which includes code for the Challenges listed at the end

## Instructions
1. Start a new Scratch Project
2. Name it Ghostbusters and save it
3. Delete the default Sprite
4. Add a ghost Sprite
5. Add a spooky backgdrop 
6. Add a ghost Sprite
7. Challenge: Add code so the ghost appears and disapears forever when the green flag is clicked
    * Challenge Solution:
        1. Events > `When flag clicked`
        2. Control > `forever` loop
        3. Put inside your forever loop
            1. Looks > `hide`
            2. Control > `wait 1 seconds`
            3. Looks > `show`
            4. Control > `wait 1 seconds`
        4. Save and test your code
8. Now, let's we make our ghost appear in random positions instead of always staying in the same place. Add this code before the `show` block in your forever loop:
    1. Motion > `go to "random position"` 
    2. Save and test your code.
9. Challenge: 
    1. Can you make the ghost `wait` a random amount on time while it's hidden?
    2. Can you use the `set size` block to make the ghst randomly get larger and smaller when it appears?
        * Challenge Solution:
            1. Put this in your `wait` block after the `hide` block:
                * Operators > `pick random "1" to "10"`
            2. Change the values of "1" and "10". Experiment with different values.
            3. Above your `show` block add:
                1. Looks > `set size to "100"%`
                2. Put a `pick random "1" to "10"` inside your `set size` block
                3. Change the values of "1" and "10". Experiment with different values. (I used "20" and "100")
10. Now, let's add code so that when you click on the ghost, the ghost disappears because it's been caught:
    1. Control > `when this sprite clicked`
    2. Looks > `hide`
11. Add a sound when the ghost is caught. Try it yourself
    * Hint: there are `play sound` blocks in "Sound"
    * Hint: Change the sound you want to use in the "Sounds" tab
        * Here's my code:
            1. `when this sprite clicked`
            2. `hide`
            3. `play sound "Squish Pop: until done`
12. Now let's add a score to our game. To do this we'll add a variable. Variables are how programs remember information. 
    1. Variables > click "Make a variable"
    2. Name it "score"
    3. Make sure "For all sprites" is clicked & click "OK"
    4. Now we can see the variable "score" shown on the stage
    5. Note: You can hide variables by unticking the checkbox beside them. 
13. Now that we have a score variable, let's make our player score points when we catch the ghost. To do this we need to *change the variable everytime we click the ghost sprite*:
    1. Variables > `change "my variable" by "1"`
    2. Change the value of "my variable" to "score" #it's super important you choose the right variable - otherwise the score variable won't change and you'll get no points!
    3. Test your code. Did you notice the `score` never resets? To reset the score add this to the `when flag clicked` code:
        1. Variable > `set "my variable" to "0"`
        2. Change "my variable" to "score" so you have: `set "score" to "0"`
        3. Try putting this block before and after the forever loop and see what happens. Where is the correct location?
14. Now let's add a timer to our game so it doesn't play forever and ever.

    1. Create a new variable called "time"
    2. Click on the Stage editor and add a `when flag clicked` event block with the following code:
    3. Variables > `set "my variable" to "0"`
    4. Control > `repeat until`
    5. Inside the `reapeat` block add:
        1. Control > `wait "1" seconds`
        2. Variable > `change "my variable" by "1"`
    6. Now change the `time` variable values so that `time` starts at 10 seconds & *counts down* by 1 second at a time
        1. Change the values in the `set "my variable" to "0"` block to: "time" and "10"
        2. Change the values in the `change "my variable" by "1"` block to: "time" and "-1"
    7. Now let's add the controls for the `repeat until` block, so we tell it when to stop repeating.
        1. Get the: Operators > `" " = "50"` block
        2. Put it in the `repeat` blocks value
        3. Get the" Variables > `time` 
        4. Put this in the first value of the Operator block
        5. Change the second value of the Operator block to "0"
            * Your code should now read:
                1. `when flag clicked`
                2. `set "time" to "10"`
                3. `repeat until <"time = "0">`
                4. `wait "1" seconds`
                5. `change "time" by "-1"`
        6. Test your game. Notice the ghost stop doesn't stop appearing and disapearing when the timer reaches 0. To fix that add this block underneath your `repeat until` block:
            1. Control > `stop "all"`
15. Save and test your game. Is your game too easy or too hard? You can change the difficulty by altering:
    1. The time the player has to play the game
    2. The speed the ghost appears and disappears
    3. The size the ghost appears
        * Try different combinations until you are happy with the difficulty
16. Challenge:
    1. Can you add more Sprites to the game?
    2. Can you make each Sprite have a different difficulty level? Eg: some are harder to catch and give more points, while some are easier to catch and give less points 
    3. Can you add a Sprite that makes you loose points?
    4. Can you add an animation/new look when a sprite is caught?
    5. Can you add a game over message when the timer runs out?

Extra Challenges solutions are in the "Ghostbuters 2" file/project

    