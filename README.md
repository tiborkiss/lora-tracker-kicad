# Träckthäspäck — a kid-friendly Meshtastic LoRa tracker

KiCad design of a small LoRa tracker board, created as a Swiss
[Zukunftstag](https://www.nationalerzukunftstag.ch/) project: with a group of children
we build a working Meshtastic tracker that the kids can take home and use.

The tracker is deliberately powered by **three ordinary AA batteries** — no
Li-ion cell — so it is simple and safe for children to handle and charge.

## Board

- Seeed Wio WM1110 module (LR1110 packet/radio controller)
- BMI270 motion sensor (wake-on-movement)
- ST7789 display on a 4-pin connector
- Active GNSS antenna + SMA LoRa antenna
- USB-C, SWD debug header
- Battery holder for 3× AA

## Firmware

The corresponding firmware is a Meshtastic fork and can be built from

<https://github.com/tiborkiss/firmware.git>, branch `bringup/wio-st7789-lcd`.

## Repository contents

- `träckthäspäck.kicad_sch` / `.kicad_pcb` / `.kicad_pro` — schematic and PCB
- `träckthäspäck.csv` — bill of materials
- `träcker 01.pdf` — board rendering
- `KiCAD-Shortcuts-PDF.pdf` — KiCad shortcut cheat sheet

## License

MIT — see [LICENSE](LICENSE).
