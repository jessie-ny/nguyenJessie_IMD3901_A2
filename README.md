# nguyenJessie_IMD3901_A2

1.Overview of what you did (i.e., what are the controls? Why this design?)

I imported an environment from sketchfab. In the environment I created 4 buttons, and 2 types of objects. Users can move around the environment on a desktop with AWSD keys, and can interact with the environment with the ring shaped cursor fixed to the centre of the screen. On mobile, users can drag their finger to move around the environment or allow “motion tracking” and tilt their phones to “look” around the environment. And they can also interact with the environment with the ring shaped cursor fixed to the centre of the screen. 

The environment I imported from sketchfab is a basketball court, and so using the tutorial from class, I created 4 buttons that would:
- Create a ball
- Shoot the ball
- Change the colour of the ball
- And destroy it

I also created 2 types of objects: discs, and blocks. I added animations on the discs to move up and down, and added an opacity animation to some of the discs. When the user interacts with the discs using the cursor, the discs are destroyed. And when the user interacts with the blocks, they rotate.

I wanted to create a design where there were defenders that the user needed to defeat (the discs) and the offence that the user could move/manipulate (the blocks). 

I also used the class code so that the sound would attenuate depending on user distance and direction to sound. Which worked in this environment as the sounds gets quieter as the user moves away from the basketball court. 

2. What was challenging.
Figuring out an efficient way to create all of the cylinders and blocks. I wanted to create multiple objects with the same properties, with varying positions and animations. 

3. What went well (i.e., how did you solve the above challenges?).
I was able to solve the above challenges by utilizing the a-frame component “mixin”. Which allowed me to define a bundle of reusable components. So I created two mixins called “destroyCylinders” and “rotateBlocks” that I could reuse. 

4. Credits:
Environment:
- This work is based on "BasketBall Place" (https://sketchfab.com/3d-models/basketball
place-2ffb5e2a045240e7a9809c3bca74b968) by MouradZzz °<° (https://sketchfab.com/mouradZzz) licensed under CC-BY-4.0 (http://creativecommons.org/licenses/by/4.0/)

Mixins and random-color.js documentation:
- https://aframe.io/docs/1.4.0/guides/building-a-minecraft-demo.html

Music:
- https://soundcloud.com/user-545714970/sets/roundball-rock-aka-the-theme utm_source=clipboard&utm_medium=text&utm_campaign=social_sharing

Cursor documentation:
- https://github.com/aframevr/aframe/blob/master/docs/components/cursor.md

Sound documentation:
- https://github.com/aframevr/aframe/blob/master/docs/components/sound.md

Event-set-component documentation:
- https://glitch.com/~aframe-event-set-component
- https://www.youtube.com/watch?v=RsA5a-gDk4c

Opacity animation documentation:
- https://codepen.io/dansinni/pen/vdvZVb
