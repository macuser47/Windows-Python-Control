# Windows-Python-Control
Python 2.7 Functions that enable basic UI interface using Python

This script in conjunction with Numpy, PyWin, and The Python Imaging Library enables anyone to control the Mouse and Keyboard of their Windows PC using python.  

This is based on the tutorial found here: http://code.tutsplus.com/tutorials/how-to-build-a-python-bot-that-can-play-web-games--active-11117  

I added several functions to enchance functionality. (Just noticed how punny this is)

The script features the following functions:

# getMouse()  
Outputs the x, y coordinate of the mouse to the console (ULO)  

# setMouse(x, y)  
Sets the position of the mouse to (x, y)  

# leftClick()
Performs a mouse click with 0.1 seconds between mouse up and mouse down  

# leftDown()
Changes the state of the mouse to mouse down  

# leftUp()
Changes the state of the mouse to mouse up  

# screenGrab()
Returns a image screenshot at the moment the function is called  
  
This can be used for AI purposes by calling getpixel((x,y)) on the image and checking the color (this returns a tuple with the 3 RGB values)  

# type(string)
Likely the most useful function in this script, it types out string with 0.1 seconds between each keypress and release.  

# togglekey(key)
Toggles the single character with 0.1 seconds between key up and key release. This is useful for keys without characters, as nonstandard characters can be input into the function that correpond to the values in the array VK_CODE (e.g. "backspace")  

# pressKey(key)
Works the same as toggleKey, but only puts the key into the down state  

# depressKey(key)
Works the same as toggleKey, but only puts the key into the up state  

# toggleKeyManual(key)
Works the same as toggleKey, but key is the Windows VK Hex Code for the character, not the cahracter itself. (e.g for tab: 0x08)  

# pressKeyMaunal(key)
Works the same as toggleKeyManual, but only puts the key into the down state  

# depressKeyMaunal(key)
Works the same as toggleKeyManual, but only puts the key into the up state  

# shiftKey(char)
Toggles key that requires shift to be pressed, with 0.1 seconds between key down and key up  

# Miscelaneous Functions  

#getRand(a, b)
Returns a random float (inclusive) between a and b.  

#getRandInt(a, b)  
Returns a random integer (inclusive) between a and b.

