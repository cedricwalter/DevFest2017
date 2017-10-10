#  First steps with PiFace Digital and Python
To use Piface Digital with Python, import the pifacedigital module:
```
import pifacedigitalio as p
```
Before use, the board must be initialised with a call to init.
```
p.init()
```
There are three main functions to control the interface

```
digital_read(pin_number)
```
returns 1 or 0 depending on the state of the input numbered pin_number
```
digital_write(pin_number, state)
```
sets the output numbered pin_number to state 0 or 1. State 1 turns the LED on and enables to open collector to sink current
```
digital_write_pullup(pin_number, state)
```
sets a 10k pullup on input numbered pin_number to be state 0 or 1. State 1 is pullup enabled

# Simple python examples
One of the quickest ways to get going is to look at examples of PiFace Digital in use. These can be ran by moving into the PiFace Digital examples directory
```
cd /usr/share/doc/python3-pifacedigitalio/examples
```
Type ls to view the contents of this directory and run the examples like so
```
python3 blink.py
```

##  Controlling an output (turn a relay on)
The first two outputs control the two on-board relays. To turn the first relay on, start a new python interpreter and type the following:

```
import pifacedigitalio as p
p.init()
p.digital_write(0,1)
```

##  Flashing an LED
```
from time import sleep
import pifacedigitalio as p
pinit()
while(True):
     p.digital_write(0,1) #turn on      sleep(1)
     p.digital_write(0,0) #turn off
     sleep(1)
```
##  Reading an input
To read the state of an input use the p.digital_read(pin) function as shown below. If a button is pressed the function returns a 1, otherwise it returns a 0.
```
import pifacedigitalio as p
p.init()
p.digital_read(1)
```
Python prints 0.
Now hold down switch number 1 (marked S1) and type p.digital_read(1) again.
Python prints 1.


see http://www.piface.org.uk/guides/Install_PiFace_Software for more