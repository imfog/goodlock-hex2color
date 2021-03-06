# Samsung's Good Lock Hex to Color
This python program takes in a hex value and then uses Android's ADB interface to pick the correct color from Samsung's Good Lock color picker.

This tool run on the command line only.  Knowledge of basic command line usage is need to use this tool.

The first and only argument needed is the hex value of the color you want.

Please view the footnotes before you get started.

## Requirements

### Windows  
1. [Samsung's Universal USB Driver for Mobile Phones](http://downloadcenter.samsung.com/content/DR/201602/20160219075034805/SAMSUNG_USB_Driver_for_Mobile_Phones_v1.5.45.00.exe)  
2. [ADB](https://www.androidfilehost.com/?fid=24521665358595410)
3. [Python 3](https://www.python.org/)

### Mac/Linux
1. ADB (footnote #2)
2. [Python 3](https://www.python.org/)

## How to
Your phone should be connected to your computer with a USB cable and USB Debugging should be turned on. Good Lock should be open and opened up to the **custom color picker screen** with the tile you want to change set as the selected tile.

If you do not have a button at the bottom of the color picker screen that says "Custom", update Good Lock.

You should run this command for each tile you want to change, replacing the hexadecimal color code as needed:

`python hex2goodlock.py "#253f3f"`  
or   
`python hex2goodlock.py`

### Example

<p align="center">
<img src="/images/how-to.gif" />
</p>
[Full Youtube Video](https://www.youtube.com/watch?v=pSsmssP1OXU)


## Footnotes
1. The ADB installer for Windows comes from [this thread](http://forum.xda-developers.com/showthread.php?t=2317790)
2. The ADB binary for Mac can be downloaded using [this guide](http://forum.xda-developers.com/showthread.php?t=1917237) or, for [Homebrew](http://brew.sh/index.html) users, with `brew install android-platform-tools`
3. Linux people should install ADB from their package manager. I trust that if you're running linux you know what you're doing and don't want me mucking up your OS
4. Mac and Linux should come with Python and you should not need to install it. To determine if you have python please open Terminal and type `python -V`. If you have Python this should return which python version you have. If you get anything else you don't have python.
5. This program uses a few hacks and tricks. Right now these hacks/tricks are working but may change in the future.

### Tested on
* Galaxy S7 Edge from T-Mobile in the condensed display mode using macOS.
* Galaxy S7 Edge from T-Mobile in the standard display mode using macOS.
* Galaxy S7 from T-Mobile in the condensed display mode using Windows 10.
* Galaxy S7 from T-Mobile in the standard display mode using Windows 10.
* Galaxy S7 from AT&T in the standard display mode using Windows 10.
* Galaxy S7 from AT&T in the standard display mode using OSX El Capitan.
* Galaxy S7 Edge from Verizon in the condensed display mode using Windows 10.
* Galaxy S7 Edge from T-Mobile 480 DPI using macOS.

### Beta Testers
* [blindingstars](https://github.com/blindingstars)

<sub><sup>Beta Testers: If you want to be added to this list please open an issue or a pull request</sub></sup>

### Contributors
* [blindingstars](https://github.com/blindingstars)
