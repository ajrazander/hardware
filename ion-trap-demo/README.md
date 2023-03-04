# The Trapped Ion
Here's a ping pong ball and spinning saddle to demonstrate how atomic physicists trap individual atoms for study and even quantum computing.

### Parts list. This is what and where I purchased each item (if you find something cheaper let me know).
* Housing. A 3D printed container to hold everything together (see designs/box_v4.stl). (Feb 2023)
* Saddle potential. A 3D printed saddle that "traps" the ping pong ball (see designs/saddle_100xy_50z.stl). (Jan 2023)
* ~600 grit sand paper. You want something fine to smooth the saddle. This will dramatically increase the trapping time. (Jan 2023)
* 12V DC motor (you'll want it geared down to the range of a few hundred RPM). Used to spin the saddle. Review the paper under the literature folder to calculate how much speed you may want. 1Hz (60 RPM) seems to be a golden speed for most saddles. I purchased one [online for $15](https://www.amazon.com/gp/product/B072R5G5GR/ref=ppx_yo_dt_b_asin_title_o08_s00?ie=UTF8&th=1) that's probably too beefy but I like the standing geometry (Jan 2023).
* 12V DC motor speed controller. You could make this yourself if you have access to a basic eletronics. I purchased [these online for $10](https://www.amazon.com/gp/product/B08HQQR3FQ/ref=ppx_yo_dt_b_asin_title_o01_s01?ie=UTF8&psc=1) (Jan 2023)
* 8 AA battery holder. Used to power the DC motor. I bought it [here for $7](https://www.amazon.com/gp/product/B07WP1CYYW/ref=ppx_yo_dt_b_asin_title_o01_s00?ie=UTF8&psc=1) (Jan 2023)
* 8 AA batteries. (Jan 2023)
* Ping pong ball. The ping pong ball is the "atom" in the trap. I used a standard 40mm size ping pong ball and [purchased a few here for $10](https://www.amazon.com/gp/product/B00V57KP1G/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&th=1). (Jan 2023)
* 2 wires. You'll need 2 wires (red and black look cool) to go from the controller to the motor. (Jan 2023)

### Instructions
[Read the instructions](https://github.com/ajrazander/hardware/tree/main/ion-trap-demo/instructions) section for how to assemble the pieces together including some pictures and videos of it working.

### Designs
The designs folder holds the 3D printed components:
1. The saddle which sits on top of the motor shaft.
2. The housing that holds all the components together.
3. The Mathematica file "saddle-design.nb" you can use to export your own custom saddle stl file. (It's suprisingly easy; then use tinkercad to get the DC motor base on the saddle).

### Literature
Contains papers I found useful when designing this project as well as the physics this demo is demonstrating. Here are some nice youtube videos demonstrating or explaning the physics in no particular order:
* https://youtu.be/9TH5mFHLmfc
* https://youtu.be/1NBOsELakx4
