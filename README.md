# PocketStar Emulator


![PocketStarEmulator](https://raw.githubusercontent.com/Schuemi/PocketStarEmu/master/PocketStar.PNG)

This is a PocketStar : https://www.zepsch.com/pocketstar/

This emulator should help to develope more great games for the Pocketstar. 


- Please note that this is an alpha version

This is my PocketStar Emulator. Sorry, but no Source code release,yet. But you can download the newes compiled version here: https://github.com/Schuemi/PocketStarEmu/releases

You need Windows10 64bit and a fast computer to run.

# How to start?

pocketstaremu.exe [filename] [-cycles] [-scaleX] [-sd SDCARDIMAGE.img] [-nosd]

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
  - no vibration yet,
  - no SD-Card support
  - some CPU instructions are missing (but not used somewhere, yet)
  - many SAMD21 components (also not used in a game, yet)
  - some display commands
  - no brightness
  - the display colors are not quite right yet
  
  
