# Rock Band Project

## Topics Covered

* Sprites (objects we can program)
* Backdrops 
* Extensions (these are like libraries in programming languages)
* Events (code to program/control when things will happen, kinda like triggers)
* Sounds
* Basic Animation (changing the look of Sprites when doing certain events)

## Notes
* This project is based on Rock Band Project in [Code Club - Scratch Module 1](https://projects.raspberrypi.org/en/codeclub/scratch-module-1)
* This project can be completed by either following the instructions in the link above, or by following the instructions below
* The file "Rock Band 1.sb3" is the basic version of this project & does not include code for the Challenges listed at the end
* The file "Rock Band 2.sb3" is an alternate version which includes code for the Challenges listed at the end

## Instructions

1. Start a new project
2. Delete default Sprite
3. Add a Sprite for a drum/instrument
4. Add a backdrop
5. Add the Music Extension
6. Click the drum sprite
7. Add the following code (make sure all blocks are connected together like Lego): 
    1. Events > `when this sprite clicked`
    2. Music > `play drum (1) Snare Drum for 0.25 beats`
8. Try different sounds by changing the sound of your drum in the dropdown list of the second line of code you just added
9. Add code to play a second sound when pressing a key:
    1. Events > `when space key is pressed`
    2. Music > `play drum (1) Snare Drum for 0.25 beats` | or right click on this line of code in the "when this sprite clicked: code block and click on "duplicate"
    3. Change the sound to be different from your first code block
    4. Try playing a beat now that you have 2 sounds with different Event triggers
10. Add a new Sprite and choose the singer
11. Click the Singer Sprite
12. Click the Sounds tab (delete the default sound if one appears)
13. Click Choose A Sound
14. Select Voices and choose a sound
15. Click the Code tab
16. Add code to make the singer sing when clicked:
    1. Events > `when this sprite clicked`
    2. Sounds > `play sound X until done` (X is the sound you choose above)
17. Click the singer in the stage to test
18. Click the Costumes tab
19. Right click the singer and duplicate
20. Click the new costume and draw some lines to indicate the singer is singing
21. Rename the costumes to `singing` and `not singing`
22. Click the Code Tab
23. Add code to animate singer Sprite when clicked:
    1. Above the `play sound X until done` block add: Looks > `switch costume to singing` 
    2. Below the `play sound X until done` block add: Looks > `switch costume to singing` 
    3. Change the 4th code block to `switch costume to not singing`
24. Repeat above steps to make the drums costume change when playing and not playing
25. Challenges: Improve The Band. Try the following:
    * Add more instruments to the project
    * Record your own sound(s) for Sprites to use | needs a mic
    * Create/paint your own Sprite(s)/Backdrop
    * Animate the backdrop so it changes
    * Make two Sprites play their sounds at the same time
    * Make one event that plays each Sprite's sounds, but plays them one after the other


