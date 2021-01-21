# RTC-set
Extremely basic ODROID-GO firmware file for setting DS3231M RTC.

## How to Use

1) Put the .fw file on your microSD card under odroid/firmware.
2) Connect the ODROID-GO to your PC via USB.
3) Open the Arduino Serial Monitor (or any other one capable of sending data) at 192600 baudrate.
4) Boot the .fw from the bootloader menu, accessible by holding down the B button while switching the system on.  You should now see messages printed in the serial terminal.
5) Send the command "SETDATE yyyy-mm-dd hh:mm:ss", where:

  - yyyy = year
  - mm = month
  - dd = day
  - hh = hour (24-hour format)
  - mm = minute
  - ss = second
  
  So, for example, you could send the command "2021-01-21 18:08:15" to set the time to January 21, 2021 at 6:08:15 PM.
  
  After sending the command, the monitor should send back messages counting up from the time you set.
