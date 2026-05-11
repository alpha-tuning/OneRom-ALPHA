# How To Flash Firmware

## Flashing the ALPHA Firmware to OneROM Fire

To flash the firmware onto your OneROM Fire, follow the steps below.

### Enter DFU Mode
Place your OneROM Fire into DFU mode by connecting the **BOOT** pin to **Ground**.

### Connect the Device
Plug the USB cable into the OneROM Fire.

Your Windows machine should detect the device and open a new window showing the **RP2350 device root folder**.

### Extract the Firmware Files
Download and unzip the `AlphaEMUxxxxx.zip` file from the repository.

### Copy the Firmware
Drag the `.UF2` firmware file into the RP2350 root folder.

Once the file finishes copying, unplug the OneROM Fire from USB.

### Exit DFU Mode
Remove the connection between the **BOOT** pin and **Ground**.

### Reconnect the Device
Plug the USB cable back into the OneROM Fire.

### Verify Device Detection
You should now see **3 devices** appear in Windows Device Manager:

- **2 new COM ports**
- **1 dummy port** labeled:  
  `One ROM, the most flexible replacement ROM for your retro system`

One COM port is used for **emulator communication**.  
The other COM port is reserved for **development use**.

### Connect to HTS
Open **Honda Tuning Suite (HTS)** and select the correct emulator COM port.

Set the baud rate to:

`921600`
