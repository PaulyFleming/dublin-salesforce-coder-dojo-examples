# Lost In Space Project

## Description
We will create an animation of space where there's a lost monkey floating in space, a rocketship flying past the earth and a giant space rock bouncing around.

## Topics Covered

* Loops - repeat loop, forever loop (methods for repeating code)
* Animating Sprites
* Control Blocks
* Can introduce Random here as an addition
* 
* 

## Notes
* This project is based on the Lost In Space Project in [Code Club - Scratch Module 1](https://projects.raspberrypi.org/en/codeclub/scratch-module-1)
* This project can be completed by either following the instructions in the link above, or by following the instructions below
* The file "Lost In Space 1.sb3" is the basic version of this project & does not include code for the Challenges listed at the end
* The file "Lost In Space 2.sb3" is an alternate version which includes code for the Challenges listed at the end

## Instructions
1. Start a new Scratch Project
2. Name it Lost In Space and save it
3. Delete the default Sprite
4. Add the earth and rocketship sprites to the stage
5. Add the stars backdrop
6. Click on the rocketship sprite & click on the costumes tab
7. Rotate the rocketship so it's on it's side
8. Click the code tab & add this code to make the rocketship move:
    1. Events > `When flag clicked`
    2. Motion > `point in direction 90` (Change the default number to "0")
    3. Motion > `go to x: -151 y: -191` (Change the default numbers to "-150" & "-150")
    4. Looks > `say "Hello!" for "2" seconds` (Change the block to say "Let's go" for 2 seconds)
    5. Motion > `point towards "mouse-pointer"` (Change the block to point towards "Earth")
    6. Motion > `glide "1" secs to x: "-151" y: "-91"` (Change the block so x and y read "0" "0")
9. Click the green flag above the stage to test your animation
10. Challenge: 
    1. Can you make the rocketship move more slowly towards the Earth?
    2. Can you make the rocketship move until it touches the Earth?
        * Challenge solution:
            1. Change the value of "glide" to a number higher than 1, eg 2
            2. Swap the `glide to x: y:` code block for the `glide to position` block and change the value of "position" to "Earth"
11. Now let's use a Loop to animate the rocketship. Start by deleting the `glide` block
12. Add a `repeat` block and a `move X steps` block to your code:
    1. Control > `repeat 10 times` (Change the repeat number to "200")
    2. Motion > `move 10 steps` (Change the steps value to "2")
13. Test your code!
14. Now let's change the color of the rocketship as it moves towards Earth. Add this code into your `repeat` loop:
    1. Looks > `change color effect by 25`
15. Test your code!
16. Challenge: Can you make the rocketship get smaller as it travels towards Earth?
    * Solution: 
        1. Add Looks > `set size to "100%"` as the first line of code under `when flag clicked` | NOTE: Try placing this block further down in the code and see what happens. Does it matter where this block is in order to make the animation look right?
        2. Add Looks > ` change size by "10"` as the last line of code in your `repeat` loop (experiment by changing the value of the size parameter to get an animation you like ["-1" works quite well])
17. Add the monkey sprite to the stage
18. Click the monkey sprite and click the costumes tab
19. Change the fill to show the red line and change the outline to a white color by changing the Saturation value to "0"
20. Click the circle tool and draw a space helmet around the monkey's head
21. Challenge: Can you make the monkey spin in a circle forever? 
    * Solution:
        1. Add a `forever` loop to the event `when flag clicked` and add the `turn 15 degrees` Motion block. Experiment with the degrees value. What does this value control in this forever loop?
22. Now lets add the "Rocks" sprite to the stage
23. Challenge: Can you make the rock bounce around the stage?
    * Solution
        1. Events > `when flag clicked`
        2. Motion > `point towards "random position` (CHange value to "Earth")
        3. Control > `forever` loop
        4. Motion > `move "10" steps` inside the forever loop (Change to "2" steps)
        5. Motion > `if on endge bounce` inside the forever loop
24. Add the star sprite to the stage
25. Challenge: Can you make the star repeatedly grow and shrink?
    * Solution: 
        1. Place a `forever` loop in the Event `when flag clicked` on your star sprite
        2. Place 2 `repeat` loops inside the `forver` loop. Change the values to repeat "20" times in each
        3. Place a `change size by 10` Looks block in each `repeat` loop
        4. Change the size in the `repeat` loops to "2" & "-2"
        5. Test your code!

    * Alternate solution to introduce `random`:
        1. Place the `when flag clicked` event block
        2. Place a `set size to "100"%` Looks block
        3. Place a `forever` loop
        4. Place a `change size by "10"` Looks block
        5. Get the Operators block `pick random "1" to "10"` and place it in the number area of the `change size by` block inside your `forever` loop.
        6. Change the values of the `pick random "1" to "10"` block to make the star grow and shrink. ("-5" & "5" is a nice combo)

26. Extra Challenges:
    1. Can you make the rocketship run in a loop so it always moves towards the Earth circles around and moves away from the Earth? The rocketship must get smaller while going towards Earth and get bigger while moving away from the Earth. 
    2. Can you make the rocks change position if they touch the monkey, earth or rocketship?
    3. Can you make the monkey move if the rocks or the rocketship touch it?

Extra Challenges Solutions are in the "Lost In Space 2" file/project



