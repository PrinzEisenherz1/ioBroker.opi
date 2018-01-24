![Logo](admin/admin.png)
# ioBroker.admin
===================
[![NPM version](http://img.shields.io/npm/v/iobroker.opi.svg)](https://www.npmjs.com/package/iobroker.opi)
[![Downloads](https://img.shields.io/npm/dm/iobroker.opi.svg)](https://www.npmjs.com/package/iobroker.opi)

[![NPM](https://nodei.co/npm/iobroker.opi.png?downloads=true)](https://nodei.co/npm/iobroker.opi/)

OPI-Monitor implementation for integration into ioBroker without GPIO`s.

## Important Information
Works only with node >= 0.12

** Tested Hardware: ** OrangePi plus2 H3

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

#### *CPU*
- cpu_frequency
- load1
- load5
- load15

#### *Memory*
- memory_available
- memory_free
- memory_total

#### *Network (eth0)*
- net_received
- net_send

#### *eMMC*
- emmc_root_total
- emmc_root_used

#### *Swap*
- swap_total
- swap_used

#### *Temperature*
- soc_temp

#### *Uptime*
- uptime

#### *WLAN*
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

## Changelog
### 0.1.0 (2018-01-24)
- Admin3 support.

### 0.0.6 (2017-08-01)
- stable release.

### 0.0.2 (2017-06-01)
- Initial release. Beta Version.


## License
Modified for OrangePi by Johnny Schneider <johann.schneider1@googlemail.com>

Copyright (c) 2015-2016 husky-koglhof <husky.koglhof@icloud.com>

MIT License
