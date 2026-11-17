# QUADLINK (QL-04) — USB 2.0 High-Speed Hub

**A custom USB hub PCB designed in the eSim / KiCad-based workflow for FOSSEE PCB Design Task 7.**

QUADLINK provides one upstream USB-A connection and four downstream connections: three USB-A ports and one USB Type-C port. The design is based on the **Microchip USB2514B** hub controller and supports **USB 2.0 High-Speed signaling at up to 480 Mb/s**. The upstream bandwidth is shared by all four downstream ports; the USB-C connector carries USB 2.0 data, not USB 3.x SuperSpeed signals.

> **Project status:** Schematic capture, footprint assignment, PCB placement, routing, and design-rule cleanup have been completed. This is a PCB design project; hardware fabrication, functional testing, USB compliance, and electrical performance have **not** been demonstrated.

## Project objectives

- Design and document a multiport USB hub using the eSim schematic-to-PCB workflow.
- Integrate upstream and downstream USB data connections, ESD protection, regulated power, and per-port power switching.
- Apply good PCB design practices for USB differential pairs, component placement, decoupling, grounding, and signal routing.
- Verify the layout with KiCad's Design Rule Checker (DRC) and present it in the 3D Viewer.

## Hardware overview

| Block | Implementation |
| --- | --- |
| USB hub controller | Microchip **USB2514B** |
| Upstream interface | **1 × USB-A** |
| Downstream interfaces | **3 × USB-A**, **1 × USB Type-C** |
| USB-C configuration / control | STMicroelectronics **STUSB1602** |
| Downstream port power switching | **4 × TPS2553** current-limited power-distribution switches |
| Local 3.3 V supply | **AP2112K-3.3** regulator |
| USB data-line protection | **USBLC6-2SC6** ESD devices |
| Hub clock | **24 MHz** crystal |
| Nominal signaling rate | USB 2.0 High-Speed, **480 Mb/s** (shared) |

### Functional blocks

1. **USB hub core:** The USB2514B handles the upstream link and distributes USB 2.0 traffic to the four downstream ports.
2. **USB port protection:** ESD protection devices are located along the USB data connections.
3. **Port power:** TPS2553 switches provide individual downstream VBUS switching and fault signaling.
4. **USB-C control:** The STUSB1602 handles USB-C attach/configuration-related signals. The hub and USB-C controller participate in the USB-C port's VBUS-enable logic.
5. **Power and clock:** The board derives local 3.3 V power from upstream 5 V and provides the hub with a 24 MHz clock.
6. **Debug access:** Test points and labeled interface signals support inspection and troubleshooting.

## PCB layout and routing

- USB D+ and D− are routed as **five differential pairs**: one upstream pair and one pair for each downstream port.
- The USB differential-pair net class targets **90 Ω differential impedance**. The configured nominal width and gap are **0.266 mm** and **0.200 mm**, respectively; these are layout settings, **not a measured impedance result**.
- ESD devices are included near the respective USB connection paths.
- Power connections use wider tracks and copper pours where appropriate; low-speed control lines are routed separately.
- The layout includes decoupling close to supply pins, ground connections, mounting holes, and silkscreen annotations.

### Copper stackup (implementation detail)

The board uses a **four-copper-layer stackup**: `F.Cu` for primary signal/power routing, `In1.Cu` as a GND reference plane, `In2.Cu` for separated power pours, and `B.Cu` for additional routing. USB differential-impedance and return-path performance require stackup-specific verification before manufacturing.

## Design workflow

1. Create and organize the schematic in eSim's schematic environment.
2. Assign footprints and check component pin mappings.
3. Transfer the design to PCB Editor with **Sch to PCB Update**.
4. Place components, define the board outline, and route data, power, and control connections.
5. Configure/refill copper zones and run DRC.
6. Inspect the layout using the eSim/KiCad 3D Viewer.

## Repository contents

The project is distributed with its editable KiCad/eSim design files. Paths may vary depending on the final submission layout.

```text
usbhub/
├── usbhub.kicad_sch           # Schematic
├── usbhub.kicad_pcb           # PCB layout
├── usbhub.kicad_pro           # Project settings
├── usbhub.kicad_dru           # Custom design rules, if used
├── fp-lib-table               # Footprint library mappings
├── sym-lib-table              # Symbol library mappings
├── USB_Hub_Custom.pretty/     # Project-specific footprints
├── STUSB1602AQTR/            # Related component library assets, if referenced
├── TPS2553DBVT/              # Related component library assets, if referenced
├── 3d_models/                # Required project-relative STEP/WRL models, if included
└── documentation/            # Task 7 report, screenshots, and DRC evidence
```

**Note:** Include only files and libraries actually referenced by the final project. Local lock files, caches, editor preferences, and automatic backup folders are not needed in the submission.

## Opening the project

1. Download or clone the project folder without changing its internal relative paths.
2. Open it in the **eSim version required by the evaluation**.
3. Open `usbhub.kicad_sch` and `usbhub.kicad_pcb` using the included project configuration.
4. Check the footprint/symbol library tables and required 3D model paths.
5. Refill copper zones, run DRC, and open the 3D Viewer to inspect the board.

**Compatibility notice:** The layout has been edited using KiCad 9-based tools. Opening and rendering the PCB in an eSim installation does **not**, by itself, establish full editability in eSim 2.3/2.5. The final submission must be checked using the exact required version and its complete schematic-to-PCB workflow.

## Verification and limitations

- **DRC:** The latest design-stage check was reported as having zero errors and zero warnings. Include an exported final DRC report or screenshot in `documentation/` for reproducible evidence.
- **Not hardware tested:** No assembled-board operation, transfer-rate benchmark, or USB certification is claimed.
- **Power budget:** The upstream USB 2.0 bus-power budget and downstream current-limit policy require explicit review before hardware use.
- **Signal integrity:** The target differential impedance, especially at layer transitions and across reference-plane regions, requires manufacturer-specific stackup verification.
- **USB-C operation:** Source configuration, attach behavior, fault handling, and VBUS-enable sequencing require hardware-level verification.

## Documentation

The accompanying Task 7 report should include the project overview, circuit descriptions, schematic and footprint screenshots, PCB layout and routing methodology, DRC evidence, 3D renderings, design considerations, and conclusions.

## Author and context

**Sanjay G.**  
Chennai Institute of Technology  
Prepared for **FOSSEE eSim Semester Long Internship — Autumn 2026, Task 7: PCB Design**.
