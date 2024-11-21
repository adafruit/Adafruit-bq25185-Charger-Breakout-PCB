## Adafruit bq25185 USB / DC / Solar Lithium Ion/Polymer Charger PCB

<a href="http://www.adafruit.com/products/6091"><img src="assets/6091.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit bq25185 USB / DC / Solar Lithium Ion/Polymer Charger. 

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/6091

### Description

We're always on the look out for better ways to make projects portable: being able to charge your battery in the most convenient manner will let projects run no matter what power is available. The Adafruit bq25185 USB / DC / Solar Charger Board uses the new bq25185 is a nifty charger chip which has a lot of flexibility for different kinds of batteries (LiPoly, LiIon or LiFePO4), charging rates (250mA, 500mA, or 1A) and power sources (USB, DC or solar). It's also a great value, so it's a good upgrade from MCP73833 or MCP73831-based charger boards.

To let folks really explore what this chip can do, we made a basic breakout board with all the things we find most useful: two ways to power/charge including a solar-friendly DC input, adjustable current and voltage, power path management, and status and control I/O.

* USB Type C connector with 5.1k CC resistors so it will work with any computer or power supply to get 5V and up to 1A
* Separate DC or Solar Input - Two pads on the side can be used to connect a 5 ~ 18V power supply, which can be used instead of USB. If the input is a solar panel, the charging chip will adjust the current draw so that the voltage does not dip below the battery, thus optimizing the solar power input. No large capacitor needed to stabilize it, and you get near-MPPT capability without the cost and complexity of MPPT.
* Default charge rate of 1A, but you can cut the IS jumper on the front and solder either jumper on the back to set the rate to 500mA or 250mA
* Default 3.7V nominal / 4.2V max battery chemistry/voltage for all modern 1-cell LiPoly or LiIon batteries. You can set this to 3.2V / 3.65V for LiFePO4 batteries by cutting the VS jumper on the front and soldering a jumper on the back
* Power Path to Load - If the load connector is drawing current while the USB / DC/Solar power is attached, it will default to drawing current from the charger and any left over current will go to the battery. That keeps your battery from constantly charging/discharging which will reduce the battery life. The max draw from USB / DC / Solar is still 1A, if you need more current it will come from the battery and the chip can provide up to 3A current spikes from the battery to the load output!
* Regulated 4.5V-max Load Output - no matter what voltage you have on the USB or DC / solar inputs, the Load output port will never go above 4.5V due to an internal voltage regulator. Keep this in mind, though, when dealing with high currents and high DC voltages as the LDO will make the board start to overheat and throttle the current.
* Three Status LEDs - Orange Charging LED, red Fault LED, and Green Power Good LED. The charge/fault pins are also available on the left side breakout pads.
* Thermistor - cut the TH trace and you can connect a 10K thermistor to the TH pad which will adjust the charge rate to keep the battery from overheating.
* Chip Enable to disable the charger.
* Mounting holes!

This board is pretty much plug-and-play. Change any jumpers you like and then connect your battery to the BATT port, and the LOAD goes to your circuit. Don't forget the LOAD will never go above 4.5V, but it can go as low as 3.0V if the battery is nearly empty. You can monitor the voltage on the battery and load via the secondary pads on the right side, if necessary.

To use with solar, pick up a 5~7V solar panel, and either cut the connector off to wire it directly, or use a 2.1mm adapter cable plus a 2.1mm terminal block to get two wires for the DC Input port.

If you need a board with higher charge current or a DC plug already on-board, check out the bq24074 which has up to 1.5A charge rate and a on-board 2.1mm DC jack.

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. 
See license.txt for additional details.
