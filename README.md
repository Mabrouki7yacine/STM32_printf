# Viewing Serial Output

To view serial output from your device, use a USB-to-Serial adapter to connect the device to your PC. Once connected, open a serial terminal :

- **Windows:** PuTTY — select `Serial`, choose the COM port, set baud rate
- **Linux:** `screen /dev/ttyUSB0 115200` or `picocom -b 115200 /dev/ttyUSB0`
- **Arduino IDE:** Serial Monitor

On Linux, if you get a permission error, add yourself to the `dialout` group:
```bash
sudo usermod -aG dialout $USER
```
Requires logout/login to take effect.
