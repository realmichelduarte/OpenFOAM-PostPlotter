# OpenFOAM PostPlotter

A browser-based scientific post-processing tool for OpenFOAM probe and `postProcessing` data, created by **Michel Armando Duarte Flores**.

OpenFOAM PostPlotter is designed for thesis and research workflows where simulation data need to be compared, inspected, styled, and exported as clean scientific figures without building a separate plotting script for every case.

## Current version

**v20**

## Features

- Load OpenFOAM probe files and `postProcessing` folders.
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
3. Load OpenFOAM probe files or a `postProcessing` folder.

The application runs locally in the browser. Simulation data are processed client-side.

> **Note:** OpenFOAM PostPlotter is an independent third-party tool and is not affiliated with or endorsed by the OpenFOAM project or its distributors.

## OpenFOAM workflow

Typical inputs come from OpenFOAM function-object output such as:

```text
postProcessing/
└── <region or function>/
    └── <probe function>/
        └── 0/
            ├── T
            ├── phaseChangeSource:alpha1
            ├── U
            ├── p
            └── ...
```

The parser reads time-series probe data and creates one selectable series per detected probe.

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
