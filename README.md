# Klipper Pin Mapper

A web-based tool for visualizing and validating Klipper stepper motor and driver pin assignments against mainboard pinouts.

🔗 **Live Demo:** [https://adamrodgers.github.io/klipper-vis/](https://adamrodgers.github.io/klipper-vis/)

## Features

- **Auto-detect board** from your configuration based on pin signatures
- **Visual board layout** showing all driver slots and their pin assignments
- **Pin validation** - compare your config against expected board pinout
- **Issue detection** with suggested fixes for mismatched pins
- **Comparison table** for detailed side-by-side analysis

## Supported Boards

| Board | Notes |
|-------|-------|
| BTT Octopus Pro v1.0 | PA0 for Motor4-EN |
| BTT Octopus Pro v1.1 | PA2 for Motor4-EN (changed from v1.0) |
| BTT Octopus v1.1 | |
| BTT Kraken | 8x TMC2160 onboard |
| BTT Manta M8P v1.0/1.1 | STM32G0B1 |
| BTT Manta M8P v2.0 | STM32H723 |

## Usage

1. Open the tool in your browser
2. Paste your Klipper `printer.cfg` stepper and TMC driver sections
3. Click "Map Pins" 
4. Review the board visualization and any detected issues
5. Use the "Comparison Table" tab for detailed pin-by-pin analysis

## Why This Exists

When configuring a new 3D printer mainboard or troubleshooting motor issues, it's easy to:
- Use the wrong pin for a driver slot
- Copy a config from a different board version (e.g., Octopus Pro v1.0 vs v1.1)
- Miss subtle pinout differences between board revisions

This tool helps catch those issues before you spend hours debugging.
