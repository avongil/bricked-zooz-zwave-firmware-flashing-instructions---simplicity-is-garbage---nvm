# bricked-zooz-zwave-firmware-flashing-instructions---simplicity-is-garbage---nvm
The official Zooz method for flashing the firmware is absolute rubbish.  Simplicity simply does not work. It will burn up hours of your time and end up in failure.
nvm is quick and simple.


Instructions on how to flash a Zooz Z-Wave with nvm-windows

Install nvm.  In windows you can use winget in powershell opened as admin.  
* winget install nvm-windows

nvm install latest
nvm list
nvm use xx.x.x  (use a version listed)

In a comand prompt, navigate to your firmware. Unzip and locate the .gbl file.
* npx @zwave-js/flash@latest COMxx Zooz_xxx.gbl --verbose   (figure out what COM port it is on via the device manager)
