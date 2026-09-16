# MAX3485 – Altium Designer Library

Custom Altium Designer library for the **MAX3485**, a 3.3V, 10Mbps RS-485/RS-422 transceiver.

This project includes a custom-designed schematic symbol and 3D model created and verified using the manufacturer's documentation.

---

## Component Overview

| Parameter | Value |
|---|---|
| Part Number | MAX3485CSA+ |
| Manufacturer | Analog Devices / Maxim Integrated |
| Function | RS-485 / RS-422 Transceiver |
| Supply Voltage | 3.3V |
| Data Rate | Up to 10Mbps |
| Number of Pins | 8 |
| Package | 8-Pin SOIC, Narrow (0.15") |
| Package Type | SOIC-8 |
| Exposed Thermal Pad | No |

---

## Project Scope

The purpose of this project is to create a clean and reusable Altium Designer library for the MAX3485.

The library design process includes:

- Schematic Symbol
- PCB Footprint
- 3D Model
- Pin Mapping
- Package Dimension Verification
- 3D Model Alignment
- Design Rule and Visual Verification

---

## Design Process

### 1. Datasheet Analysis

The manufacturer's documentation was analyzed to determine:

- Pin numbers
- Pin names
- Pin functions
- Electrical pin types
- Package type
- Package dimensions
- Pin pitch
- Lead dimensions
- Recommended PCB land pattern

The official manufacturer documentation was used as the primary reference for the component design.

---

### 2. Schematic Symbol

A custom schematic symbol was created in Altium Designer based on the MAX3485 pin configuration.

#### Pin Configuration

| Pin | Name | Function |
|---:|---|---|
| 1 | RO | Receiver Output |
| 2 | /RE | Receiver Enable |
| 3 | DE | Driver Enable |
| 4 | DI | Driver Input |
| 5 | GND | Ground |
| 6 | A | RS-485 Non-Inverting Input/Output |
| 7 | B | RS-485 Inverting Input/Output |
| 8 | VCC | Power Supply |

The symbol was organized according to functional groups to improve schematic readability.

---

### 3. PCB Footprint

The MAX3485 uses an 8-pin narrow SOIC package with a 1.27 mm pin pitch.

The footprint design is based on the manufacturer's package drawing and recommended land pattern.

#### Main Package Parameters

| Parameter | Value |
|---|---:|
| Number of Pads | 8 |
| Pin Pitch | 1.27 mm |
| Package Body Length | 4.80 – 5.00 mm |
| Package Body Width | 3.80 – 4.00 mm |
| Overall Package Width | 5.80 – 6.20 mm |
| Exposed Pad | None |

The footprint includes:

- SMD Pads
- Pin 1 Identification
- Silkscreen
- Assembly Outline
- Courtyard
- 3D Body Alignment

---

### 4. 3D Model

A custom 3D model was created for the MAX3485 package.

The model was aligned with the PCB footprint to ensure correct:

- Component orientation
- Pin-to-pad alignment
- Package dimensions
- Component height
- Pin 1 orientation

The 3D model was checked using Altium Designer's 3D PCB view.

---

## Verification

The component library was checked against the manufacturer's documentation.

### Schematic Verification

- [x] Pin numbers verified
- [x] Pin names verified
- [x] Pin functions verified
- [x] Power pins identified
- [x] Input/output types reviewed

### Footprint Verification

- [x] Pin count verified
- [x] Pin pitch verified
- [x] Package dimensions verified
- [x] Pad arrangement verified
- [x] Pin 1 identification verified
- [x] No exposed thermal pad
- [x] Silkscreen checked
- [x] Courtyard checked

### 3D Verification

- [x] 3D model created
- [x] Model aligned with footprint
- [x] Pin 1 orientation verified
- [x] Package height checked
- [x] 3D PCB view verified

---

## Design Notes

The MAX3485 and other 8-pin SOIC devices may appear similar physically, but identical pin count and pitch do not necessarily mean identical footprints.

For this reason, the package dimensions and recommended land pattern were independently verified before finalizing the footprint.

The footprint design should always be verified against the exact component ordering code and the manufacturer's latest documentation before production use.

---

## Files

```text
MAX3485/
├── Schematic/
│   └── MAX3485.SchLib
│
├── PCB/
│   └── MAX3485.PcbLib
│
├── 3D/
│   └── MAX3485.step
│
├── Preview/
│   ├── Symbol.png
│   ├── Footprint.png
│   └── 3D.png
│
└── README.md
