# BarbelMotionTracker

This git project is dedicated to a prototype implementation that attempts to track and evaluate the motion of a barbell in the gym.

## 3D-Files

Here you will find the FFF (FDM) printable files for a case for the board. All STL-files are in metric (mm). To complete the assembly you will need some additional hardware (M3 screws, rubber pad, M3 heat set inserts, 4mmx0.5mm brass tubing, 2cm wide velcro strap)

## PCB_Design

Here you will find the KiCad8.0 design files as well as the pre exported gerbers (ready to order at JLCPCB). You will also find the ibom.html file which is a Interactive Bill Of Materials that you can open in any modern browser. It is of great use when doing board smd assembly.

## Software-BarbelMotionTracker

Here you will find a PlatformIO project that contains the software running on the board. It is written in C/C++ for the esp32 platform using the arduino framework.

To get started install VSCode, install the PlatformIO extension plug in the board using the USB-C shared power and data port and make sure the board is turned on using the power switch.

The software collects all the raw sensor data into a CSV-File for future of board processing.

### Micro SD-Card

The sd-card has to be formatted as FAT32. FAT32 is only supported by micro-sd-cards with capacity less than 32GB.
The sd-card has to contain a settings.txt file that has to be populated. Check the sdcard.h code for details.