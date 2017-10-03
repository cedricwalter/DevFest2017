# Sense HAT examples

Example programs using the Sense HAT - particularly for the Astro Pi competition

## About

British ESA astronaut [Tim Peake](https://twitter.com/astro_timpeake) is going to the [International Space Station](https://twitter.com/Space_Station) for 6 months at the end of 2015 and taking two [Raspberry Pi](https://www.raspberrypi.org/) computers to run experiments coded by participants in the [Astro Pi](http://astro-pi.org/) coding competition for UK schools.

The Sense HAT is the hardware attachment board mounted to the Pis on the ISS, and will be available to the public as a product soon.

The Raspberry Pi Foundation have created a [Python API](https://pypi.python.org/pypi/sense-hat) to provide access to the board's LED matrix and sensors. See the documentation at [pythonhosted.org/sense-hat](http://pythonhosted.org/sense-hat/)

## Usage

With a Sense HAT on a Raspberry Pi, and the firmware and Python library installed (see [Sense HAT software installation](http://pythonhosted.org/sense-hat/)),
download or clone this repository, enter the `python` directory and run the examples with Python 3 or Python 2.

e.g.

```bash
git clone git://github.com/cedricwalter/devfest2017
python3 random_sparkles.py
```

## Make your own program
Follow this [guide](https://github.com/raspberrypilearning/astro-pi-guide)

## Examples

### Magic 8 Ball 

- [magic8ball.py](magic8ball.py)

### Random Sparkles

Let your Sense HAT shine with pride

- [random_sparkles.py](random_sparkles.py)

### Conway's Game of Life

[Conway's Game of Life](https://en.wikipedia.org/wiki/Conway's_Game_of_Life) is a zero-player cellular automaton game

- [conway.py](conway.py)

The game is randomly generated each time. Some games will be over very quickly, others will last a few generations. Press `Ctrl + C` to quit and then run it again.

### Minecraft Colour

Walk around a Minecraft world and the Sense HAT will light up the colour of the block you're standing on

- [minecraft_colour.py](minecraft_colour.py)

Be sure to open a Minecraft world first

### Minecraft Map

Walk around a Minecraft world and the Sense HAT will show an 8x8 map of your player's surroundings

- [minecraft_map.py](minecraft_map.py)

Be sure to open a Minecraft world first. Note blocks are cached for speed so alterations are not accounted for.

### Colour Match Game

Two colours are selected at random and shown on the Sense HAT - controlling the RGB values with the keyboard you have to try to match the middle squares with the outside colour

- [colour_match.py](colour_match.py)

Keys:

```
r: increase red
t: decrease red
g: increase green
h: decrease green
b: increase blue
n: decrease blue
esc: give up
```

### Jokes

One line jokes scrolling on your Sense HAT display

- [jokes.py](jokes.py)

Choose your own jokes list

### Geeky Jokes

One line programmer jokes scrolling on your Sense HAT display

- [geeky_jokes.py](geeky_jokes.py)

Requires [pyjokes](http://pyjok.es/)

### Astro Cam

Stream a scaled-down picture from the camera module to the Sense HAT's LED matrix

- [astro_cam.py](astro_cam.py)

Requires a [camera module](https://www.raspberrypi.org/products/camera-module)

### Temperature Bar Graph

Show a bar graph of the temperature in real time

- [temperature.py](temperature.py)

### Humidity Bar Graph

Show a bar graph of the humidity in real time

- [humidity.py](humidity.py)

