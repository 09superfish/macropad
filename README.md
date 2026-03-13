# Macropad

A custom 5×5 mechanical macropad built around the ATmega32U4-MU microcontroller. This is a two-person hobby project — one handles the PCB design, the other handles the firmware.

> ⚠️ **Status: PCB designed — not yet built.** This project is still in the hardware design phase.

---

## Overview

| Property | Details |
|----------|---------|
| Layout | 5×5 (25 keys) |
| Microcontroller | ATmega32U4-MU |
| PCB Tool | KiCad |
| Firmware | Custom (ATmega32U4) |
| Status | PCB designed, not built |

---

## Project Structure

```
macropad/
├── KiCad/          # Schematic and PCB layout files
├── firmware/       # Firmware source (ATmega32U4)
└── README.md
```

---

## Pin Mapping

The 5×5 key matrix uses the following pin assignment:

| Function | Pins |
|----------|------|
| Rows (output) | PB0, PB1, PB2, PB3, PB4 |
| Columns (input, pull-up) | PF0, PF1, PF2, PF3, PB5 |

---

## Hardware

- **MCU:** ATmega32U4-MU (QFN-44 package)
- **PCB:** Designed in KiCad
- **Interface:** USB (native USB support on the 32U4)
- **Key matrix:** 5×5 with diodes per key to prevent ghosting

---

## Firmware

Firmware is written for the ATmega32U4 and maintained separately. The firmware handles:

- Matrix scanning
- USB HID communication
- Key mapping / layers

---

## Team

| Role | Person |
|------|--------|
| PCB Design | [@09superfish](https://github.com/09superfish) |
| Firmware | TBD (friend's GitHub handle) |

---

## Branches

| Branch | Description |
|--------|-------------|
| `main` | outdated design |
| `routing-re-design` | Current PCB routing rework |

---

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use it as a reference for your own macropad builds.
