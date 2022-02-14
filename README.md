# Aviation_400Hz_PowerSupply

400 Hz 115 VAC power supply to feed aviation instruments.

## 400Hz Oscillator

The purpose of the oscillator is to drive an audio power amplifier feeding into a reverse connected low voltage 115 VAC 400Hz transformer.

![schematic](./images/schematic.jpg)

The red LEDS are part of the amplitude stabilizing feedback circuit.
The 33k and 10nF capacitors determine the frequency.
The op-amp is 1/2 of a LM358, a NE5532 was tried but stability was a problem - an 982 pF capacitor between opamp + and - terminals helped eliminate the parasitic oscillation. LM358 does not need this.

![breadboard](./images/breadboard.jpg)

Output is adjustable between +-3 to +-Vcc (12v)
Distortion is adequate judging by viewing waveform

![waveform](./images/waveform.jpg)

Oscillogram shows output set to +-5 Vpp
