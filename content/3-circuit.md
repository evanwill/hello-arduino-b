---
title: Blink an LED
nav: Blink
gallery: true
topics: Circuit; LED; Output Pins
description: Building on our `Blink` skillz, lets build a LED circuit and control it with UNO!
---

For this project you will need a breadboard, some jumper wires, a 220 *or* 330 ohm resistor, and an LED. 

{% include gallery-figure.html alt="led" img="led1.jpg" %}

{% capture led %}
*Know your LED:* the longer leg is the `anode` and connects to positive voltage, i.e. `+` or `5V`; the short leg is the `cathode` and connects to ground, i.e. `-` or `GND`.  

*Know your Resistor:* resistors are marked by color bands, but they are often hard to read - you can check them with a [multimeter](https://learn.sparkfun.com/tutorials/how-to-use-a-multimeter).
{% endcapture %}{% include card.html text=led %}

## First Circuit

1. Gently push the legs of your LED into two different rows on the breadboard. Remember which one is the long leg! 
    {% include gallery-figure.html alt="LED legs added to breadboard rows 5 and 7" img="led2.jpg" %}
2. Connect the LED `cathode` (short leg) to `GND` by inserting the legs of a 220 ohm resistor into the row and the `-` Rail. 
    {% include gallery-figure.html alt="220 ohm resistor added to breadboard connecting LED cathode to GND rail" img="led3.jpg" %}
3. Connect the LED `anode` (long leg) to `5V` by inserting a jumper wire into the row and the `+` Rail.
    {% include gallery-figure.html alt="Jumper wire added to breadboard connecting LED anode to 5V rail" img="led4.jpg" %}

4. Connect the breadboard to the UNO's power supply: 
- use a red jumper wire to connect the `+` rail to the pin labeled `5V` on the UNO. 
- use a black jumper wire to connect the `-` rail to any pin labeled `GND` on the UNO (you have 3 choices). 

    {% include gallery-figure.html alt="jumper wires added to connect 5V and GND on the breadboard to UNO" img="led5.jpg" %} 

    {% include gallery-figure.html alt="side view showing the GND and 5V pins on UNO" img="led6.jpg" %}

5. Plug your UNO into your USB cable. 

You should now have a beautiful glowing LED!

## Blink it! 

This circuit is drawing power from UNO, but it is not controlled by it. 
We need to connect the LED to a pin so we can start blinking!
First, unplug the UNO from the USB--never modify your circuit while connected to power!

1. Unplug the wire connecting the `anode` from the `+` rail. 

2. Connect the `anode` wire to pin `10` on the UNO. 

    {% include gallery-figure.html alt="jumper wire connecting LED anode to pin 10 on UNO" img="led7.jpg" %} 

    {% include gallery-figure.html alt="side view showing pin 10 on UNO" img="led8.jpg" %}

3. On the IDE `Blink` sketch, replace `LED_BUILTIN` with `10`. The basic code should look like:

   ```
   void setup() {
       pinMode(10, OUTPUT);
   }

   void loop() {
       digitalWrite(10, HIGH);
       delay(1000);
       digitalWrite(10, LOW);
       delay(1000);
   }
   ```

4. Plug UNO into the USB, and click the upload arrow to load the sketch.

You should now have a beautiful **blinking** LED! 

## Extra Credit

The best way to learn is by *messing around*!
Try altering your code and circuit.
Remember: it is hard to *break* UNO!

- make an interesting pattern blinking both the LED and LED_BUILTIN.
- add another LED and make them blink together.
