# The Trapped Ion
How do you trap one atom? Wolfgang Paul was awarded the Nobel Prize for one strategy which is now called the Paul trap. Here, you'll demonstrate it with a ping pong ball for the ion (a charged atom) and a spinning saddle for the oscillating voltages.

![Spinning saddle trapped a ping pong ball](https://github.com/ajrazander/hardware/blob/main/ion-trap-demo/instructions/videos/trapped_ion_test.gif)

### Parts list
This is what and where I purchased each item (if you find something cheaper let me know).
* Housing. A 3D printed container to hold everything together (see designs/box_v4.stl). (Feb 2023)
* Saddle potential. A 3D printed saddle that "traps" the ping pong ball (see designs/saddle_100xy_50z.stl). (Jan 2023)
* ~600 grit sand paper. You want something fine to smooth the saddle. This will dramatically increase the trapping time. (Jan 2023)
* 12V DC motor (you'll want it geared down to the range of a few hundred RPM). Used to spin the saddle. Review the paper under the literature folder to calculate how much speed you may want. 1Hz (60 RPM) seems to be a golden speed for most saddles. I purchased one [online for $15](https://www.amazon.com/gp/product/B072R5G5GR/ref=ppx_yo_dt_b_asin_title_o08_s00?ie=UTF8&th=1) that's probably too beefy but I like the standing geometry (Jan 2023).
* 12V DC motor speed controller. You could make this yourself if you have access to a basic eletronics. I purchased [these online for $10](https://www.amazon.com/gp/product/B08HQQR3FQ/ref=ppx_yo_dt_b_asin_title_o01_s01?ie=UTF8&psc=1) (Jan 2023)
* 8 AA battery holder. Used to power the DC motor. I bought it [here for $7](https://www.amazon.com/gp/product/B07WP1CYYW/ref=ppx_yo_dt_b_asin_title_o01_s00?ie=UTF8&psc=1) (Jan 2023)
* 8 AA batteries. (Jan 2023)
* Ping pong ball. The ping pong ball is the "atom" in the trap. I used a standard 40mm size ping pong ball and [purchased a few here for $10](https://www.amazon.com/gp/product/B00V57KP1G/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&th=1). (Jan 2023)
* 2 wires. You'll need 2 wires (red and black look cool) to go from the controller to the motor. (Jan 2023)

### Designs
The designs folder holds the 3D printed components which you will need to print:
1. The saddle which sits on top of the motor shaft.
2. The housing that holds all the components together.
The Mathematica file "saddle-design.nb" allows you to export your own custom saddle stl file. (It's suprisingly easy; then use tinkercad to get the DC motor attachment shaft on the saddle).

### Literature
Contains papers I found useful when designing this project as well as the physics this demo is demonstrating. Here are some nice youtube videos demonstrating or explaning the physics in no particular order:
* https://youtu.be/9TH5mFHLmfc
* https://youtu.be/1NBOsELakx4

# Instructions
There are two phase to this project: assembly and experimenting!

### Assembly
Order and 3D print the parts. On the speed controller PCB board, secure wire leads that will go to the battery holder and the DC motor (see step 3 for better image).

<img src="https://github.com/ajrazander/hardware/blob/main/ion-trap-demo/instructions/photos/assembly_1.png" width="400">

1. Place batteries in the battery holder and wiggle it into its slot on the 3D printed housing. It should fit snuggly.

<img src="https://github.com/ajrazander/hardware/blob/main/ion-trap-demo/instructions/photos/assembly_2.png" width="400">

2. Attach the speed controller board to the 3D printed housing. Disconnect the speed controller’s black switch. Pull the outer knob off the potentiometer and take off the washer and nut under the knob. Push the exposed potentiometer knob through the bottom hole of the 3D printed housing (see image below). This might need some moderate force and wiggling to get the threads through the hole. Reassemble the knob: put the washer back on, tighten the nut, and push the knob back on.

<img src="https://github.com/ajrazander/hardware/blob/main/ion-trap-demo/instructions/photos/assembly_3.png" width="400">

3. Attach the speed controller power output to the DC motor. It doesn’t matter which lead from the speed controller is connected to the plus or minus lead of the DC motor. Definitely use a more secure connection than shown here (such as soldering on the wires).

<img src="https://github.com/ajrazander/hardware/blob/main/ion-trap-demo/instructions/photos/assembly_4.png" width="400">

4. Put the DC motor in the cylindrical base. Be sure the 3D printed parallel rails in the cylinder match with the metal groves at the bottom of the DC motor casing. This stabilizers the motor’s rotation. Confirm the fit by wiggling the DC motor. It should not rotate.

<img src="https://github.com/ajrazander/hardware/blob/main/ion-trap-demo/instructions/photos/assembly_5.png" width="400">

5. Attach the speed controller switch. Push the white plug from the front rectangular hole of the 3D printed housing to inside the housing by the speed controller. Plug it in to the speed controller. Carefully wiggle and push the black switch into place. It will be a tight fit.

<img src="https://github.com/ajrazander/hardware/blob/main/ion-trap-demo/instructions/photos/assembly_6.png" width="400">

6. Wrap up. With the speed controller’s switch off. Attach the battery wire leads to the battery holder. Slip the ping pong ball into the socket. Find the flat side of the DC motor shaft and the flat side of the 3D printed saddle’s base and push the saddle on. This might need a bit of force, but should slide on nicely.

Extra. **You will need to smooth the 3D printed saddle to get good trapped times** (~ minutes of trapping are possible with very smooth saddles). Read more about this under Experimenting point 3.

###  Experimenting
1. Test the DC motor is working as expected. Turn on the dc motor using the controller (without the saddle on the DC motor shaft). Does the DC motor shaft spin? Is the DC motor stable in the cylindrical base? Does varying the speed controller’s potentiometer knob affect the DC motor’s speed? Can you get to the rotational speed you want/calculated for the saddle shape you 3D printed? Troubleshoot accordingly ;).

2. Measure the affect of the saddle’s speed on the trapping time. Start with the saddle spinning at slow speed. Place the ping pong ball in the center of the spinning saddle. If it rolls off, try increasing the speed. If the saddle looks like its flinging the ping pong ball off, try decreasing the speed. Measure the saddle rotation speed and the trapping time. Make a plot.

3. Measure the affect of friction on the trapping time. Measure how long you can keep the ping pong ball trapped in the saddle with different smoothness. Without smoothing the 3D printed saddle, I get about ~10 seconds. After 15 minutes of moderately sanding with wet 600 grit sand paper, I get ~30 seconds. With another 15 minutes of more aggressive sanding (wet sand paper and buff it with a rag so I can’t feel any bumps with my fingers), I can get 60 seconds. Doing more smoothing and adding a dry lubricant (such as non-stick Teflon spray), I’ve seen 10 minutes of continuous trapping.

3. How does the initial condition of the ping pong ball affect the trapping time? Try comparing on-center with off-center starting positions. Try placing the ball in the saddle vs giving the ball a little spin. Try spinning the ping pong ball with vs against the saddle direction. What happens? 

4. Try different balls and saddle shapes! (See designs folder for the Mathematica notebook that can export new saddle stl files)

5. And of course, what’s the longest trapping time you can get and what helped the ball stay trapped for so long?
