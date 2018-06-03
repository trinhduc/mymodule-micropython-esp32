# mymodule-micropython-esp32

I'm using ubuntu for this project.

## Setting up the toolchain and ESP-IDF

(1) Can follow the **Setting up the toolchain and ESP-IDF** at [MicroPython port to the ESP32](https://github.com/micropython/micropython/tree/master/ports/esp32)

(2) Then follow the document **Adding a Module** at [MicroPython Development Documentation](http://micropython-dev-docs.readthedocs.io/en/latest/adding-module.html#adding-your-own-source-file)

(3) You can get a prompt via the serial port with **minicom**

* (3.1) Install Minicom

	```
	sudo apt-get install minicom
	```

* (3.2) Setup minicom: setting using port minicom same as in Makefile at section (1), with command and choose in image below 

	```
	sudo minicom -s
	```

	[setup-minicom](assets/setup-minicom.png)

	After save config.

	`Note`: `F - Hardware Flow Control`, and `G - Software Flow Control` both choose: `No`.

* (3.3) Jump to section **Building the firmware** at [MicroPython port to the ESP32](https://github.com/micropython/micropython/tree/master/ports/esp32)

* (3.4) Getting a Python prompt with minicom

	```
	sudo minicom -b /dev/ttyUSB0
	```

	[first-into-minicom](assets/first-into-minicom.png)

	Hit enter:

	[enter-for-see](assets/enter-for-see.png)

	[hit-name-your-module](assets/hit-name-your-module.png)
