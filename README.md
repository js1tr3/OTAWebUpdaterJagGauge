# OTAWebUpdaterJagGauge
Jaguar Megasquirt Tachometer Gauge
Moving coil meter, control of Smiths gauge form ESP32 Cam Thinker module.
Can Transciever to Megasquirt.


GPIO 0 determines whether the ESP32 is in flashing mode or not. This GPIO is internally connected to a pull-up 10k Ohm resistor.
GPIO 33 – Built-in Red LED

MicroSD card	ESP32
CLK	GPIO 14
CMD	GPIO 15
DATA0	GPIO 2
DATA1 / flashlight	GPIO 4 ( could unsolder the LED and re-use the pin for driving the tachometer?)
DATA2	GPIO 12 --- use for can TX
DATA3	GPIO 13 --- use for can RX

GPIO 1 and GPIO 3 are the serial pins (TX and RX, respectively). Because the ESP32-CAM doesn’t have a built-in programmer, you need to use these pins to communicate with the board and upload code. 
