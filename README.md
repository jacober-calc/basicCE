# basicCE

An archive of 13 TI-BASIC programs written by Eric James (jacober-calc) for the **TI-84 Plus CE** graphing calculator: physics experiments, practical calculators, and a fictional terminal simulation.

Each program has its own folder containing the original calculator file, a usage guide, screenshots, and the original documentation. The [originals](originals/) directory preserves all 13 ZIP downloads unchanged.

## Program catalogue

### Motion and braking

| Program | Calculator name | Purpose |
| --- | --- | --- |
| [GDist CE](programs/gdist/) | `GDIST` | Calculates deceleration, stopping time, and g-force from initial velocity and stopping distance. |
| [GForce CE](programs/gforce/) | `GFORCE` | Calculates deceleration, stopping distance, and stopping time from initial velocity and desired g-force. |
| [GTime CE](programs/gtime/) | `GTIME` | Calculates deceleration, stopping distance, and g-force from initial velocity and stopping time. |
| [Stopping Distance CE](programs/stopping-distance/) | `STOPDIST` | Estimates reaction distance, braking distance, and total stopping distance from speed and road conditions. |

### Transit and vehicles

| Program | Calculator name | Purpose |
| --- | --- | --- |
| [BusPlan CE](programs/busplan/) | `BUSPLAN` | Estimates the number of buses required for a route from round-trip time, layover percentage, and headway. |
| [Overhang CE (KICKOUT)](programs/overhang/) | `KICKOUT` | Calculates net lateral rear-overhang kickout for a vehicle turning through a given angle. |

### Marine

| Program | Calculator name | Purpose |
| --- | --- | --- |
| [CPA CE](programs/cpa/) | `CPA` | Calculates closest point of approach between two vessels using constant courses and speeds. |
| [Hull Speed CE](programs/hull-speed/) | `HULLSPD` | Calculates theoretical vessel hull speed from a length entered in feet or metres. |

### Space

| Program | Calculator name | Purpose |
| --- | --- | --- |
| [Delta-V CE](programs/delta-v/) | `DELTAV` | Explores the ideal rocket equation using initial mass, final mass, and exhaust velocity. |
| [Orbit CE](programs/orbit/) | `ORBIT` | Explores circular-orbit calculations using orbital velocity or height, with preset and custom celestial bodies. |

### Radio

| Program | Calculator name | Purpose |
| --- | --- | --- |
| [HAMRadio CE](programs/hamradio/) | `HAMRADIO` | Calculates frequency, wavelength, and photon energy and displays a radio-band classification. |

### Everyday calculations

| Program | Calculator name | Purpose |
| --- | --- | --- |
| [Hours CE](programs/hours/) | `HOURS` | Calculates hours worked and pay from start and end times entered in H.MM format. |

### Fictional terminal simulation

| Program | Calculator name | Purpose |
| --- | --- | --- |
| [SornaOS CE](programs/sornaos/) | `SORNAOS` | A menu-driven fictional Sorna field terminal with company messages, dinosaur data, and simulated network failures. |

## Installation

1. Open the program’s folder and read its README for units, settings, and assumptions.
2. Transfer its `.8xp` file to a TI-84 Plus CE using TI Connect CE.
3. Open the calculator’s PRGM menu and run the calculator name listed above.

The filenames are preserved from the original releases. The name displayed on the calculator is stored inside the file and may differ from its filename. Transfer the `.8xp` file, not the screenshots or documentation.

## Archive layout

```text
basicCE/
├── README.md
├── LICENSE
├── originals/                 # Unchanged original ZIP downloads
└── programs/
    └── <program>/
        ├── README.md         # Current archive guide
        ├── <original>.8xp    # Original tokenized TI-BASIC program
        ├── docs/             # Original documentation, unchanged
        └── screenshots/      # Original screenshots, unchanged
```

The `.8xp` files contain tokenized TI-BASIC programs rather than plain-text source listings. This archive does not yet include verified text exports or a build system.

## Preservation and status

Imported from the 13 supplied CE release ZIPs on October 29, 2026. Original ZIPs, calculator files, documentation, and screenshots are preserved byte-for-byte.

The per-program READMEs are new archive guides. Original documentation retains its historical wording, filenames, dates, examples, and links, including RTF files and SornaOS’s `.md.md` extensions. Version numbers are recorded only where the original documentation provides them. ZIP timestamps are not treated as release dates.

This is a preservation import, not a new program release. Files and links have been checked during import; execution and numerical results have not been tested on calculator hardware. Formula-based tools retain the assumptions and limitations of their original models. SornaOS’s reconstruction story and archival note are fictional, in-universe material.

For future changes, keep the original ZIPs unchanged and update the affected program’s README to explain any changes to its extracted files. Verified readable TI-BASIC listings can be added alongside the corresponding `.8xp` files later.

## License

The programs and accompanying author-created documentation are available under the [MIT license](LICENSE). Third-party names and fictional references remain the property of their respective owners.
