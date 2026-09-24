# Changelog

## v22

- Added an eye toggle to hide/show complete cases without deleting them.
- Hidden cases are excluded from plots, legends, previews, metadata counts, and CSV export while retaining their loaded data and styling.
- Series belonging to hidden cases are visually dimmed in the detected-series panel.

## v21

- Added smart recursive OpenFOAM folder scanning.
- Detects nested `postProcessing/probes` outputs even when they are several directories below the selected folder.
- Groups detected outputs by OpenFOAM case root and proposes them as separate cases.
- Added a confirmation dialog with selectable cases and editable case names.
- Added compatible-output detection for probe/sampler folders that are not literally named `probes`.
- Avoids silently merging multiple detected cases into one dataset.

## v20

- Updated About / Developer section.
- Embedded the developer portrait directly in the application for offline use.
- Displayed the full portrait vertically instead of cropping it to a square.
- Preserved the OpenFOAM PostPlotter plotting and case-comparison functionality from v16–v19.

## v16

- Added case and individual-file deletion controls.
- Continued multi-case plotting, scientific figure editing, export controls, and detected-series management.