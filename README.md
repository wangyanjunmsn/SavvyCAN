# SavvyCAN
QT based cross platform canbus tool 
(C) 2015-2016 EVTV and Collin Kidder

A QT5 based cross platform tool which can be used to load, save, and capture canbus frames.
This tool is designed to help with visualization, reverse engineering, debugging, and
capturing of canbus frames.

Really requires at a resolution of at least 1024x768. Fully multi-monitor capable.

You are highly recommended to use the CANDue board from EVTV:
(http://store.evtv.me/proddetail.php?prod=ArduinoDueCANBUS&cat=23)

The CANDue board must be running the GVRET firmware which can also be found
within the collin80 repos.

It is very soon to be possible to use any SocketCAN compatible device
under LINUX. There may, however, be some loss of some functionality as
some functions of SavvyCAN are designed for use directly with the
EVTVDue and CANDue 2.0 boards.

It should, however, be noted that use of a capture device is not required to make use
of this program. It can load and save in several formats:

1. BusMaster log file

2. Microchip log file

3. CRTD format (OVMS log file format from Mark Webb-Johnson)

4. GVRET native format

5. Generic CSV file (ID,D0 D1 D2 D3 D4 D5 D6 D7)

6. Vector Trace files

7. IXXAT Minilog files

8. CAN-DO Logs

9. Vehicle Spy log files

Requires QScintilla library available at:

https://www.riverbankcomputing.com/software/qscintilla/download

Also uses QCustomPlot available at:

http://www.qcustomplot.com/ 

However, this source code is integrated into the source for SavvyCAN and one isn't required to download it separately.

The project now requires (yes, requires) at least QT 5.6.0 because of
a dependency on QtSerialBus which is still an optional feature. You
will need to download it when installing QT.