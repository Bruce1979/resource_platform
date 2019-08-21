#Rapsberry Pi Resources

#GPIOZero Library

[https://gpiozero.readthedocs.io/en/stable/](https://gpiozero.readthedocs.io/en/stable/)

This library is a simple interface for Python 3 developers to access sensors and motors.

For example:

~~~~
from gpiozero import LED
from time import sleep

led = LED(17)

while True:
    led.on()
    sleep(1)
    led.off()
    sleep(1)
~~~~