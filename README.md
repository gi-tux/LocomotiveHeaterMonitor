# LocomotiveHeaterMonitor
This is a project to build a monitor system for a locomotive heater built from a pool heater for a railroad.

The application will be built using a Raspberry Pi and the Python programming language.  The application will run when the Pi is booted and will automatically start the monitoring function based upon temperature differences in air temperature and output temperature.  The temperature readings will come from DS18B20 sensors.  The temperature will be read every five seconds and twelve consequative readings can cause an alert to be sent.

The system will alert users via email when certain criteria are reached.  An alert will continue to be sent at a regular interval until one of the users acknowledges the alert.  The application will provide a way to cease alerts once they have been tiggered and acknowledged.  The alert will contain the temperature readings for all of the sensors but will indicate which sensor triggered the alert.

The system will need to monitor the air temperature as well as the input temperature of the water lines to the locomotives and output temperature of the water lines from each of two locomotives.  This will mean that four temperature sensors will need to be monitored.

Once the ouput temperature of the water lines from each locomotive raises above 90 degrees F, monitoring will begin.  If the output temperature or the input temperature falls below 90 degrees F after this point the alert decision will need to be made.  If the air temperature falls below 30 degrees F, an alert will also need to be raised.
