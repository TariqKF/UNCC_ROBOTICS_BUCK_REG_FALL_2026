# Synchronous Buck Converter (4S → 12V)

A high-current synchronous buck converter that steps a 4S battery pack down to a regulated 12 V output. Designed in KiCad 10 by **Tariq Khalaf**.

![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)

## Features

- **Controller:** TI LM5145 synchronous buck controller (U1)
- **Power stage:** 6× TI CSD18512Q5B N-channel MOSFETs (Q1–Q6), 1.0 µH inductor (L1)
- **Input protection:** LM74700 ideal-diode reverse polarity protection (U2), SMDJ20CA TVS diode (D2), 60 A fuse (F1)
- **Connectors:** XT90 input and output (J1, J2)
- **Snubber** on the switch node to reduce voltage spikes and EMI
- **Status LEDs:** green and red indicators (D3, D4)

## Repository Contents

| File | Description |
|---|---|
| `Buck-Booster-Convertor.kicad_pro` | KiCad project file (open this) |
| `Buck-Booster-Convertor.kicad_sch` | Top-level schematic |
| `Buck_Converter.kicad_sch` | Buck converter sub-sheet |
| `Buck-Booster-Convertor.kicad_pcb` | PCB layout |
| `Sch_PDF/Buck-Booster-Convertor.pdf` | Schematic PDF (no KiCad needed) |

## Opening the Project

1. Install [KiCad](https://www.kicad.org/) 10 or newer.
2. Clone or download this repository.
3. Open `Buck-Booster-Convertor.kicad_pro` in KiCad.

## License

© 2026 Tariq Khalaf. This design is licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). See [`LICENSE`](LICENSE) for the full text.

You are free to use, modify, build, share, and sell this design, including commercially, **as long as you give credit**.

### How to Credit

If you use, modify, or share this design (or anything derived from it), you must:

1. **Credit the author:** Tariq Khalaf
2. **Link to the original:** https://github.com/TariqKF/UNCC_ROBOTICS_BUCK_REG_FALL_2026
3. **Link to the license:** https://creativecommons.org/licenses/by/4.0/
4. **Say if you made changes**

Example attribution:

> Based on "Synchronous Buck Converter" by Tariq Khalaf (https://github.com/TariqKF/UNCC_ROBOTICS_BUCK_REG_FALL_2026), licensed under CC BY 4.0. Modified by [your name].

For physical boards, put the credit in your documentation, README, or product listing.

## Disclaimer

This design is provided as-is, without warranty of any kind. It handles high currents from lithium battery packs. Build and use it at your own risk.
