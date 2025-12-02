# UniFi - Voucher Receipt Printer

**Parts List**

 * Printer - Epson TM-T20III (also tested with TM-T88IV, if printer is changed, you will need to make requisite USB ID and escpos profile changes)
	* https://www.amazon.com/dp/B07YLSTMCX
 * High quality thermal paper
 	* https://www.amazon.com/dp/B0CM7NWNBM?ref=fed_asin_title
 * Pi - Raspberry Pi Zero 2W (Running Raspbian 13)
	* https://www.adafruit.com/product/6008
 * Button
	* https://www.adafruit.com/product/481
 * Step Down Regulator (to power Pi from printer power supply)
 	* https://www.pololu.com/product/4892

Button connected to GPIO 17
LED ring connected to GPIO 18

**Notes**

* This fork is re-written to support UniFi consoles such as the UDM Pro.
* Updated linux install based on Raspbian 13 on a Pi Zero 2 W
* Follow steps in Linux Helper Commands text file to install and run.

You will need to provide Network-Image.bmp for the service to function. This image should be placed in the same folder as your .py files. It should be 250px maximum in any dimension, 1 bit bitmap.
