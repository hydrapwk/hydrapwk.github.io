---
layout: tools-doc
title: esptool
permalink: /doc/tools/hydrapwk-tools-esptool
comments: true
tool-icons: /assets/graphics/tools_graphics/hydrapwk-icon-esptool.svg
tool-version: blank
packages-name: esptool
tools-command: esptool --help
whoupdate: Joe
userupdate: https://github.com/me-joe
categories: E
update: 2025-09-30 06:02:00 +0700
author: Joe
editpage: https://github.com/hydrapwk/hydrapwk.github.io/blob/main/content/_tools/hydrapwk-tools-esptool.md
---

```
 Usage: esptool [OPTIONS] COMMAND [ARGS]...                                                                                                                                                                                                   
                                                                                                                                                                                                                                              
 esptool v5.0.2 - serial utility for flashing, provisioning, and interacting with Espressif SoCs.                                                                                                                                             
                                                                                                                                                                                                                                              
╭─ Options ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
│ --chip              -c  [auto|esp8266|esp32|esp32s2|esp32s3|esp32c3|esp32c2|esp32c6|esp32c61|esp32c5|esp32h2|esp32h21|esp32p4|es  Target chip type.                                                                                        │
│                         p32h4]                                                                                                                                                                                                             │
│ --port              -p  PATH                                                                                                      Serial port device.                                                                                      │
│ --baud              -b  INTEGER                                                                                                   Serial port baud rate used when flashing/reading.                                                        │
│ --port-filter           [TEXT]                                                                                                    Serial port device filter, can be vid=NUMBER, pid=NUMBER, name=SUBSTRING, serial=SUBSTRING.              │
│ --before                [default-reset|usb-reset|no-reset|no-reset-no-sync]                                                       Which reset to perform before connecting to the chip.                                                    │
│ --after             -a  [hard-reset|soft-reset|no-reset|no-reset-stub|watchdog-reset]                                             Which reset to perform after operation is finished.                                                      │
│ --no-stub                                                                                                                         Disable launching the flasher stub, only talk to ROM bootloader. Some features will not be available.    │
│ --trace             -t                                                                                                            Enable trace-level output of esptool interactions.                                                       │
│ --verbose           -v                                                                                                            Print all output, disable collapsing output stages.                                                      │
│ --silent            -s                                                                                                            Silence all output except for errors.                                                                    │
│ --override-vddsdio      [1.8V|1.9V|OFF]                                                                                           Override ESP32 VDDSDIO internal voltage regulator (use with care).                                       │
│ --connect-attempts      INTEGER                                                                                                   Number of attempts to connect, negative or 0 for infinite. Default: 7.                                   │
│ --help              -h                                                                                                            Show this message and exit.                                                                              │
╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
╭─ Commands ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
│ chip-id                                  Print the device chip ID.                                                                                                                                                                         │
│ dump-mem                                 Dump arbitrary memory to a file.                                                                                                                                                                  │
│ elf2image                                Create an application image from ELF file                                                                                                                                                         │
│ erase-flash                              Erase the SPI flash memory.                                                                                                                                                                       │
│ erase-region                             Erase a region of the SPI flash memory.                                                                                                                                                           │
│ flash-id                                 Print the SPI flash memory manufacturer and device ID.                                                                                                                                            │
│ get-security-info                        Print security information report.                                                                                                                                                                │
│ image-info                               Print information about a firmware image (bootloader or application).                                                                                                                             │
│ load-ram                                 Download an image to RAM and execute.                                                                                                                                                             │
│ merge-bin                                Merge multiple raw binary files into a single flashable file.                                                                                                                                     │
│ read-flash                               Read SPI flash memory content.                                                                                                                                                                    │
│ read-flash-sfdp                          Read SPI flash SFDP (Serial Flash Discoverable Parameters).                                                                                                                                       │
│ read-flash-status                        Read SPI flash memory status register.                                                                                                                                                            │
│ read-mac                                 Print the device MAC address.                                                                                                                                                                     │
│ read-mem                                 Read arbitrary memory location.                                                                                                                                                                   │
│ run                                      Run application code loaded in flash.                                                                                                                                                             │
│ verify-flash                             Verify a binary blob against the flash memory content.                                                                                                                                            │
│ version                                  Print esptool version.                                                                                                                                                                            │
│ write-flash                              Write a binary blob to flash. The address is followed by binary filename, separated by space.                                                                                                     │
│ write-flash-status                       Write SPI flash memory status register.                                                                                                                                                           │
│ write-mem                                Modify or write to arbitrary memory location.                                                                                                                                                     │
╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
```