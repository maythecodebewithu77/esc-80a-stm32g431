Hardware design of a drone motor controller (ESC) built around the
STM32G431CBU6 microcontroller and the DRV8302 gate driver. Designed in KiCad.

![Schematic](docs/schematic.png)

## Status
- Schematic: complete and reviewed
- PCB layout: [in progress / completed / handed to a layout designer]
- Firmware: not started
- Hardware testing: not done yet

## Main specifications
- Input voltage: up to 25 V
- Current: 80 A (design target)
- Microcontroller: STM32G431CBU6
- Gate driver: DRV8302
- Power supply: LMR16020 (25 V to 12 V), TPS54331 (12 V to 3.3 V)
- Power MOSFETs: NVMFS5C638NLT1G

## Design notes
- Planned 4-layer PCB: signal, ground, power, signal, with 2 oz copper
- Errors found and fixed during design review: PWM pin mapping,
  current-sense wiring, reverse-polarity MOSFET size, ADC clamp diode

## Folders
- `hardware/` KiCad project files
- `docs/` schematic and design notes

## Next steps
- Complete PCB layout and thermal checks
- Write and test firmware

## Author
Vigneshwar S, ECE student, SRM IST
