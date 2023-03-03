# Assembly Instructions
There are three phase to this project: building, testing, and experimenting!

### Build
Order and 3D print the parts. On the speed controller board, secure wire leads that will go to the batter holder and the DC motor (see step 3 for better image). ![Assembly picture 1](https://github.com/ajrazander/hardware/blob/main/ion-trap-demo/instructions/photos/assembly_1.png)

1. Place batteries in the battery holder and wiggle into the 3D printed box slot. It should fit snuggly. ![Assembly picture 2](https://github.com/ajrazander/hardware/blob/main/ion-trap-demo/instructions/photos/assembly_2.png)

2. Disconnect the black switch to the speed controller. Pull the outer knob off the potentiometer and take off the washer and nut under the knob. Push the exposed potentiometer knob through the bottom hole. This might need some moderate force and wiggling to get the threads through the hole. Reassemble the knob: put the washer back on; tighten the nut; push the knob back on. ![Assembly picture 3](https://github.com/ajrazander/hardware/blob/main/ion-trap-demo/instructions/photos/assembly_3.png)

3. Attach the speed controller power output to the DC motor. It doesn’t matter which lead is connected to plus or minus on the DC motor. I suggest to use a more secure connection than shown here (such as soldering on the wires). ![Assembly picture 4](https://github.com/ajrazander/hardware/blob/main/ion-trap-demo/instructions/photos/assembly_4.png)

4. Put the DC motor in the cylindrical base. Be sure the vertical 3D printed lines in the cylinder match with the metal groves at the bottom of the DC motor casing. Confirm the fit by wiggling the DC motor. It should not rotate. ![Assembly picture 5](https://github.com/ajrazander/hardware/blob/main/ion-trap-demo/instructions/photos/assembly_5.png)

5. Attach the speed controller switch. Pull the white plug through the front rectangular hole of the 3D printed base. Plug it in to the speed controller. Wiggle and push the black switch into place. It will be a tight fit. ![Assembly picture 6](https://github.com/ajrazander/hardware/blob/main/ion-trap-demo/instructions/photos/assembly_6.png)

6. Wrap up. With the speed controller’s switch off. Attach the battery wire leads to the battery holder. Slip the ping pong ball into the socket.
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
Contains papers I found useful when designing this project as well as the physics this demo is demonstrating. Here are some nice youtube videos demonstrating or explaning the physics in no particular order:
* https://youtu.be/9TH5mFHLmfc
* https://youtu.be/1NBOsELakx4

### Pictures
Pictures of different parts and how they fit together.

Saddle design. The saddle shape can be redesigned and calculated to your liking by using the "saddle-design.nb" notebook. Mathematica allows for a simple equation to stl file export.
