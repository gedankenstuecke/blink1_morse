# blink1-tool morse code wrapper
This is a small python script that wraps around the blink1-tool for the command line. It translates the command line input text into [morse code](http://en.wikipedia.org/wiki/Morse_code) and emits them through the blink1. 

## Setup
* Make sure you have [downloaded the right version of the blink1-tool](http://blink1.thingm.com/blink1-tool/) for your OS. 
* Set the BLINK_TOOL_PATH in morse.py to the full path to your blink1-tool
* That should be it! 

## Examples
Here are two short clips showing it in action: 
* http://vine.co/v/b6wwHZJJUAQ
* http://vine.co/v/b6ZtaiFzQWF

## Gosh, this code is ugly!
Yup, it is. It's a quick hack with some features added as an afterthought. But it seems to work. If you want to rewrite it or make it less ugly: Go for it!

## Commands
```
usage: morse.py [-h] [-c COLOR] [-s] [-tc TARGET_COLOR] [-t TIME] text

positional arguments:
  text                  This is the text that should be emitted

optional arguments:
  -h, --help            show this help message and exit
  -c COLOR, --color COLOR
                        The (initial) color of the blinks. Specify as R,G,B.
                        Default: 255,255,255
  -s, --shift           Should the color shift? If yes: --target-color needs
                        to be specified
  -tc TARGET_COLOR, --target-color TARGET_COLOR
                        The final color of the blinks. Specify as R,G,B.
                        Default: 255,255,255
  -t TIME, --time TIME  Duration of a single dit in milliseconds. Default: 100 
```
