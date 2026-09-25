# OpenFOAM PostPlotter

A browser-based scientific post-processing tool for OpenFOAM probe, spatial-profile, solver-log, and `postProcessing` data, created by **Michel Armando Duarte Flores**.

OpenFOAM PostPlotter is designed for thesis and research workflows where simulation data need to be compared, inspected, styled, animated, and exported as clean scientific figures without building a separate plotting script for every case.

## Current version

**v29**

## Features

- Load OpenFOAM probe files, spatial-profile `.xy` files, solver logs, and `postProcessing` folders.
- Smart recursive folder import with automatic OpenFOAM case detection.
- Separate data views for **Time series**, **Spatial profiles**, and **Solver logs** so incompatible datasets are not mixed.
- Detect horizontal/vertical spatial profiles from file structure and contents, including files such as `line_y20mm.xy` and `line_y30mm.xy`.
- Read spatial-profile columns such as `x U_x U_y U_z T phaseChangeSource:alpha1`.
- Friendly OpenFOAM variable labels while retaining original field names in metadata/tooltips.
- Automatic derived velocity fields:
  - `Velocity magnitude |U|`
  - `Velocity XY`
- Difference plots between compatible cases with maximum absolute difference and its X position.
- Compare multiple profile heights at the same variable and time.
- Time slider, previous/next controls, Play/Pause animation, and optional locked axes for profile evolution.
- Automatic scientific axis precision to avoid visually duplicated tick labels.
- Spatial-profile family detection: related cases can share a family color while variants use different line styles.
- Time-series/probe plots remain color-coded by physical variable.
- Quick case and family visibility controls; hidden families stay hidden during temporal animation.
- Automatic case-comparison shortcuts for detected case families/variants.
- Curve metrics including min/max, X locations, average, velocity RMS, Uy zero crossings, and difference metrics where applicable.
- Configurable physical reference lines, including liquidus, solidus, liquid fraction, velocity-zero, geometric-center, and custom X/Y references.
- Resizable/collapsible settings panel, independently scrollable plot area, chart zoom and Fit controls.
- Resizable adaptive legend with grouped cases/families.
- Thesis Figure mode with high-resolution PNG and SVG export.
- Hide/show complete cases without deleting loaded data or settings.
- PNG, SVG, and CSV export.
- English and Spanish interface.
- Light and dark app appearance.
- Local persistence of visual defaults.
- Built-in About / Developer section.

## Solver logs

OpenFOAM PostPlotter recognizes `foamLog`-style outputs in `logs/` and groups related files instead of treating every sub-iteration as an unrelated dataset.

For example:

```text
logs/
├── p_rgh_0
├── p_rgh_1
├── ...
├── p_rgh_5
├── p_rghFinalRes_0
└── p_rghIters_0
```

The **Solver logs** view lets you select a log family and move between available sub-iterations with a selector and previous/next controls.

## Run locally

No installation or build process is required.

1. Download or clone the repository.
2. Open `index.html` in a modern desktop browser.
3. Load individual OpenFOAM files or select a project/post-processing folder.

The application runs locally in the browser. Simulation data are processed client-side.

> **Note:** OpenFOAM PostPlotter is an independent third-party tool and is not affiliated with or endorsed by the OpenFOAM project or its distributors.

## Smart folder import

You can select a folder above the actual outputs. PostPlotter scans the selected tree, identifies compatible OpenFOAM datasets, groups them by case root, and keeps time-series, spatial-profile, and solver-log data in their appropriate views.

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
