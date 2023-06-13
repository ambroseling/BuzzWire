# BuzzWire
A computer organization project that used C to create a hardware game

![IMG_7058](https://user-images.githubusercontent.com/93873940/231223566-0d163d1c-a31e-4ad7-8db0-216d722fe8ac.JPG)

## Instructions
The aim of the game is to trace a wire around a metal maze to the other side in 30 seconds or less WITHOUT touching the wire

## Game Logic

We used ARM assembly and C to write interrupts (Generic Interrupt Controller & IRQ handler) for the KEYs and ARM A9 Private Timer. We also used an Analog-To-Digital Converter on the DE1-SoC board to read voltage changes from the circuit board. 

## Circit logic
We used an AND gate chip 7S0008 (input: 5v and floating wire(the handheld wire) / output: 5v if no touch, 0v if wire is touched). The wire is attached to GND so when the wire is touched the circuit is grounded, which reads a 0v.
