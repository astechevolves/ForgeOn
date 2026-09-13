<img src="/Images/ForgeOn%20Logo.png" alt="ForgeOn Logo" width="350">
Voron 2.4 5 head StealthChanger

This build started out as a platform by which to install an INDX. It then took a hard left and became a 5 head stealth changer. In trying to decide how to set up the spools to feed the printer I ended up with a [Storon](https://github.com/astechevolves/storon) to store and feed the printer. 

# ForgeOn — Voron 2.4 StealthChanger

<p align="center">
  <img src="/Images/Printer%20idle%20and%20standing%20by.jpg" alt="ForgeOn Voron 2.4 StealthChanger" width="600">
</p>


## Platform and Motion

- Voron 2.4 350mm
- Beacon level sensor mounted to CNC shuttle
- Five-tool StealthChanger system
- Custom made switch home static in the back corner, for more consistent tool docking
- LDO CNC AWD Kit
- 500 mm/s @ 12K accel

## Electronics

- Waveshare 7.9 touchscreen display running HelixScreen
- Klipper on a Pi5
- LDO Leviathan V1.3 controller w/ expansion board
- Knomi Screens not on the toolhead to [show toolhead specific data](https://github.com/astechevolves/knomi-toolchanger)
- NiteHawk Hexa 6+1 tool hub board
- 5X Nitehawk 36 USB Toolhead boards
- Axiscope and Sexball alignment

## Toolheads
- [Burninator](https://github.com/The-Duke-96/Burninator) toolheads 
- Phaetus Rapido 2 HF hotend
- Sherpa Mini CNC extruder
- Custom Umbilical support and Nitehawk Mount bracket

## Macro Based Fun Stuff
- KIAUH
- ShakeTune
- TMC Auto Tune
- Color coded tool lanes from Storon up to ForgeOn for easy reference
- Pre-Print brush wipe of all toolhead used in coming print, last head to wipe is first to be used in print
- Toolhead LED's assigned color from Orca output to match currently ongoing print
- Custom dock G-Code to wipe on dock/undock against the silicone nozzle wipe strip at each toolhead
- Load/Unload with material prompt and coordinated with the lll-plus buffer's I2C controls to push or pull from Storon to toolhead
- Motion/Position checking to make sure the start position to front wipe location avoid dock position impact
- More details at [my KlipperBackup location](https://github.com/astechevolves/KlipperBackup)


