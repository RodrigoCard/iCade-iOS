# iCADE-iOS
Project which demonstrates using the iCADE and iControlPad with iOS devices.

## Demo
Pair up you iCADE or iControlPad, run the project and you're off.

## Usage
To use in your own app, copy the following 3 files from the iCade folder:

* `iCadeReaderView.h`, `iCadeReaderView.m` and `iCadeState.h`

Add an instance of `iCadeReaderView` to your main game view.  Set `view.active = YES` to ensure 
the view receives events from the controller.  In addition, when active, the view will 
automatically handle `didEnterBackground` and `didBecomeActive` notifications, to avoid loss of events.  
You can either read the `iCadeReaderView.iCadeState` property to determine the current state, or 
implement the `iCadeEventDelegate` protocol on your target to receive appropriate notifications.

## Hardware Compatibility
* [iCADE](http://www.thinkgeek.com/electronics/retro-gaming/e762/), 
* [iControlPad](http://icontrolpad.com/home) with [firmware revision 2.0](http://icontrolpad.com/support)
* [Gametel](http://gametel.eu/index.php/english)

### Mapping
Lists the mapping between various controllers.  Directional controls are the same.  It is recommended 
you use the latest [v2.1a](http://boards.openpandora.org/index.php?/topic/5137-new-icp-test-firmware-v21/page__view__findpost__p__89228) iControlPad firmware for better button mappings.

8 buttons are mapped as follows:

	iCADE		iControlPad (v2.0)	iControlPad (2.1a)
	A			START				SELECT
	B			B					START
	C			SELECT				LEFT SHOULDER
	D			Y					RIGHT SHOULDER
	E			RIGHT SHOULDER		Y
	F			LEFT SHOULDER		B
	G			A					X
	H			X					A
	
The iCADE button layout is:

	A C E G
	B D F H

## License
Copyright (C) 2011 by Stuart Carnie

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.


