# usb2serial-driver

to use the usb to serial dongle:

run the PL2303_64bit_installer
download/install .NET Framework 3.5 if it prompts you
you'll need to restart

run the installer again
it prompts you to plug in the decive
plug in the device, press continue
restart the computer

check for drvice manager and make sure it is assigned a com port

power the esp8266 with an external 3.3V supply (can't power it
from D-SUN dongle)

connect:
dongle gnd to esp gnd
dongle TX to esp RX
dongle RX to esp TX

if using the reset/program board I made:
put switch close to reset button (or middle) to go into program mode
put switch farthest away from reset button to go into run mode

set arduino:
generic esp8266 module
upload speed 912600
flash size 4MB (FS:1MB) (for a esp12e)


note: to upload spiffs, arduino serial console must be closed



2/22/23:  use this for the usb driver: https://help.mictrack.com/articles/how-to-fix-pl2303hxa-phased-out-issue/

Upgrade PL2303 Driver
Right-click the “Windows Start” and select the“Device Manager”:
Click “Port (COM & LPT)”, right-click “PL2303HXA PHASED OUT…” ;
Select “Update driver”;
Click “Browse my computer for drivers“,
Click “Let me pick from a list of available drivers on my computer”
Click “10/27/2008” then click next;
Back to the “Port (COM & LPT)” and then it shows the COM Port
