# PocketStar Emulator


![PocketStarEmulator](https://raw.githubusercontent.com/Schuemi/PocketStarEmu/master/PocketStar.PNG)

This is a PocketStar : https://www.zepsch.com/pocketstar/

This emulator should help to develope more great games for the Pocketstar. 


- Please note that this is an beta version

This is my PocketStar Emulator. Sorry, but no Source code release,yet. But you can download the newes compiled version here: https://github.com/Schuemi/PocketStarEmu/releases

You need Windows10 64bit and a fast computer to run.

# How to start?

pocketstaremu.exe [filename] [-cycles] [-scaleX] [-sd SDCARDIMAGE.img] [-nosd] [-startrec] [-stoprec [FRAMES]] [-screenshot [FRAME]] [-addr [ADDRESS]]  [-battery [full/half/low/empty]] [-charging] [-draining]

filename 

  The filename has to be a PocketStar Game (compiled as Build type "game"),  "pocketris.bin" for example.
  
-cycles

  This means that the emulator executes the real CPU cycles. Your computer must be very fast to accurately replicate the cycles. Something about an Intel i7 with 3.2 GHz, I think. If your computer isn't fast enough, but you need the right number of cycles during an emulated second, please use it. 
  
 -scaleX
 
  The window size. you can use -scale2 to -scale8. (Without a space between -scale and the number)
  
  -sd SDCARDIMAGE.img
  
  Can be used to specify the name of an SD card image. If this option is omitted, the file "PocketSD.img" will be loaded.
  
  -nosd
  
  Insert no SD Card
  
  -startrec
  
  Starts gif recording immediately
  
  -stoprec [FRAMES]
  
  Stops recording after X frames and quits the emulator. One frame is a 10th of a second.
  
  -screenshot [FRAME]
  
  Makes a screenshoft after X Frames and quits the emulator. One frame is a 10th of a second.
  
  -addr [ADDRESS]
  
  Loads a program at this address. The default is 0x10000. If you whant to load the Menu for example, enter 0x2000.
  
  # Serial Monitor
  
  To debug your program you can open a serial monitor. If you open Serial1 and write to it a window will automaticly open and shows your debugging messages.
  For example:
  ```
      Serial1.begin(115200);
      Serial1.print("Hello World!\n");
  ```
  
  ![SerialMonitor](https://raw.githubusercontent.com/Schuemi/PocketStarEmu/master/sm.PNG)
  
  -battery [full/half/low/empty] [-charging] [-draining]
  With this parameter you can simulate the battery. Set it to full, half, low or emty. also you can add -charging or -draining. The speed of charing or draining is faster than on the real hardware, I think it's better to test this way.
  
  # Animated Gifs
  
 
 You can start a gif recording by pressing the key "G" or with the start parameters. While recording you will see a blinking red square in the upper right corner. (Of corse this square is not visible in the recording). To stop it, press "G" again. The Gif will be saved in the working directory and the name of the Game with a ".gif" at the end. Multiple gifs are possible.
 
 # PNG screenshot
 
 You can make a PNG screenshot by pressing "P" or with the start parameters. The png will be saved in the working directory and the name of the Game with a ".png" at the end. Multiple screenshots are possible.
  
  
  # SD Card
  
  The SD card is emulated with a RAW image formatted in FAT32. In the zip file you find the Image "PocketSD.img". This is a 36MB image, already formated and with "games" and "apps" directorys. In Windows you can mount this image with the free software "OSFMount" ( https://www.osforensics.com/tools/mount-disk-images.html ). After mounting the image, you have a new volume as if you had inserted a real SD card. Please demount the image, before you start the PocketStar Emulator. Otherwise the Emulator can't write on the Image.
  
  # The controls
  UP = arrow up
  
  LEFT = arrow left
  
  DOWN = arrow down
  
  RIGHT = arrow right
  
  A = space
  
  B = left strg
  
  Pause = ESC
  
  
  
  # What is missing?
  - some CPU instructions are missing (but not used somewhere, yet)
  - many SAMD21 components (also not used in a game, yet)
  - some display commands
  - the display colors are not quite right yet
  
  
