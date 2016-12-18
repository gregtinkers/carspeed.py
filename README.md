# Car Speed Detection - carspeed.py (version 2.0)

## Blog URL

Full program details at:   https://gregtinkers.wordpress.com/2016/03/25/car-speed-detector/

## Description

This program for the Raspberry Pi determines the speed of cars moving through the Picamera's field of view. An image of the car and labeled with its speed is saved.

## Requirements

* Raspberry Pi 2 Model B  (or 3)
* Picamera
* Opencv

## Usage

Install OpenCV 3 and Python 3 on the Pi. 

Copy carspeed.py into the same directory as your home directory. 

Point the Picamera at the road. Before you run carspeed.py, modify the constant DISTANCE to the distance from the front of the Picamera lens to the middle of the road. You may also need to adjust the vflip and hflip to match you camera's orientation.

Run from a terminal with:
     python carspeed.py

Use a mouse to draw a rectangle around the area you wish to monitor. I recommend a height just sufficient to capture the whole car and a width about one half the frame, centered. Press 'c' and the program will begin monitoring the road.

As cars pass through the monitored area, an image will be written to disk with the speed.

Exit the program with a press of the 'q' key.

## License:

(The MIT License)

Copyright (c) 2016 Greg Barbu

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
