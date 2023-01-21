# The Trapped Ion
Here's a ping pong ball demonstrating how atomic physicists trap individual atoms for study.

### Parts list. Lists each part and where I purchased them (if you find something cheaper let me know).
* Box. A 3D printed container to hold everything together (see designs/box.stl)
* Saddle. A 3D printed saddle that "traps" the ping pong ball (see designs/saddle_100xy_50z.stl).
* ~600 grit sand paper. You want something fine to smooth the saddle. This will dramatically increase the trapping time.
* 12V DC motor (probably want it it geared down to a few hundred RPM). Used to spin the saddle. Review the paper under the literature folder to calculate how much speed you may want. 1Hz (60 RPM) seems to be a golden speed for most saddles. I purchased one [online for $15](https://www.amazon.com/gp/product/B072R5G5GR/ref=ppx_yo_dt_b_asin_title_o08_s00?ie=UTF8&th=1) that's probably too beefy but I like the standing geometry (Jan 2023).
* 12V DC motor speed controller. You could make this yourself if you have access to a basic eletronics shop. I purchased [these online for $10](https://www.amazon.com/gp/product/B08HQQR3FQ/ref=ppx_yo_dt_b_asin_title_o01_s01?ie=UTF8&psc=1) (Jan 2023)
* 8 AA battery holder. Used to power the DC motor. I bought it [here for $7](https://www.amazon.com/gp/product/B07WP1CYYW/ref=ppx_yo_dt_b_asin_title_o01_s00?ie=UTF8&psc=1) (Jan 2023)
* 8 AA batteries.
* Ping pong ball. The ping pong ball is the "atom" in the trap. I used a standard 40mm size ping pong ball and [purchased a few here for $10](https://www.amazon.com/gp/product/B00V57KP1G/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&th=1)
* 2 wires. You'll want 2 wires (red and black look cool) to go from the controller to the motor.

### Instructions
There are three phase to this project (and all projects): building, testing, and then playing!

Build
1. Order parts and 3D print the box and saddle files
2. After printing the saddle, thoroughly sand the center of the saddle surface where the ball will be with ~600 grit sand paper. Remember to wet the sand paper while smoothing the saddle. Once sanded, buff it up with a rag. Repeat until it feels smooth to the touch.
3. Put batteries in battery holder.
4. Attach the battery holder leads to the 12V DC motor controller. If you bought the same one I did, then use a screwdriver to open up the driver slot, put the battery hold lead in, and tighten the slot with the screwdriver.
5. Attach 2 wires to the controller output which will eventually attach to the motor. Use the same method as above.
6. Pull off the knob from the contoller's potentiometer and unscrew the nut. Remove the washer. Slide the controller's potentiometer handle into the hole in the box. Tighten the washer and nut until the controller is held in place. Put the knob back on. 
7. Wiggle the controllers switch into the rectangular hole above the potentiometer's hole. It may be a little loose. You may be tempted to hot or super glue it in place, but don't do that until you're sure everything is working how you want it to.
8. Wire the DC motor. Attach the leads from the controller output to the DC motor leads. It doesn't matter which wire goes to which lead. Attach as you see fit. Soldering is probably the best option. If that's not possible for you, you could get away with taping the wires on with electrical tape.
9. Place the motor on the motor stand in the box. Be sure to line up the motor leads by the open section and align the small metal folds on the bottom of the motor with the short rails in the motor stand. The motor should fit snuggly.
10. Match up the motor shaft with the bottom of the saddle. There's a small flat side to both that needs to be aligned. The saddle should snuggly slide on.

Testing
1. Turn on the dc motor using the controller. Does it spin? Does varying the voltage to the motor with the potentiometer knob work? Can you get to the rotational speed you want/calculated?

Playing
1. Start with the saddle spinning at slow speed. Place the ping pong ball in the center of the spinning saddle.. If it rolls right off, that's what you want at this point. That means the saddle is spinning too slowly.
2. Slowly increase the speed and replace the ping pong ball until it doesn't fall off. Ta-da! It's trapped!
3. Measure how long the ping pong ball stays trapped?

### Designs
The designs folder holds the 3D printed components:
1. The saddle which sits on top of the motor shaft.
2. The box that holds all the components together

### Literature
Contains papers I found useful when designing this project as well as the physics this demo is demonstrating.

### Pictures
Pictures of different parts and how they fit together.

Saddle design. The saddle shape can be redesigned and calculated to your liking by using the "saddle-design.nb" notebook. Mathematica allows for a simple equation to stl file export.
