![image](https://github.com/arbadacarbaYK/Matrix-Bitcointicker/assets/63317640/70560a1b-4d50-4117-a905-a58b132a459f)

# Bitcointicker for the MAX7219 Dot Matrix Display

Import the .ino to Arduino. Set your board to esp32 dev module and install the libraries given in the include statements. 
Change your Wifi and optionally also the PIN-out, if you chose to set them different than given in the sketch which next to the GND/VCC is

#define CLK_PIN   18 // VSPI_SCK

#define DATA_PIN  23 // VSPI_MOSI

#define CS_PIN    5  // VSPI_SS


Set your port to the usb-device you are adressing, press the left button on the esp32 for (only) 2seconds while also pressing upload in Arduino.

If your computer has the (usb driver)[https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers?tab=downloads], but your Arduino is unable to access your computer's serial port, you'll get an error like "Failed to open serial port" or something like "dev/tty01 not found". On Linux and MacOS computers, you can fix this by running a command that (temporarily) gives all users access to it with 
```
sudo chmod 777 /dev/ttyUSB*
```

Have fun.

![photo_2024-07-06_13-11-57](https://github.com/arbadacarbaYK/Matrix-Bitcointicker/assets/63317640/f20c29de-2e8b-49c7-b48a-980124b0bacf)
