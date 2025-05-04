# SiSeriesRadio
This project details the design and development of a Si4732/Si4735 based radio receiver utilizing a Raspberry Pi Pico for control and a custom-designed PCB
# SiRadioSeriesBorde - Open Source Si4732/Si4735 Radio with Raspberry Pi Pico Front End

[![License](https://img.shields.io/badge/License-Attribution%20Required-blue.svg)](LICENSE)
[![GitHub Issues](https://img.shields.io/github/issues/ecmastermind/SiRadioSeriesBorde)](https://github.com/ecmastermind/SiRadioSeriesBorde/issues)
[![GitHub Forks](https://img.shields.io/github/forks/ecmastermind/SiRadioSeriesBorde)](https://github.com/ecmastermind/SiRadioSeriesBorde/network/members)
[![GitHub Stars](https://img.shields.io/github/stars/ecmastermind/SiRadioSeriesBorde)](https://github.com/ecmastermind/SiRadioSeriesBorde/stargazers)

## Overview

The SiRadioSeriesBorde is a fully open-source hardware project for creating a versatile radio receiver based on the Silicon Labs Si4732 and Si4735 radio receiver ICs. This version 2.0 design builds upon a successful initial breakout board, incorporating a dedicated Raspberry Pi Pico-driven front-end user interface. The hardware is thoughtfully divided into three separate boards for ease of assembly, troubleshooting, and potential future expansion. This design allows for direct replacement and easy upgrading of existing Si series radio cards with a modified pin configuration optimized for the Raspberry Pi Pico, replacing previous ESP32 implementations.

## Key Features

* **Si4732/Si4735 Radio Receiver:** Supports reception of AM, FM, and SW bands (depending on the specific Si47xx chip used).
* **Raspberry Pi Pico Front End:** Provides a powerful and flexible platform for controlling the radio and displaying information.
* **Dedicated Power Supply Circuit:** Ensures stable and reliable power for the radio and front-end components.
* **Dual 0.96 inch OLED Displays:** Offers clear and simultaneous display of radio information.
* **SPI Display Header:** Provides an alternative interface for connecting displays.
* **5 Input Switches:** Allows for user interaction and control of radio functions.
* **Rotary Encoder:** Enables precise tuning and menu navigation.
* **Three Separate Boards:**
    * **Radio Card:** Houses the Si4732/Si4735 receiver IC and essential passive components. Designed for easy replacement and upgrade of Si series radio cards.
    * **Front End UI Board:** Contains the Raspberry Pi Pico, OLED displays, switches, rotary encoder, and display header.
    * **Interconnect/Power Board:** Provides power distribution and interconnects the Radio Card and Front End UI Board.
* **3.5mm Audio Jack Output:** Standard audio output for headphones or external speakers.
* **Onboard I2S Expansion Ports:** Allows for digital audio output and potential integration with external audio processing.
* **Open Source Hardware:** All design files and documentation are publicly available.

## Board Descriptions

This project comprises three distinct PCB boards:

1.  **Radio Card (Si4732/Si4735 Board):**
    * Contains the Si4732 or Si4735 radio receiver IC.
    * Includes necessary passive components for the radio circuit (e.g., filtering capacitors, inductors).
    * Features a connector designed for direct attachment to the Interconnect/Power Board.
    * Pin configuration is specifically adapted for the Raspberry Pi Pico interface, replacing previous ESP32 designs.

2.  **Front End UI Board (RPi Pico Board):**
    * Houses the Raspberry Pi Pico microcontroller.
    * Integrates dual 0.96 inch OLED displays.
    * Provides connections for the 5 input switches and the rotary encoder.
    * Includes an SPI header for alternative display options.
    * Connects to the Interconnect/Power Board for power and control signals to the Radio Card.

3.  **Interconnect/Power Board:**
    * Provides a centralized power distribution network for all boards.
    * Facilitates the electrical connection between the Radio Card and the Front End UI Board.
    * May include voltage regulation circuitry to ensure proper power delivery.
    * Offers easy connection points for an external power source.

## Hardware Files

This repository contains the hardware design files for each of the three boards, including:

* **RadioCard/:** (e.g., Schematic, PCB layout in KiCad, Eagle, etc.)
* **FrontEndUIBoard/:** (e.g., Schematic, PCB layout in KiCad, Eagle, etc.)
* **InterconnectPowerBoard/:** (e.g., Schematic, PCB layout in KiCad, Eagle, etc.)
* **GerberFiles/:** (Generated manufacturing files for each board)
* **BOM/:** (Bill of Materials for each board)

## Software

The software for the Raspberry Pi Pico front end is currently under development and will be available in a separate directory or linked repository upon completion. The software will be responsible for:

* Interfacing with the Si4732/Si4735 radio receiver via I2C.
* Reading input from the switches and rotary encoder.
* Controlling and displaying information on the dual OLED displays.
* Potentially implementing features like scanning, presets, and more.

## Getting Started

To get started with this project:

1.  **Explore the Hardware Files:** Familiarize yourself with the schematics and PCB layouts of the three boards.
2.  **Review the Bill of Materials (BOM):** Understand the components required for each board.
3.  **Generate and Order PCBs:** Use the provided Gerber files to order the PCBs from a manufacturer.
4.  **Source Components:** Obtain all the necessary electronic components listed in the BOM.
5.  **Assemble the Boards:** Carefully solder the components onto the respective PCBs.
6.  **Connect the Boards:** Connect the three boards together as intended in the design.
7.  **Software (Coming Soon):** Once the software is available, upload it to the Raspberry Pi Pico to bring the radio to life.

## Contributing

Contributions to this open-source project are welcome! If you have ideas for improvements, bug fixes, or new features, please feel free to:

* **Fork the repository** and create a branch for your changes.
* **Submit a pull request** with a clear description of your modifications.
* **Open an issue** to report bugs or suggest enhancements.

## License

This project is licensed under the **Attribution Required** license. This means that you are free to use, modify, and distribute the hardware design, but you **must give appropriate credit** to the original author(s) (ecmastermind). Please include a clear attribution in any derivative works or projects based on this design. See the [LICENSE](LICENSE) file for more details.

## Acknowledgements

We would like to thank the open-source community for their valuable contributions and resources that have made this project possible.

## Contact

For any questions or inquiries, please feel free to contact [your contact information here, e.g., email, GitHub profile].

**SiRadioSeriesBorde by ecmastermind - Fully Open Source. Attribution Required.**
