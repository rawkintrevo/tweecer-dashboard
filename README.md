

# Setup

On RaspberryPi- run `lsusb` to make sure RPi can "see" device.

Need to get idVendor and idProduct

add line to `/etc/udev/ruldes.d/10-ftdi.rules`

```
ACTION="add", ATTRS{idVendor}=="whatever number", ATTRS{idProduct}=="another number", SYMLINK+="tweecer"
```
