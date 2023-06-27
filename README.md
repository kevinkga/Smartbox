# Smartbox
A 3d printer smart filament storage solution that enables multi material printing.

# Features
- Drybox
  - Displays humidity levels as well as temperature 
  - Even when your filament is not being dried is remains in a low humidity environment thanks to dessicant cannisters.
  - An automated mode also ensures that the humidity level remains low by activating the drying process if humidity levels exceed configured thresholds.
- Dehumidification of filament.
  - Set your filament type and the amount of time you would like for it to extract the moisture.
  - The lid stays slightly open and the fan heater circulates air, letting moisture escape during drying process.
  - When complete the lid shuts itself and the dessicant inside ensures that the filament as well as the dessicant remains dry.
- Easy loading and unloading of filament.
  - Just place the spool into the box and attach the filament to the box.
  - The box detects the filament and pulls in more until it is primed.
- Spool usage monitor
  - The system comes with a built-in scale that monitors how much filament you have left.
  - The remaining weight is displayed on the status indicator and can be referenced at any point to know if you will have enough filament for a print.
 
# Setting up the box
Each box comes with a dock. Place the box onto its dock, ensuring that the docking pins align to the bottom. Plug the canbus connector into your mainboard's CAN connection, if it is the first box. Otherwise, connect it to the CANBus outlet of the adjacent box.

## Klipper
Once you complete the hardware setup, you will need to let Klipper know that you've added a new device. To do this add the [include box1.cfg] entry to your printer.cfg

# Loading filament
Unpack your filament and place it on the spool with the tip of the filament pulling from over the spool towards the front. Place the tip of the filament into the feeder. 

The indicator LED changes to blinking yellow while the box primes the filament for use. If everything goes well the led stays in solid green.
