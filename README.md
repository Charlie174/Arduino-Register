## Arduino-Register
Increase the Arduino pins using shift registers (74HC595).

With register pins ST_CP, SH_CP, DS, we can controll 8 bit with that register. Unique function call ShiftOut(DS_pin,SH_CP_pin,MSBFIRST,number). Before that function storage must be cleared using ST_CP low.
OE pin, GND should be connect to ground.
MR pin, VCC shold be connect to +5V
for one register Serial out pin wthout any connection that will used to connect other registers.


# with many registers
same as earlier in one register but for data input DS pin we must connect, 1st register's serial out pin (pin_9)
