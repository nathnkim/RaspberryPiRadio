# RaspberryPiRadio
Wireless radio hacked together out of thrift store speakers, a cordless drill battery, and a Raspberry Pi.

## Notes to self
Internet radio streams are played via the `mpv` player (https://mpv.io/), which is run by a `systemd` service file in order to auto run upon Raspberry Pi boot-up. Service files live in `/etc/systemd/system`. Service can be restarted by 
```
sudo systemctl daemon-reexec
sudo systemctl daemon-reload
sudo systemctl enable [SERVICE FILE NAME].service
sudo systemctl start [SERVICE FILE NAME].service
```

## Hardware 
- Bose Companion 2 speakers (original series) 12V DC input
- Raspberry Pi 3B+ Version 1 running Debian GNU/Linux 12 (bookworm)
- Raspberry Pi DAC Pro hat 
- Dewalt 20V Li-ion batteries

---
## To Do List, Nov 22 2025
- Add a switch to pi GPIO + accompanying service file to boot up/ turn off Raspbery Pi
- Finish spec'ing auxilliary components for LM2596 adjustable step down converters to convert 20V battery to 12V and 5V sources for Pi and speakers 



