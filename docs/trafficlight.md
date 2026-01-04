# Traffic Light

## Paper Circuit

### Materials needed: 
- 3 LED Lights (red, yellow, green)
- 1 CR2032 Button Battery
- Copper Tape
- 1 copy of [template](https://raw.githubusercontent.com/Nina-tinkerntwinkle/tinker-n-twinkle/main/assets/files/traffic_light_template.pdf)

### Instructions: 
**<ins>Step 1:</ins>** Lay the copper tape down, following the drawn out path on the template.

**<ins>Step 2:</ins>** Fold the legs of the LED, place it on the indicated spot in the template, making sure that the positive and negative legs are facing the right directions. Use small pieces of copper tape to connect the legs to the path from Step 1. Repeat for all 3 lights.

**<ins>Step 3:</ins>** Place the button battery at the indicated spot with the negative side facing down and fold the flap switch corner. The LED should light up when the flap comes into contact with the battery. If you want the light to stay on, use a binder clip to hold the flap in place.

## TinkerCAD: 

**<ins>Step 1:</ins>** Drag an Arduino (Arduino Uno R3), a breadboard, 3 LEDs, and 3 pushbuttons into the workspace. To change the color of the LED, click on the LED in the workspace and select a different color from the dropdown in the top right corner. 

**<ins>Step 2:</ins>** Create three circuits in parallel to match the traffic light template (diagram below), connecting the power and ground rails on the breadboard to the GND and 13 pins on the Arduino (just like the simple circuit). 

(insert diagram) 

**<ins>Step 3:</ins>** Recreate the code from the simple circuit as shown below. This will make sure the Arduino is always supplying power. 

(insert code)

**<ins>Step 3:</ins>** Run the simulation and press the pushbuttons one at a time to see the different lights light up! 

You'll notice that a warning symbol appears when a light turns on that says that the current through the LED is much higher than the recommended maximum. To fix this, let's add a resistor in each path. 

**<ins>Step 4:</ins>** Drag in 3 resistors and set them to 100 ohms each. Place them on the breadboard in the path of each LED. Run the simulation again and press the pushbuttons. The warning symbol shouldn't appear this time. 

(insert diagram)
