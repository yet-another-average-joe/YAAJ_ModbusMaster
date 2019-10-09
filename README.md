# YAAJ_ModbusMaster

This Arduino library was forked from https://github.com/4-20ma/ModbusMaster

As is, this great library does *NOT* comply the MODBUS specification, and cannot without editing deep in the code : the T1.5 and T3.5 delays/timeouts are not implemented.

mods :

- added T1.5 and T3.5 support
- support for HardwareSerial *ONLY*
- removed the hungarian notation (not needed anymore nowadays)
- renamed many member functions and attributes for better readability
- removed all the comments for auto generated documentation (everything is self explanative)
- replaced constexpr with #define (as a Visual Studio user, #define gives better readability than constexpr with IntelliSense)

Tested with STM32 as master, Schneider Telemecanique Altivar VFD + Arduino Nanos running SimpleModbusSlave library.

