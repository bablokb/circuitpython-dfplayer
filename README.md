Introduction
============

This is a library for the mini-dfplayer, a minimalistic MP3-player
available for a few bucks from Ebay, Amazon and other distributors.

![](dfplayer.jpg)

The chip has a number of pins for direct control, but also an
UART-interface and this library controls the chip using the documented
commands.

The core of the code is from a micropython implementation of the interface
[https://github.com/jczic/KT403A-MP3](https://github.com/jczic/KT403A-MP3).


Installation
------------

Just copy the file `lib/DFPlayer.py` to your `lib`-directory on your board.


Usage
-----

Import the library and create a `DFPlayer`-object. If you don't pass an
uart, the constructor uses `board.RX` and `board.TX` to create a default.
Use the created object to control the player. For the API just have a
look at the source-code.

A real-world example can be found in the project:
[https://github.com/bablokb/xmas-music-box](https://github.com/bablokb/xmas-music-box).