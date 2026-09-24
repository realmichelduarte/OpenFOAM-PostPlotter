# OpenFOAM PostPlotter

A browser-based scientific post-processing tool for OpenFOAM probe and `postProcessing` data, created by **Michel Armando Duarte Flores**.

OpenFOAM PostPlotter is designed for thesis and research workflows where simulation data need to be compared, inspected, styled, and exported as clean scientific figures without building a separate plotting script for every case.

## Current version

**v22**

## Features

- Load OpenFOAM probe files and `postProcessing` folders.
- Smart recursive folder import: select a project folder and PostPlotter can locate nested `postProcessing/probes` outputs automatically.
- Automatic OpenFOAM case detection with a confirmation dialog before adding detected cases.
- Editable detected case names and selective case import.
- Recognize compatible probe outputs even when the sampler folder is not literally named `probes`.
- Hide or show complete cases with an eye toggle without deleting their data or settings.
- Detect common fields such as temperature, liquid fraction, velocity, pressure, density, and additional scalar fields.
- Compare multiple simulation cases.
- Keep the same physical variable color across cases while using different line styles.
- Combined or separated plot layouts.
- Dual-axis plotting.
- Kelvin / Celsius conversion.
- Custom axis ranges and decimal formatting.
- Editable title, legend, axis labels, tick labels, and pinned-point annotations.
- Exact export preview (WYSIWYG) and workspace preview.
- Thesis, paper, and wide export presets.
- PNG, SVG, and CSV export.
- English and Spanish interface.
- Light and dark app appearance.
- Local persistence of visual defaults.
- Built-in About / Developer section.

## Run locally

No installation or build process is required.

1. Download or clone the repository.
2. Open `index.html` in a modern desktop browser.
3. Load individual OpenFOAM files or select a project/post-processing folder.

The application runs locally in the browser. Simulation data are processed client-side.

> **Note:** OpenFOAM PostPlotter is an independent third-party tool and is not affiliated with or endorsed by the OpenFOAM project or its distributors.

## Smart folder import

You can select a folder above the actual probe output. For example:

```text
QuickCup_Solidification/
├── B4/
│   └── postProcessing/
│       └── probes/
└── C4/
    └── postProcessing/
        └── probes/
```

PostPlotter scans the selected tree, identifies compatible OpenFOAM probe outputs, groups them by case root, and asks which detected cases should be added.

## Author

**Michel Armando Duarte Flores**  
Materials Engineer · Metallurgical Engineering Research  
GitHub: [@realmichelduarte](https://github.com/realmichelduarte)  
LinkedIn: [Michel A. Duarte Flores](https://www.linkedin.com/in/realmichelduart/)  
Instagram: [@realmichelduarte](https://instagram.com/realmichelduarte)

## License

**Proprietary — All Rights Reserved.**

This repository is public for viewing, demonstration, portfolio, and source-review purposes only. Public availability does **not** grant permission to copy, modify, redistribute, rebrand, sell, reuse, or incorporate this software into other projects.

See [`LICENSE`](LICENSE) for the complete terms.

© 2026 Michel Armando Duarte Flores. All Rights Reserved.