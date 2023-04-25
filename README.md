# Strobe-Tuner
Strobe tuner for electric guitar in standard tuning using Arduino Uno

This program uses an interupt to constantly monitor voltage of an input signal.

The signal is sampled and analyzed to calculate its frequency.
The measured frequency is compared to the frequencies of each string on a standard electric guitar.  The closest desired frequency is chosen.  

The LEDs are sequenced left or right depending on the input frequency being higher or lower than desired frequency.  The LED sequence slows down as the input frequency approaches the desired frequency.  

When the input frequency matches the desired frequency, the LEDs flash in unison.

The program also includes a warning when the input signal amplitude is to large for the analog input of the Arduino Uno.