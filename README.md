# Web Device CLI for Frodo

A Web Command Line Interface for Frodo via NUS (Nordic UART Service) using [Web
Bluetooth](https://webbluetoothcg.github.io/web-bluetooth/).

[![](img/web-device-cli-chrome-desktop.png)](https://youtu.be/i6OgX4civrM)

The website loads javascript code provide you with a Browser Terminal that uses
your local computer's Bluetooth adapter to connect to Frodo. All of this without
installing any extra software!

This project is based on a fork of the Web Device CLI from
[https://github.com/makerdiary/web-device-cli]. Apart from changing the look and
feel of the terminal it adds some minor fix so the backspace key is correctly
transmitted to the Nordic CLI component via BLE NUS.

## Prerequisites
* Frodo flashed with some reccent firmware.
* A browser that supports Web Bluetooth. At the time of writing Google Chrome on
Windows is the only Browser that supports it out of the box. On Linux Google
Chrome can be configured (with som experimental feature flag) to enable Web
Bluetooth as well.
* A Computer with a Bluetooth Transceiver i.e. any modern Laptop (or just by
  some cheap Bluetooth USB dongle that support BLE).

## How to Use the CLI
You can immediately start to use the Web CLI as this repository is live hosted under the following URL:

**[https://meggiman.github.io/frodo_cli](https://meggiman.github.io/frodo_cli)**

Open the URL, hit connect in the upper left corner. If your Browser supports Web
Bluetooth you will see a small Pop-up window with nearby bluetooth low energy
devices. Search the list for the entry "Frodo" and click connect. Your browser
will connect to Frodo and you can immediately start interacting with it via the
console. 

Enter `help` <kbd>Enter</kbd> to list the most important available commands. Use
tab completion to quickly enter commands with auto-complete. Most commands are
documented and its documentation can be shown by entering the command followed
by `-h` (e.g. `bioz config_meas -h`).

## MIT License

Copyright (c) 2019 makerdiary

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
