# ChosunTruck

## Introduction
ChosunTruck is an autonomous driving solution for [Euro Truck Simulator 2](https://eurotrucksimulator2.com/).
Recently, autonomous driving technology has become a big issue and we have studied the technology related to this.
It is being developed in a simulator environment called Euro Truck Simulator 2 to study it with vehicles.
Because this simulator provides a good test environment that is similar to the real road, we chose it.

## Features
* You can drive a vehicle without handling it yourself.
* You can understand the principle of autonomous driving.
* (Experimental) You can detect where other vehicles are.

## How To Run It
### Windows

#### Dependencies
- OS: Windows 7 64bits

- IDE: Visual Studio 2015

- OpenCV version: 3.0

#### Required to allow input to work in Windows:
Note: Input is not currently working correctly.
- **Go to C:\Users\YOURUSERNAME\Documents\Euro Truck Simulator 2\profiles and edit controls.sii from di8.keyboard/fusion.mouse to sys.keyboard/sys.mouse.** (thanks Komat!)

#### Then:
- Open the visual studio project and build it. 
- Run ETS2 in windowed mode and set resolution to 1024 * 768.(It will work properly with 1920 * 1080 screen resolution and 1024 * 768 window mode ETS2.)

### Linux
#### Dependencies
- OS: Ubuntu 16.04 LTS

- OpenCV version: 3.1

- (Optional) Tensorflow version: 0.12.1

### Build the source code with the following command (inside the linux directory).
```
make
```

- Run ETS2 in windowed mode and set its resolution to 1024 * 768. (It will work properly with 1920 * 1080 screen resolution and 1024 * 768 windowed mode ETS2)
- It cannot find the ETS2 window automatically, move the ETS2 window to the right-down corner to fix this.
- In ETS2 Options, set controls to`Keyboard + Mouse Steering`, `left click` to acclerate, and `right click` to brake.
- Go to a highway and set truck's speed to 40~60km/h. (I recommend you turn on cruise mode to set the speed easily)
- Run this program!

#### To enable car detection mode, add an option -D or --Car_Detection.
```
./ChosunTruck [-D|--Car_Detection]
```
----
If you have some problems to run this project, reference the demo video below. Or, open a issue to contact our team.

## Demo Video
Lane Detection(Youtube link)

[![youtube link](http://img.youtube.com/vi/vF7J_uC045Q/0.jpg)](http://www.youtube.com/watch?v=vF7J_uC045Q)

Lane Detection + Vehicle Detection(Youtube link)

[![youtube link](http://img.youtube.com/vi/w6H2eGEvzvw/0.jpg)](http://www.youtube.com/watch?v=w6H2eGEvzvw)

## Founders
Chiwan Song, chi3236@gmail.com

JaeCheol Sim, simjaecheol@naver.com

Seongjoon Chu, hs4393@gmail.com

## Contributers
[zappybiby](https://github.com/zappybiby)

## How To Contribute
Anyone who is interest in this procject is welcome! Just Fork it and Pull Requests!

## License
ChosunTruck, Euro Truck Simulator 2 auto driving solution
Copyright (C) 2017 chi3236, bethesirius, uoyssim

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
