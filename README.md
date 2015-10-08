# Zatar's Raspberry Pi / Pibrella Example Device
This project aims to help you get a simple, well known device working with Zatar (http://zatar.com) as quickly and effortlessly as possible.

This repository contains the files required for the Raspberry Pi Development kit walkthroughs described at developers.zatar.com.

The structure of this repository is as follows:


**zatar-rpi-iotkit-java.jar** - a Java file that when run on a Raspberry Pi with a Pibrella daughter board on it connects to Zatar and lets a developer interact with the Pibrella peripherals remotely through the Zatar Device Portal.
**agent.properties** - a configuration file that is used by the zatar-rpi-iotkit-java.jar file


Out of the Box Demo Instructions

1. Connect the Pibrella daughter board to your Raspberry Pi
2. On your Raspberry Pi clone this repository.
`git clone "this repository's URL"`
3. Go into the folder of the new repository. Run the .jar file. You'll need to include the configuration file as an argument.
`sudo java -jar zatar-rpi-iotkit-java.jar agent.properties`
Take note of the serial number displayed. This will be needed in a future step.
4. In a browser go to api.zatar.com (create an account if necessary). Its recommended you do this on another machine.
5. Add a device to your world in Zatar. Enter the serial number from step 4 including all leading zeroes. If necessary continue the Add Device Wizard instructions

Your Pibrella/Raspberry Pi should now be accessible in Zatar. Change settings to set the state of the LEDs. Push the button on the Pibrella board and see the state change in Zatar.
