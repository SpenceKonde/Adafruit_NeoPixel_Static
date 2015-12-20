# MODIFIED NeoPixel Library - removed use of digitalWrite/pinMode

Usually, pinMode() is used only in setup() where it can be replaced by a bit of direct port manipulation. In this case, getting rid of the pinMode() calls in this library (which are entirely unnecessary - you just need to make sure the pin is an output and low when you start using it) will save the 250-300 bytes of flash used to store pinMode function call. 


# Adafruit NeoPixel Library

Arduino library for controlling single-wire-based LED pixels and strip such as the [Adafruit 60 LED/meter Digital LED strip][strip], the [Adafruit FLORA RGB Smart Pixel][flora], the [Adafruit Breadboard-friendly RGB Smart Pixel][pixel], the [Adafruit NeoPixel Stick][stick], and the [Adafruit NeoPixel Shield][shield].

After downloading, rename folder to 'Adafruit_NeoPixel' and install in Arduino Libraries folder. Restart Arduino IDE, then open File->Sketchbook->Library->Adafruit_NeoPixel->strandtest sketch.

[flora]:  http://adafruit.com/products/1060
[strip]:  http://adafruit.com/products/1138
[pixel]:  http://adafruit.com/products/1312
[stick]:  http://adafruit.com/products/1426
[shield]: http://adafruit.com/products/1430
