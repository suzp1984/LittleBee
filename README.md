LittleBee
=========

An image convert GUI tool for Embedded developers, implemented by PyQt.

This application suppose have the PyQt's MainWindows style, that means
it should have menus, toolbars, central widgets and status bar.


  +---------------------------------------------------------------+ menu
  +---------------------------------------------------------------+
  |                                                               | toolbars
  +---------------------------------------------------------------+
  |                                                               |
  |                                                               |
  |                                                               |
  |                                                               |
  |                                                               |
  |               central widget                                  |
  |                                                               |
  |                                                               |
  |                                                               |
  |                                                               |
  |                                                               |
  |                                                               |
  |                                                               |
  +---------------------------------------------------------------+ status bars
  +---------------------------------------------------------------+

Functions
---------

Image process, It always need to load an piece of image into single color LCD 
in embedded development. Take following instance as example, I have an 
128*128 LCD, and I need to display an image into the LCD to prove the device 
works. The image file should be the format as an 128*128 bit buffer, with bit
0/1 to indicate on/off of an point. I can make the image by this tools.

1. load an image into app.
2. config the select region into 128 * 128.
3. move the select region to select the right region.
4. click save, then the app can conert and save into 128 * 128 bits buffer
into target file.
