---
title: Preparation
nav: Prep
---

{% capture prep %}
**For this workshop you will need:**

- An Arduino UNO and it's USB cable.
- A few basic electronic components, as found in most Arduino starter kits: a breadboard, some jumper wires, a piezo, a 10k ohm resistor, a few 220 or 330 ohm resistors, a photoresistor, and a few LEDs.
- Access to [Arduino IDE Software](https://www.arduino.cc/en/software), either installed on your computer or via the online Web Editor -- see notes below.

{% endcapture %}{% include card.html text=prep %}

Most of this workshop is based on projects from the official [Arduino starter kit](https://store-usa.arduino.cc/products/arduino-starter-kit-multi-language?selectedStore=us).
This means the code examples are built into the IDE and the parts are readily available.

*At U of I [The MILL](http://mill.lib.uidaho.edu/) will provide all the required materials. However, it may be helpful to set up Arduino IDE on your own computer so that you will have the code and tools available after the workshop.*

------------

## Choosing an Arduino IDE Version

The Arduino IDE is software used to write code for your Arduino projects, then compile and load the code onto your boards.
There is a browser-based version or a stand alone desktop application.

Each version has some advantages and limitations--but in the end they function very similarly and do exactly the same thing!
Personally, I suggest using the desktop version for starting out.

### Arduino Desktop IDE

The Desktop IDE (v1) is software than can be installed on your computer.

- Visit the [Arduino Software page](https://www.arduino.cc/en/software), and look under "Downloads" for the version matching your operating system.

The installation is documented step-by-step for different operating systems:

- [Windows](https://docs.arduino.cc/software/ide-v1/tutorials/Windows) -- download the first option ("Win 7 and newer") which is an installer file. Run the file to install on your system (this will require administrative privileges!)
- [Mac](https://docs.arduino.cc/software/ide-v1/tutorials/macOS) -- download the Max OS X version. Drag the downloaded package into your Applications.
- [Linux](https://docs.arduino.cc/software/ide-v1/tutorials/Linux) -- for most laptops, download the 64 bit version (if you are using Raspberry Pi you might need the ARM 32 bit version). Extract the package to a sensible location, then run the install script.

For workshops and teaching, the "portable IDE" version might be the best option for Windows and Linux.
This requires some manual steps to set up, follow [Arduino IDE Portable Installation](https://docs.arduino.cc/software/ide-v1/tutorials/PortableIDE).
This version will work without administrative privileges!

{% capture v2 %}
*Note: version 2 of the desktop IDE is nearing release!*

V2 will have a very similar interface, but in a completely updated (and improved) package.
The initial install on Windows does not require administrative privilege, however, on first time booting the IDE will try to install cores for your boards and may encounter permissions errors. 
I was able to click the "Board Manager" tab, select "Arduino AVR Boards", and click "install" to get them manually installed and working.
{% endcapture %}{% include card.html text=v2 extra-class="border-info" %}

### Arduino Web Editor 

The Arduino website tends to push people towards using the Web Editor, which is a browser based version of the Arduino IDE. 
It allows you to edit and store all your code online without installing the desktop IDE.

The Web Editor enables some advanced IoT features (that aren't necessary if you are just getting started using Arduino UNO projects), and is tied to a subscription service model--normal use should fall in the "free" tier, but you might get reminders about how great it would be to upgrade! 

To get started you will need an individual account set up and the "Arduino Create Agent" installed on your laptop with administrative privileges.
In many workshop and teaching situations these requirements might make getting started harder with the Web Editor than using the desktop version.

Get started:

- Visit the [Arduino Web Editor](https://create.arduino.cc/editor) and set up an account (or log in).
- [Install the Arduino Create Agent](https://create.arduino.cc/getting-started/plugin/welcome) following their walk through instructions.
- View [Web Editor Docs](https://docs.arduino.cc/cloud/web-editor/tutorials/getting-started/getting-started-web-editor) for more info and tutorials!

*Note:* the documentation is a bit of a maze, seems to be undergoing some updates and rearrangement. 
It is easiest to use the links built into the [Web Editor](https://create.arduino.cc/editor) to find help.
Chromebook's are supported in the newest version, which isn't clear from documentation--and you do not need the old paid app version.
