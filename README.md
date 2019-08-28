# Hardware
Printed circuit boards used in NINscope were designed in KiCAD.
Check the wiki page for more info: https://github.com/ninscope/Hardware/wiki

:exclamation::exclamation: LabMaker is in the process of manufacturing the sensor and interface PCBs as a unit for sale. Please fill out the following form if you are interested in purchasing the PCBs through LabMaker: 

https://docs.google.com/forms/d/e/1FAIpQLSfAj43ocVpiAZvSG1-GbBokts9RmP8jfD8x3Ee3YmrGeCPbAg/viewform

### Printing material
We have 3D printed the microscope housing using an EnvisionTec Micro Plus Advantage printer with RCP-30 resin (requires coating afterwards) and Formlabs Form 2 printer using RS-F2-GPBK-04 black resin. 

### Assembly of optics

The assembly of optics resembles that of the first-gen. UCLA miniscope, with a few differences. First the emission and dichroic optical filters are 500 µm and therefore thinner and more fragile. The emission filter of 1000 µm thickness is glued on to the plano-convex lens with optical bonding glue (NOA81, Norland Products) and lowered into the lower half of the NINscope housing. 

For more details see: https://github.com/ninscope/Hardware/wiki/5.-Mechanical-assembly-NINscope

### Cleaning the CMOS sensor

In case of dust particles or other particulates dropping on the CMOS sensor one can use 'Sticky Swabs' (ideal-tek, https://www.ideal-tek.com/public/doc/Sticky-swabs-leaflet_Ideal-tek.pdf) to remove them without causing damage to the sensor.

### Computer requirements

We recommend using a laptop with SSD drive for respectively mobility and optimal disk write speeds. Despite this we have tested operating NINscope on a variety of systems including a MacBook Pro laptop running MacOS Mojave (R2015, i7, SSD), Mac Mini running MacOS High Sierra (R2014, i5, 5400 rpm HD), Dell PC Z240 running Windows 7(i7, NVMe SSD Samsung MZVLW256), a NUC7i5BNH running Windows 10 (i5, SSD Crucial MX500), a Linux Workstation running Ubuntu 18.04 (Intel Xeon, SSD) and a Dell PC OptiPlex 3050 SFF running Ubuntu 18.04 (i5, SSD).

### Interfacing to a PC

:warning:  A USB 3.0 port (on some PCs indicated by SS, SuperSpeed USB) is required to connect the modified UCLA DAQ (v3.2) to a PC, otherwise NINscope will not be recognized during installation.

### Webcams for behavioral monitoring

UVC-compliant USB webcams are supported. We have successfully tested Logitech webcams inlcuding the C920 HD pro cam. PS3 Eye webcams are currently not supported as they are not UVC-compliant.

### DAQ trigger and output port cables

SMA to BNC cables can be purchased directly, e.g.: https://nl.mouser.com/ProductDetail/Johnson-Cinch-Connectivity-Solutions/415-0028-048?qs=sGAEpiMZZMufBZYvsU%2Fbe5IX9y1Z%252BxjUbtuL98E%2Fl5g%3D.
This allows for triggering the acquisition with an external trigger, or logging the miniscope frames during acquisition.

### Note about setting the excitation LED current

:warning: Care is adviced when setting the curent to the excitation LED. Please note that low curernts (2.38-9.38 mA) provide sufficient light output (0.12-0.46 mW before GRIN objective) to perform imaging (in cortex and striatum respectively). Moreover, it is adviced to stay within the linear range of the LED driver (<35 mA). Be aware that driving a large current to the excitation LED in combination with optogenetic stimulation could lead to unexpected intensity drops during image acquisition. We have been succesful in our experiments using currents to the optogenetic LED of 11-33 mA and 2.38-9.38 mA to the excitation LED.
