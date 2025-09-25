# CpEnder3S1ProThumbGen
Creality print v6 post processor to convert the thumbnail images in gcode.

## Tested with
- Creality Print v6.2.2.3203
- Ender 3 S1 Pro
 - F/W version 2.0.8.28F4
 - Screen version 1.0.5

## Installation
### Script
- Install Python.
- Install Pillow.
- Take the .py script and place it somewhere
- Write the full path with commas to the script and your Python installation in the Creality Print "Post-processing Scripts" field under Nozzle/Other

### Executable file (no-Python)
- Take the .zip and unzip it to somewhere
- Write the full path with commas to the CpEnder3S1ProThumbGen.exe in the Creality Print "Post-processing Scripts" field under Nozzle/Other


- Make sure that you have correct Printer Settings:
	- G-code flavor - Marlin
	- G-code thumbnails - 300x300
	- Format of thumbnails - JPEG

	Now this script will work every time when you export the gcode.
- 
## Editing the script
If you edit the script you need to create the executable again.

### Creating the executable
- Install PyInstaller with pip: ``` pip install pyinstaller ```
- Run the command ``` python -m  PyInstaller --onefile --console --nowindowed 'CpEnder3S1ProThumbGen.py```

## Version history
- 2024-06-10 v1.0 Initial release