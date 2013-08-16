GooeyPi
=======
Simple wxPython-based crossplatform Pyinstaller GUI front-end. Supports UPX, as well as some of the most common Pyinstaller options.

Currently only tested on Windows, but plan on testing on Linux and Mac OS X shortly.

Features
--------
Easy-to-use, saves your preferences, allows for quick building of executable
binaries. Built and tailored specifically for PyInstaller. 

Supports the following common flags: 
- --onefile Single-file deployment
- --ascii Do not include unicode encoding
- --noconfirm Remove output directory without confirmation
- --noconsole Windowed mode (no console on program launch)

Binaries are automatically saved in the same directory as the script file. 

Prerequisites
-----------
*Required*
- wxPython >= 2.9.4.0
- Python >= 2.7.3 (not compatible with Python3)
- PyInstaller >= 2.1 (development version. Support for 2.0 is coming soon!)
- configobj >= 4.7.2

*Optional*
- UPX >=3.09


Installation
------------
No installation needed. Just clone/download and run: python gooeypi.py
You may need to use: python2 googlepi.py if you have Python3 installed. 

Usage
-----
- Click Options.
- Select your Pyinstaller directory, and optionally, your UPX directory.
- Select any flags you wish to pass to the installer. 
- Click OK, watch as your application builds. 
- Your dist folder and binary will be in the same folder as your Python script.

To Do
-----
- Provide options for build/dist folder destinations
- Move the pyinstaller subprocess to its own thread
- Provide option for manual flags
- Test on ~~Linux~~ / Mac
- Autodetect Python2 command line. **fixed??**
- ~~Fix some bad path code (should be using os.path.join)~~
- ~~Fix preferences not saving on Linux~~
- ~~Fix pyinstaller path not saving~~

Contributing
------------
I welcome all feature recommendations, issues, and contributions! 
