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

# Table of contents

- [Overview](#overview)
- [Features](#features)
- [Requirements](#requirements)
- [Configuration](#configuration)
- [Data points](#data-points)
- [Example object structure](#example-object-structure)
- [Troubleshooting](#troubleshooting)
- [Development](#development)
- [License](#license)

---

# Overview

This adapter connects ioBroker with a **Klipper based 3D printer** via the **Moonraker API**.

Moonraker acts as the communication interface between Klipper and external systems such as:

- Mainsail
- Fluidd
- ioBroker
- Home automation systems

The adapter retrieves printer information and exposes them as **ioBroker states**.

---

# Features

- Connection to Moonraker API
- Access to Klipper printer objects
- Automatic state creation
- Access to printer telemetry
- Integration into ioBroker automation

Examples:

- Monitor printer status
- Track bed mesh values
- Monitor current consumption
- Trigger automations when a print finishes

---

# Requirements

- Node.js ≥ 18
- ioBroker
- Klipper
- Moonraker API

Typical setup:
