# ISFS Soil Sensor Documentation & Verification Box

This repository contains documentation, CAD files, and design resources for ISFS soil sensors, as well as the design files for the custom sensor verification test box.

## Repository Structure

```
/
├── README.md                  # This file
├── index.html                 # Landing page with links to all sensor docs
│
├── sensors/
│   ├── gsoil/                 # Gsoil (soil heat flux) sensor docs & info
│   ├── tsoil/                 # TSoil (soil temperature) sensor docs & info
│   ├── qsoil/                 # Qsoil (soil moisture) sensor docs & info
│   └── tp01/                  # TP01 (soil thermal properties) sensor docs & info
│
└── verification-box/          # Sensor verification test box
    ├── README.md              # Box-specific documentation
    └── [CAD files]            # Fusion 360 and exported files (aluminum extrusion frame, laser cut panels, 3D printed parts)
```

## Sensor Pages

Each sensor folder contains an HTML page with relevant specifications, calibration notes, known issues, and field deployment guidelines. See `index.html` for a full linked overview.

## Verification Test Box

The verification box is an 18×18×6 inch enclosure built from aluminum extrusions, laser-cut aluminum panels, insulation foam, and 3D printed components. It is designed for batch testing and cross-validating soil sensors before field deployment.

### Hardware

| Component | Part |
|-----------|------|
| Fan assembly | Dell PowerEdge R730/R730XD 6-Fan Cage (KJ38G-A00) |
| Power supply | Dell PowerEdge R820/R720/R720XD 750W PSU (E750E-S0) |
| Heating option A | 150W heat lamp |
| Heating option B | 500mm² silicone heating pad (3D printer bed style) |

Active ventilation is provided at the bottom of the enclosure. The heating element (lamp or pad) sits above the sand bed. The silicone pad is the preferred heating option due to its precision and suitability for extended runs.

### Design Goals

- Uniform, controllable thermal environment for sensor cross-validation
- Support for simultaneous testing of large sensor batches
- Reproducible day/night thermal cycle simulation
- Improved over the original heat lamp + aluminum plate approach used in earlier tests

## Background

This repository grew out of batch verification work done on Gsoil sensors at ISFS. After repaints, wire repairs, or wizard board replacements, sensors must be verified against each other before field deployment to confirm they are within 0.5 Wm⁻²mV⁻¹ of each other. See the Gsoil sensor page for the full verification procedure.


## Questions

For questions contact Aanthony Edwards (OP)