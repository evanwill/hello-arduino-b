---
title: Microcontroller Overview
nav: false
---

## Microcontrollers and SBCs

Arduino is a very popular ecosystem of microcontroller prototyping board based on open source hardware and software--designed to be simple, flexible, affordable, and educational.

You also may have heard of Raspberry Pi, a very popular ecosystem of single board computers (SBCs)--also designed to be simple, flexible, affordable, and educational.
Basically, it is just a minimal computer with everything contained on a small circuit board. See [Getting Started with Raspberry Pi](https://evanwill.github.io/_drafts/notes/rpi-intro2.html).

Both are very flexible, with great documentation and community.
Which one you need depends on your project!

Arduino: 

- Microcontroller board, 8-bit processor, tiny memory.
- Very simple, solid, reliable.
- Very low power consumption.
- Doesn't have an operating system, it just runs your code, i.e. it does one thing really well!
- Generally programmed in C/C++ (not the easiest to learn), and require code to be compiled for flashing to the board.

Raspberry Pi:

- Single board computer with full operating system.
- Having an operating system means you can do lots more stuff, like outputting to a monitor, running software, and using high-level programming languages (mainly Python).
- Relatively simple and reliable, but OS requires updates, might need restarting, etc.
- Consumes much more power than a microcontroller and requires steady power supply to avoid issues.

A new ecosystem of microcontroller boards powered by [MicroPython](https://micropython.org/) / [CircuitPython](https://circuitpython.org/) is emerging which removes some of the barriers of the traditional Arduino programming.
These are worth checking out if you want to use Python, or need a board slightly more powerful than Arduino but don't need a full computer!

## Outline

- quick [survey](https://docs.google.com/forms/d/e/1FAIpQLSeXJYme34JNQvXmdPZ4v9LjFz7hOUxAM3nq3XAczk2xRzNIqg/viewform?usp=sf_link)
- Arduino overview - what are some use cases?
- install IDE 
- code overview
- blink
