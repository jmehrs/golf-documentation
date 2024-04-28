## Datasheet
- [Datasheet](https://www.espressif.com/sites/default/files/documentation/esp32-c3_datasheet_en.pdf) ^d965c4

## Features
- Wi-Fi
	- IEEE 802.11b/g/n-compliant
	- Supports 20 MHz, 40 MHz bandwidth in 2.4 GHz  band
	- 4 × virtual Wi-Fi interfaces
	- more... (see [[esp32c3#^d965c4|datasheet]])
- Bluetooth
	- Bluetooth 5
	- Bluetooth Low-Energy (LE)
	- Bluetooth mesh
	- High power mode (20 dBm)
	- Speed: 125 Kbps, 500 Kbps, 1 Mbps, 2 Mbps
	- more... (see [[esp32c3#^d965c4|datasheet]])
- CPU and Memory
	- 32-bit RISC-V single-core processor, up to 160 MHz
	- 400 KB SRAM (16 KB for cache)
	- 8 KB SRAM in RTC
	- more... (see [[esp32c3#^d965c4|datasheet]])
- Advanced Peripheral Interfaces
	- 22 or 15 programmable GPIOs
	- Digital interfaces:
		- 3 × SPI
		- 2 × UART
		- 1 × I2C
		- 1 × I2S
		- Remote control peripheral, with 2 transmit channels and 2 receive channels
		- LED PWM controller, with up to 6 channels
		- Full-speed USB Serial/JTAG controller
		- General DMA controller (GDMA), with 3 transmit channels and 3 receive channels
		- 1 × TWAI® controller compatible with ISO 11898-1 (CAN Specification 2.0)
	- Analog interfaces:
		- 2 × 12-bit SAR ADCs, up to 6 channels
		- 1 × temperature sensor
	- Timers:
		- 2 × 54-bit general-purpose timers
		- 3 × digital watchdog timers
		- 1 × analog watchdog timer
		- 1 × 52-bit system timer
- Power Management
	- Fine-resolution power control through a selection of clock frequency, duty cycle, Wi-Fi operating modes, and individual power control of internal components
	- more... (see [[esp32c3#^d965c4|datasheet]])
- Security
	- Secure boot - permission control on accessing internal and external memory
	- Flash encryption - memory encryption and decryption
	- more... (see [[esp32c3#^d965c4|datasheet]])
- RF Module
	- Antenna switches, RF balun, power amplifier, low-noise receive amplifier
	- Up to +21 dBm of power for an 802.11b transmission
	- Up to +20 dBm of power for an 802.11n transmission
	- Up to -105 dBm of sensitivity for Bluetooth LE receiver (125 Kbps)

## Electrical Characteristics
For more information, see [[esp32c3#^d965c4|datasheet]]
### Absolute Maximum Ratings
| Parameters       | Description                  | Min  | Max  | Unit |
| ---------------- | ---------------------------- | ---- | ---- | ---- |
| Input power pins | Allowed input voltage        | –0.3 | 3.6  | V    |
| $I_{output}$     | Cumulative IO output current | —    | 1000 | mA   |
| $T_{STORE}$      | Storage temperature          | –40  | 150  | °C   |
### Recommended Power Supply Characteristics
| Parameter                | Description               | Min | Typ | Max | Unit |
| ------------------------ | ------------------------- | --- | --- | --- | ---- |
| VDDA, VDD3P3, VDD3P3_RTC | Recommended input voltage | 3.0 | 3.3 | 3.6 | V    |
| VDD3P3_CPU               | Recommended input voltage | 3.0 | 3.3 | 3.6 | V    |
| VDD_SPI (as input)       | —                         | 3.0 | 3.3 | 3.6 | V    |
| $I_{VDD}$                | Cumulative input current  | 0.5 | —   | —   | A    |
### DC Characteristics (3.3V, 25 °C)
| Parameter | Description                                                               | Min         | Typ | Max         | Unit |
| --------- | ------------------------------------------------------------------------- | ----------- | --- | ----------- | ---- |
| $C_{IN}$       | Pin capacitance                                                           | —           | 2   | —           | pF   |
| $V_{IH}$       | High-level input voltage                                                  | 0.75 × VDD1 | —   | VDD1 + 0.3  | V    |
| $V_{IL}$       | Low-level input voltage                                                   | –0.3        | —   | 0.25 × VDD1 | V    |
| $I_{IH}$       | High-level input current                                                  | —           | —   | 50          | nA   |
| $I_{IL}$       | Low-level input current                                                   | —           | —   | 50          | nA   |
| $V_{OH}$       | 2 High-level output voltage                                               | 0.8 × VDD1  | —   | —           | V    |
| $V_{OL}$       | 2 Low-level output voltage                                                | —           | —   | 0.1 × VDD1  | V    |
| $I_{OH}$       | High-level source current (VDD1 = 3.3 V, VOH >= 2.64 V, PAD_DRIVER = 3)   | —           | 40  | —           | mA   |
| $I_{OL}$       | Low-level sink current (VDD1 = 3.3 V, VOL = 0.495 V, PAD_DRIVER = 3)      | —           | 28  | —           | mA   |
| $R_{PU}$      | Internal weak pull-up resistor                                            | —           | 45  | —           | kΩ   |
| $R_{PD}$       | Internal weak pull-down resistor                                          | —           | 45  | —           | kΩ   |
| $V_{IH_nRST}$  | Chip reset release voltage CHIP_EN voltage is within the specified range) | 0.75 × VDD1 | —   | VDD1 + 0.3  | V    |
| $V_{IL_nRST}$  | Chip reset voltage (CHIP_EN voltage is within the specified range)        | –0.3        | —   | 0.25 × VDD1 | V    |
### Current Consumption
#### RF Current Consumption in Active Mode
| TX/RX | Description                    | Peak (mA) |
| ----- | ------------------------------ | --------- |
| TX    | 802.11b, 1 Mbps, @21 dBm       | 335       |
| TX    | 802.11g, 54 Mbps, @19 dBm      | 285       |
| TX    | 802.11n, HT20, MCS7, @18.5 dBm | 276       |
| TX    | 802.11n, HT40, MCS7, @18.5 dBm | 278       |
| RX    | 802.11b/g/n, HT20              | 84        |
| RX    | 802.11n, HT40                  | 87        |
#### Current Consumption in Modem-sleep Mode
| CPU Frequency (MHz) | Description    | All Peripherals Clocks Disabled (mA) | All Peripherals Clocks Enabled (mA) | 
| ------------------- | -------------- | ------------------------------------ | ----------------------------------- |
| 160                 | CPU is running | 23                                   | 28                                  |
| 160                 | CPU is idle    | 16                                   | 21                                  |
| 80                  | CPU is running | 17                                   | 22                                  |
| 80                  | CPU is idle    | 13                                   | 18                                  |
#### Current Consumption in Low-Power Modes
| Mode        | Description                                                          | Peak ($\mu$A) |
| ----------- | -------------------------------------------------------------------- | ------------- |
| Light-sleep | VDD_SPI and Wi-Fi are powered down, and all GPIOs are high-impedance | 130           |
| Deep-sleep  | RTC timer + RTC memory                                               | 5             |
| Power off   | CHIP_EN is set to low level, the chip is powered off                 | 1             |
## Breakout Boards
- [esp32-c3 devkits](https://www.espressif.com/en/products/devkits#ESP32-C3)