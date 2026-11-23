<p align="center">
  <img src="images/QL-04 USB Hub Circuit Banner.png" alt="QL-04 USB Hub banner" width="100%" />
</p>

# QUADLINK — QL-04

**USB 2.0 High-Speed Hub | FOSSEE eSim Internship — Task 7**

QL-04 is a custom USB hub PCB based on the Microchip USB2514B. It connects a single USB-A host interface to three USB-A downstream ports and one USB-C downstream port, with individual port power control and ESD protection.

## Specifications

| Parameter | Specification |
| :--- | :--- |
| Hub controller | USB2514B |
| Upstream | 1 × USB-A male |
| Downstream | 3 × USB-A female + 1 × USB-C |
| USB standard | USB 2.0 High-Speed |
| Signaling rate | Up to 480 Mbps, shared across ports |
| Input power | 5 V USB bus power |
| Local supply | 3.3 V |
| Clock | 24 MHz |

## Circuit design

- **USB2514B:** Four-port USB hub controller.
- **AP2112K-3.3:** Local voltage regulation and supply filtering.
- **TPS2553:** Individual port power switching and overcurrent fault signaling.
- **STUSB1602:** USB-C configuration and attachment detection.
- **74LVC1G04 / 74LVC1G08:** USB-C VBUS enable logic.
- **USBLC6-2SC6:** ESD protection for USB data lines.
- **Shield and debug:** Parallel RC shield bonding and accessible test points.

## PCB layout

The layout uses five USB differential pairs, short clock connections, local decoupling, wider power tracks and clearly labeled interfaces. The USB data pairs target 90 Ω differential impedance, with a nominal trace width of 0.266 mm and gap of 0.200 mm.

### Copper stackup

The PCB uses four copper layers, with routing primarily on the outer layers and internal copper pours for ground and power distribution. The nominal impedance settings require manufacturer-specific verification.

## Design verification

The recorded ERC and DRC results show zero reported errors and warnings under the enabled checks, and DRC reports zero unconnected items.

The recorded verification results also show ignored checks and ERC exclusions; schematic parity was not run in the displayed DRC result. These results are design-stage checks, not hardware validation.

## Project files

| File / folder | Description |
| :--- | :--- |
| `usbhub.kicad_sch` | Editable schematic |
| `usbhub.kicad_pcb` | PCB layout |
| `usbhub.kicad_pro` | KiCad project settings |
| `usbhub.kicad_dru` | Custom design rules |
| `usbhub.kicad_prl` | Local project preferences |
| `usbhub.proj` | eSim project configuration |
| `fp-lib-table`, `sym-lib-table` | Library mappings |
| `STUSB1602AQTR/`, `TPS2553DBVT/`, `USB_Hub_Custom.pretty/` | Imported and custom libraries |
| `images/` | README banner |

## Opening the project

1. Clone or download the complete project folder.
2. Open the project using eSim and its KiCad-based design tools.
3. Check the included footprint, symbol and 3D model paths.
4. Open the schematic and PCB, run ERC/DRC and inspect the 3D view.

The design was edited using KiCad 9-based tools. Full compatibility with the required eSim 2.3/2.5 environment should be verified before submission.

## Project status

Schematic capture, footprint assignment, PCB routing and design-stage verification are complete. Fabrication and physical testing have not been performed. USB power budgeting, source configuration and signal integrity require further validation before hardware deployment.

---

**Designed by Sanjay G.**  
Department of VLSI Design and Technology, Chennai Institute of Technology  
FOSSEE eSim winter Internship — 2026 | Task 7
