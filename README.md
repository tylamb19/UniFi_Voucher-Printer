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

You will need to provide Network-Image.bmp, regular-font.ttf, and bold-font.ttf for the service to function. 
All of these files should be placed in the same folder as your .py files.

Network-Image.bmp should be 250px maximum in any dimension, 1 bit bitmap.
regular-font.ttf and bold-font.ttf should be full character set truetype fonts, readable by libfreetype. 
Your PrintVoucher folder should look something like the following with a fully functional install:

*****************************************************************************
```
pi_admin@piprint:~/PrintVoucher $ ls
 bold-font.ttf   LICENSE                      __pycache__        UnifiAPI.py
 img-tmp.png    'linux helper commands.txt'   README.md          venv
 lg              Network-Image.bmp            regular-font.ttf
 lg.zip          Print.py                     requirements.txt
pi_admin@piprint:~/PrintVoucher $
```
*****************************************************************************
