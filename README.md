# Zatar-Pibrella-Example
This project aims to help you get a simple, well known device working with Zatar (http://zatar.com) as quickly and effortlessly as possible.

This repository contains the files required for the Raspberry Pi Development kit walkthroughs described at developers.zatar.com.

The structure of this repository is as follows:

**rpi.properties** - a configuration file that is used by the sample .jar file
**rpi_devkit.jar** - a Java file that when run on a Raspberry Pi with a Pibrella daughter board on it connects to Zatar and lets a developer interact with the Pibrella peripherals remotely through the Zatar Device Portal.

Project Folders 1 thru 5 - The provided Java file and configuration file is all you need to connect the device. But that's not very instructional. Each Project Folder contains code that guides you down a path of making the Pibrella Zatar Dev kit dance the way you want it to.

Project 1, ADD A DEVICE SETTING - This project provides you with the capability to control 2 of the 3 LEDs on the Pibrella. Your job is to follow the instructions and add the capability of controlling the 3rd LED.

Project 2, ADD A DEVICE SENSOR - This project provides you with the capability of sensing some items on the Raspberry Pi. Your job is to follow the instructions and add the capability for the device to report additional sensors to Zatar.

Project 3, ADD A COMMAND - This project comes with sample code that that implements the ability for a remote application to trigger the LEDs to flash a given number of times.

Project 4, ADD DEVICE INFO DATA - This project comes with sample code that allows the device to report some Device Info. Your task is to add additional items of Device Info data the Raspberry Pi reports up to Zatar.

Out of the Box Demo Instructions

1. Connect the Pibrella daughter board to your Raspberry Pi
2. On your Raspberry Pi clone this repository.
`git clone "this repository's URL"`
3. Go into the folder of the new repository. Run the sample out-of-the-box demo device agent. You'll need to include the configuration file as an argument.
`sudo java -jar rpi_devkit.jar rpi.properties`
Take note of the serial number displayed. This will be needed in a future step.
4. In a browser go to api.zatar.com (create an account if necessary). Its recommended you do this on another machine.
5. Add a device to your world in Zatar. Enter the serial number from step 4 including all leading zeroes. If necessary continue the Add Device Wizard instructions

Your Pibrella/Raspberry Pi should now be accessible in Zatar. Change settings to set the state of the LEDs. Push the button on the Pibrella board and see the state change in Zatar.

