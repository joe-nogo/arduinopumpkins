Easy:

This is the complete code with seven different complete light modes defined for you. To begin with, copy and paste this code into your new sketch on the Arduino IDE. Next, look at line 239. This is our loop function which will repeat continuously until the end of times. Inside this function, I have an incomplete for loop. Try entering numbers in for VALUE to create an alternating lighting effect for different durations of time. Here is the general form of the for statement:

for (initialization; condition; iteration) 
{
// 
}

The for loop operates as follows. When the loop first starts, the initialization portion of the loop is executed. Generally, this is an expression that sets the value of the loop control variable, which acts as a counter that controls the loop. It is important to understand that the initialization expression is only executed once. Next, condition is evaluated. This must be a Boolean expression. It usually tests the loop control variable against a target value. If this expression is true, then the body of the loop is executed. If it is false, the loop terminates. Next, the iteration portion of the loop is executed. This is usually an expression that increments or decrements the loop control variable. The loop then iterates, first evaluating the conditional expression, then executing the body of the loop, and then executing the iteration expression with each pass. This process repeats until the controlling expression is false.
Once you've done this, try experimenting with other light modes I have pre-defined for you, and then try to make one of your own using mine as a reference!

Intermediate:

Examine line 203. Here I have defined a function 'RaVeMoDe' which should rapidly cycle between colors repeatedly simulating rave lighting. To create this function, look at the function setPixelColors on line 41 and figure out how it sets the the color of each of the 12 LEDs, then use that to figure out how you should define the initialization and conditional values of a string of for loops. The individual LEDs on the ring are defined from LED 0 to LED 11. To determine the values you should enter in the setPixelColor function inside the for loops, look up how colors are defined using RGB values and try to cycle through the colors of the rainbow: red, orange, yellow, green, blue, and violet. Remember to use the function pixels.show() after you have set the pixel color. If you get stuck, try looking at my other predefined functions as a reference. Once you've done that, try to come up with and create your own lighting effect from scratch!

Hard:

Look at line 82. Here I have defined a function 'Snake' for you to fill out. This function should use the values I have predefined for you in the array 'colarray' in the setup function (colarray begins being defined on line 24). This array contains 36 values for colors in groups of 3: a red, green, and blue value for each of the 12 LEDs in an equal gradient of all colors of the rainbow from red to purple. Try to create a lighting effect using this array that simulates a 'rainbow snake' where the head is red and its tail is purple, and the tail continously chases the head around the LED with an equal gradient from red to purple from head to tail. Make sure to take note of the helper function I have predefined for you 'pixels.setPixelColor()' to make it easier for you to set the color of individual LEDs. Once you have done this, try to come up with and create your own lighting effect from scratch!
