<p align="center">
    <img src="assets/albion-stats-icon.png" width="100"> 
</p>

Linux and OS X Build Status: [![Linux and OS X Build Status](https://api.travis-ci.org/mazurwiktor/albion-online-stats.svg)](https://travis-ci.org/mazurwiktor/albion-online-stats)

Windows Build Status: [![Windows Build Status](https://ci.appveyor.com/api/projects/status/jx445p7q0eow95sk/branch/master?svg=true)](https://ci.appveyor.com/project/mazurwiktor/albion-online-stats)

Albion Online Stats
===================

Albion online stats is an extension to MMORPG game - Albion Online. It tracks network traffic and displays various statistics, such as damage and DPS meter calculated from in-game actions. 

## Donate

[![Become a patron](https://c5.patreon.com/external/logo/become_a_patron_button.png)](https://www.patreon.com/wiktormazur)


## Is This Allowed
 ```Our position is quite simple. As long as you just look and analyze we are ok with it. The moment you modify or manipulate something or somehow interfere with our services we will react (e.g. perma-ban, take legal action, whatever```

~MadDave, Technical Lead at Sandbox Interactive for Albion Online, [source](https://forum.albiononline.com/index.php/Thread/51604-Is-it-allowed-to-scan-your-internet-trafic-and-pick-up-logs/?postID=512670#post512670)

* copied from [Albion Online Data](https://www.albion-online-data.com/)


## App preview

![0 6 0](https://user-images.githubusercontent.com/11301109/67619801-62a24180-f800-11e9-9899-c6137403d9c9.png)

# Usage of built release

> **Note** this section does not require any coding knowledge. Those simple two steps are required to use this software :)

## Installation

1. On windows make sure that WinPcap is installed in your system. [Npcap 0.9983 installer for Windows Vista/2008, 7/2008R2, 8/2012, 8.1/2012R2, 10/2016 (x86 and x64)](https://nmap.org/npcap/dist/npcap-0.9983.exe)
2. Download latest release from https://github.com/mazurwiktor/albion-online-stats/releases/latest (.exe for windows .tar for linux and mac)
3. Enjoy :)

## Configuration

After first execution the app is going to create default configuration file named `albion-online-stats.cfg`. Feel free to edit it according to your needs. 

# Getting started

## Prerequisites

- Rust installed (https://www.rust-lang.org/tools/install)
- Python installed 
- *Windows only prerequisites*  https://github.com/libpnet/libpnet#windows


## All platforms
1. Clone repository:
    ```shell 
    git clone https://github.com/mazurwiktor/albion-online-stats.git
    ```
2. [optional] Create and activate python virtualenv

    ```shell
    python -m venv env
    [linux/mac] . env/bin/activate
    [windows] .\env\Scripts\activate.ps1
    ```

3. Install requirements (backend will be compiled during requirements installation)

    ```shell
    pip install -v -r frontend/requirements.txt
    ```

4. Run the application
    ```shell
    [sudo on linux] python frontend/aostats.py
    ```

## GUI testing
- Seting TESTING variable runs frontend without backend dependency

    ```shell
    TESTING=true python frontend/aostats.py
    ```

# License
Licensed under either of

  * Apache License, Version 2.0, ([LICENSE-APACHE](LICENSE-APACHE) or http://www.apache.org/licenses/LICENSE-2.0)
  * MIT license ([LICENSE-MIT](LICENSE-MIT) or http://opensource.org/licenses/MIT)

at your option.
