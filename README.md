# OctoPi_GUI_Setup

A quick and easy guide to setting up OctoPi for beginners with zero experience. Follow these steps to setup OctoPi OS on your Raspberry Pi in a few basic steps regardless of your machine's operating system.

(Insert OctoPi Image)

So what exactly is OctoPrint? Here is a list of things OctoPrint allows you to do:

* Wirelessly upload G-code files from a computer to a 3D printer
* Manually control a 3D printer (moving the X-, Y-, and Z-axes as well as forcing extrusion)
* Monitor print temperature and change print settings
* Set up a webcam to view the Print in real time and create time lapse videos
* Slice models using CuraEngine
* Customize operation with numerous plug-ins

## Installation

### Hardware Prerequisites:

* Raspberry Pi (Model 3B or later, Raspberry Pi Zero/Zero W not recommended)
* 5.1V/2.5 A Micro USB power supply (For the RPi)
* MicroSD card (preferably 16GB or larger)
* MicroSD card reader
* USB Mouse and Keyboard
* HDMI Monitor
* Stable WiFi
* Desktop/Laptop

### Preparing the MicroSD Card:

* Download the latest image of OctoPi from
https://octoprint.org/download/

(Insert Download Page Image)

* Next download an etching tool:
https://www.balena.io/etcher/

(Insert Download Page Image)

* Insert the MicroSD card into the MicroSD card reader and connect it to your machine.

* Format the MicroSD card (FAT32 formatting only)

* Using Etcher, flash the disk image of the OctoPi OS onto the MicroSD card

* Once the flashing is complete, insert the MicroSD card into the Raspberry Pi

### Setting up the Raspberry Pi:

* Connect the Raspberry Pi to the monitor, mouse and the keyboard and power it up.

* Your Raspberry Pi will boot up automatically.

* After the boot is complete, you will see the following:

(picture of octopi login)

* octopi login: pi
* Password : raspberry

* You are now sucessfully logged in!

### Enable GUI:

* Enter the following commands into the bash terminal:

sudo raspi-config

* Re-enter the password.

* Use the arrow keys to navigate to "Network Options"

(Insert Picture)

* Select "N2 Wi-fi"

(Insert Picture)

* Enter the SSID (Name of your Wifi network), and click "<Ok>".
* Enter the password of the Wifi (if none, leave blank), and click "<Ok>".

* Click "<Finish>"

* You are now back in the bash command line.

* Enter:

sudo /home/pi/scripts/install-desktop

* Enter the password, press any key to continue.

* You will be asked whether you want the Pi to boot up into a desktop environment by default. Type ‘yes’. We can disable this functionality later on if we want to.

(Add picture)

* The resources for the desktop GUI will now download and install automatically
* When complete, Type: 

sudo reboot

* The Pi will now reboot to OctoPi Desktop GUI.

* Enter the username and password.

(Insert picture)

* Your OctoPi GUI is now ready!

(Insert Picture)

## Next: How to enable remote access to OctoPi using VNC, control your 3D printer remotely:

* (Link)

## Meta

Harshit Shandilya (https://www.linkedin.com/in/harshitshandilya/

Distributed under the MagPi License: CC BY-NC-SA license. See ``LICENSE`` for more information.

https://github.com/shandilyaguy247

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b`)
3. Commit your changes (`git commit -am)
4. Push to the branch (`git push origin)
5. Create a new Pull Request
6. For major changes, please open an issue first to discuss what you would like to change.
