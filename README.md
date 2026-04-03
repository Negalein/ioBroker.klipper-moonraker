![Logo](admin/klipper-moonraker.png)
# ioBroker.klipper-moonraker


![Number of Installations](https://iobroker.live/badges/klipper-moonraker-installed.svg)
![Stable version](https://iobroker.live/badges/klipper-moonraker-stable.svg)
![NPM version](https://img.shields.io/npm/v/iobroker.klipper-moonraker.svg)
![Downloads](https://img.shields.io/npm/dm/iobroker.klipper-moonraker.svg)
![Node](https://img.shields.io/badge/node-%3E%3D18-green)
![License](https://img.shields.io/github/license/DrozmotiX/ioBroker.klipper-moonraker)

ioBroker adapter to interact with **Klipper** via the **Moonraker API**

This adapter allows integration of **Klipper based 3D printers** into **ioBroker** using the Moonraker API.

---

## Table of contents

- Overview
- Features
- Requirements
- Configuration
- Data points
- Example object structure
- Troubleshooting
- Development
- License

---

## Overview

This adapter connects ioBroker with a **Klipper based 3D printer** via the **Moonraker API**.

Moonraker acts as the communication interface between Klipper and external systems.

---

## Features

- Connection to Moonraker API
- Access to Klipper printer objects
- Automatic state creation
- Access to printer telemetry
- Integration into ioBroker automation

---

## Requirements

- Node.js ≥ 18
- ioBroker
- Klipper
- Moonraker API

---

## Configuration

| Setting | Example |
|--------|--------|
| Host   | 192.168.1.100 |
| Port   | 7125 |
| Protocol | http |

Test:
http://PRINTER-IP:7125/server/info

---

## Data points

All states are created under:

klipper-moonraker.0

---

## Example object structure

klipper-moonraker.0.adc_current_sensor.current
klipper-moonraker.0.auto_screws_tilt_adjust.adjust_tolerance
klipper-moonraker.0.bed_mesh.mesh_matrix

---

## Troubleshooting

Check Moonraker:
http://PRINTER-IP:7125/server/info

Check logs:
iobroker logs

---

## Development

https://github.com/DrozmotiX/ioBroker.klipper-moonraker

---

## License

MIT License


The Testclient was created with Kiauh. Kiauh is a Script that help you creating a perfect environment for your Klipper Setup.

Kiauh: 
https://github.com/th33xitus/kiauh

    
## Changelog

<!--
    Placeholder for the next version (at the beginning of the line):
    ### __WORK IN PROGRESS__
-->
### 0.1.1 (2025-05-07)
* (@foxriver76) detect stale connections

### 0.1.0 (2024-04-22)
* IMPORTANT: The adapter requires Node.js 18.x+
* (foxriver76) added state to run custom GCODE commands
* (foxriver76) added possiblity to use authentication
* (foxriver76) corrected some state definitions
* (foxriver76) ported UI to json config

### 0.0.4 (2021-03-17)
* (DutchmanNL) Implemented rounding of digits
* (DutchmanNL) Transfer ownership to DrozmotiX
* (DutchmanNL) Improve automerge for dependency updates
* (Basti-RX) Update state attribute relations

### 0.0.3 (2021-01-07)
* (DutchmanNL) Switch from data-polling to live socket events :-)
* (DutchmanNL) Ensure all states and objects available are created
* (DutchmanNL) reconnect if connection closes (retry after 10 sec, ToDo : make adjustable)

### 0.0.2 (2021-01-05)
* (DutchmanNL) Implement control commands
* (DutchmanNL) Proper error handling for API calls
* (DutchmanNL) update state attributes for control commands

### 0.0.1
* (DutchmanNL) initial release

## License
MIT License

Copyright (c) 2020-2025 DutchmanNL <rdrozda@hotmail.com>

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
