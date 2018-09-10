# NFC Door Lock
This simple Python script which was featured in [Issue 4 of HackSpace magazine](https://hackspace.raspberrypi.org/issues/4) allows you to unlock a door with an NFC / RFID keyfob.

This code works with a USB RFID reader, which acts like a keyboard and inputs the code from the fob as if it were being typed on a keyboard. The striker plate is powered by its own 12V power supply and switched by a 5V single-channel relay switch connected to the Raspberry Pi's GPIO ports as shown in the diagram below:

![alt text](https://github.com/paulfp/NFC-Door-Lock/raw/master/circuit-diagram.jpg "Circuit Diagram")

## Dependencies
The script uses <b>evdev</b> which can be installed like this:

```python
sudo pip install evdev
```