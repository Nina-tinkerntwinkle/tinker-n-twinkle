# Simple Circuit

## Paper Circuit

### Materials needed: 
- 1 LED light
- 1 CR2032 Button Battery
- Copper Tape
- 1 copy of [template](https://raw.githubusercontent.com/Nina-tinkerntwinkle/tinker-n-twinkle/main/assets/files/simple_circuit_template.pdf)

### Instructions: 
**<ins>Step 1:</ins>** Lay the copper tape down, following the drawn out path on the template. 

**<ins>Step 2:</ins>** Fold the legs of the LED, place it on the indicated spot in the template, and use small pieces of copper tape to connect the legs to the path from Step 1. An LED has an **anode** and **cathode**. The anode is the positive side and indicates the longer leg, while the cathod is negative side and indicates the shorter leg. Make sure that your LED is lined up so that the anode points towards the + and the cathode points towards the -. 

**<ins>Step 3:</ins>** Place the button battery at the indicated spot with the negative side facing down and fold the flap switch corner. The LED should light up when the flap comes into contact with the battery. If you want the light to stay on, use a binder clip to hold the flap in place. 


## PHET Simulation: 

Now, we're going to build this circuit in a simulator. Open the [PHET DC Circuit Simulator](https://phet.colorado.edu/sims/html/circuit-construction-kit-dc-virtual-lab/latest/circuit-construction-kit-dc-virtual-lab_all.html) to create the simulation. 

### Instructions: 
**<ins>Step 1:</ins>** Drag in the components: a lightbulb, a battery, and a switch. 

**<ins>Step 2:</ins>** Connect the components using the wire by overlapping the circles so they snap together to match the paper circuit. 

**<ins>Step 3:</ins>** Close the switch to see the lightbulb turn on! 


## TinkerCAD: 

First, create a TinkerCAD account [here](https://www.tinkercad.com/join). Then, create a new circuit project by clicking the blue "Create" button and selecting "Circuits" from the dropdown. 

### Instructions: 
**<ins>Step 1:</ins>** Let's start by recreating the simple circuit in TinkerCAD. Drag in the components labeled "LED" and "Coin Cell 3V Battery". 

**<ins>Step 2:</ins>** Draw connections from the anode of the LED to the positive side and the cathode to the negative side. To create a wire connection, click one side of the connection and then the other (to create a turn in the wire, click once with your mouse). 

**<ins>Step 3:</ins>** Select the "Start Simulation" button in the top right corner to see the LED light up. 

**<ins>Step 4:</ins>** Now, let's add a switch to our circuit. Drag in the pushbutton component. Delete the current connection between the anode and battery. 

**<ins>Step 5:</ins>** Connect the leg of the LED to Terminal 1 (a or b) and the positive end of the battery to Terminal 2 (a or b). Select the "Start Simulation" button in the top right corner and press the pushbutton to see the LED light up. 

**<ins>Step 6:</ins>** You'll notice that there's a warning symbol next to the LED saying that the current through the LED is much higher than the recommended maximum. To fix this, we will need to add a resistor in the circuit. Drag in a resister from the component bank and set it to 100 ohms. 

**<ins>Step 7:</ins>** Delete one of the connections currently in the circuit and reconnect it with the resistor in the path of the circuit. Run the simulation to see if the warning symbol disappears. 

**Now that you've built a simple circuit, it's time to transfer it onto an Arduino microcontroller! Please read this for an introduction to Arduinos and their functions.**

First, drag an Arduino (Arduino Uno R3), a breadboard, an LED, a resistor (set to 100 ohms), and a pushbutton into the workspace. 

Notice that you don't need a battery. In this case, the Arduino is acting as the power source. The "negative" is represented by the "GND" pin, and the "positive" is represented by the other pins lining the sides of the Arduino. Additionally, the breadboard has internal connections, as shown in the diagram below: 

(insert diagram)

We will use these to help us build the circuit. First, try to translate your circuit to the Arduino and breadboard setup yourself. Make sure to use the GND & 13 pins. Then, check your circuit against the circuit below. 

(insert circuit diagram)

Because Arduino is a microcontroller, you need to add some code to control the settings of the pins. This circuit contains an external switch (the pushbutton), which means that the Arduino should be constantly supplying power to the circuit. Click the "Code" button in the top right and use the blocks to write this piece of code: 

(insert code) 

Select the "Start Simulation" button in the top right corner and press the pushbutton to watch the LED light up! 

Now that you've learned all about creating a simple circuit, it's time to move on to the next project: a traffic light! 
