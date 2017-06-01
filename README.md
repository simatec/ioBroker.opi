![Logo](admin/opi.png)
ioBroker OPI-Monitor Adapter
==============

[![NPM version](http://img.shields.io/npm/v/iobroker.opi.svg)](https://www.npmjs.com/package/iobroker.opi)
[![Downloads](https://img.shields.io/npm/dm/iobroker.opi.svg)](https://www.npmjs.com/package/iobroker.opi)

[![NPM](https://nodei.co/npm/iobroker.opi.png?downloads=true)](https://nodei.co/npm/iobroker.opi/)

OPI-Monitor implementation for integration into ioBroker without GPIO`s.

## Important Information
Works only with node >= 0.12


## Installation
After installation you have to configure all required modules via administration page.

After start of iobroker.opi, all selected modules generates
an object tree in ioBroker within opi.<instance>.<modulename>
e.g. opi.0.cpu

Be sure, that python and build-essential are installed:

```
sudo apt-get update
sudo apt-get install -y build-essential python
```

Following Objects are available after selection:

#### **CPU**
- cpu_frequency
- load1
- load5
- load15

#### **Memory**
- memory_available
- memory_free
- memory_total

#### **Network (eth0)**
- net_received
- net_send

#### **eMMC**
- emmc_root_total
- emmc_root_used

#### **Swap**
- swap_total
- swap_used

#### **Temperature**
- soc_temp

#### **Uptime**
- uptime

#### **WLAN**
- wifi_received
- wifi_send

## Configuration
On configuration page you can select following modules:

- CPU
- Memory
- Network
- eMMC
- Swap
- Temperature
- Uptime
- WLAN

## Logfiles / Configuration Settings

## Features

## Todo

## Tested Hardware
 - OrangePi plus2 H3

## Changelog

### 0.0.2 (2017-06-01)
 - removed GPIO`s. Alpha Version.

### 0.0.1 (2017-06-01)
 - Initial release. Alpha Version.

## License

Copyright (c) 2015-2016 husky-koglhof <husky.koglhof@icloud.com>

MIT License
