# TI-BASIC Ham Radio Wave Calculator

Radio wave calculator for amateur radio operators using fundamental physics equations.

## What It Does

Calculates electromagnetic wave properties (frequency, wavelength, energy) and identifies the corresponding radio band. Given any one property, it computes the other two using Planck's equation and the wave equation.

## Usage

1. Run the program
2. Select input type from menu:
   - **Input Frequency (MHz)** - calculates energy and wavelength
   - **Input Wavelength (m)** - calculates energy and frequency
   - **Input Energy (J)** - calculates frequency and wavelength
3. Program displays the calculated values
4. Program identifies the radio band based on frequency

## Physics

Uses two fundamental equations:

**Wave Equation:** c = fλ
- c = speed of light (3×10⁸ m/s)
- f = frequency (Hz)
- λ = wavelength (m)

**Planck's Equation:** E = hf
- E = photon energy (J)
- h = Planck's constant (6.63×10⁻³⁴ J·s)
- f = frequency (Hz)

## Band Classification

- **< 30 MHz:** HF/MF/LF Band
- **30-88 MHz:** HF/VHF Band
- **88-174 MHz:** VHF (2M) Band
- **174-420 MHz:** VHF Band
- **420-1000 MHz:** UHF (70CM) Band
- **1000-3000 MHz:** UHF Band
- **> 3000 MHz:** SHF+ Band

## Notes

Frequency inputs/outputs are in MHz for convenience. Internal calculations convert to Hz for physics equations.