# BIAS-FX-Clue-Midi

Modification of [MIDI CLUE BLE Glove](https://bit.ly/2PBzcX9) for BIAS
FX2.  Lets you do crazy things like
* Use your foot as an expression pedal
* Use proximity as a momentary switch
* Switch banks and presets

## Operation

Touch button 3 toggles modes. 

### Mode 1: CC Program (Default)

This mode lets you select CC modes and change the default CC numbers:
71, 72, 73.  X value is returned on the first (tilt left and right)
value, Y value from 0° to 70° is the default (opposite of an
expression pedal, easier for a foot mount), and the proximity sensor
works as a momentary switch.
 * Physical Button 1: Decrease Selected CC Number
 * Physical Button 2: Increase Selected CC Number
 * Touch Button 1: Pause CC Messages 
 * Touch Button 2: Move cursor

### Mode 2 Bank Switch

Doesn't actually move your bank up and down but sets the bank
number...so you'll need some clairvoyance; Just make sure you have a
real bank selected.  There are [8 banks of 4](https://bit.ly/3gK57kb)
to choose from.
 * Physical Button 1: Bank Down
 * Physical Button 2: Bank Up

### Mode 3 Toggle Presets

Toggles within the current bank
 * Physical Button 1: Preset 1
 * Physical Button 2: Preset 2
 * Touch Button 1: Preset 3
 * Touch Button 2: Preset 4

## What you'll need:

* [Adafruit CLUE - nRF52840 Express with Bluetooth
   LE](https://www.adafruit.com/product/4500)
 * Battery Go rechargable! pick one...both work and I used both for over an hour.
   * Super Tiny: [Lithium Ion Polymer Battery - 3.7v
     100mAh](https://www.adafruit.com/product/1570)
   * Tiny (+ more juice): 
     * [Lithium Ion Polymer Battery Ideal For Feathers - 3.7V
       400mAh](https://www.adafruit.com/product/3898)
     * [Lithium Ion Polymer Battery with Short Cable - 3.7V
     350mAh](https://www.adafruit.com/product/4237)
 * Charger (pick one)
   * [MicroUSB](https://www.adafruit.com/product/1904)
   * [USB C](https://www.adafruit.com/product/4410)
 * Cable: I assume you have a cable that goes MicroUSB into your
   computer...if you don't go get it.
 
 ## Glove Tutorial 

Adafruit has this tutorial on the [CLUE BLE MIDI
Glove](https://learn.adafruit.com/clue-midi-glove), do that first.
This code was derived from that project and the [API
docs](https://circuitpython.readthedocs.io/projects/clue/en/latest/api.html).
