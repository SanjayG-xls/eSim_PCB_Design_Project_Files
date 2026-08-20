<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,30:1a1a2e,60:2d1b69,100:cd7f32&height=250&section=header&text=STM32F4VE%20PCB%20Design&fontSize=62&fontColor=f5deb3&fontAlignY=35&desc=FOSSEE%20Autumn%20Internship%202026%20%E2%80%A2%20eSim%20%2B%20KiCad%20%E2%80%A2%204-Layer%20Board&descSize=18&descColor=cd7f32&descAlignY=55&animation=fadeIn" width="100%" />

<p align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&duration=3000&pause=1200&color=CD7F32&center=true&vCenter=true&multiline=true&repeat=true&width=900&height=80&lines=Complete+PCB+Design+for+STM32F407VET6+Development+Board;Designed+with+eSim+2.5+%7C+KiCad+6+%7C+JLCPCB+4-Layer+Stackup" />
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/STM32F407VET6-03234B?style=for-the-badge&logo=stmicroelectronics&logoColor=white" />
  <img src="https://img.shields.io/badge/ARM_Cortex--M4-0091BD?style=for-the-badge&logo=arm&logoColor=white" />
  <img src="https://img.shields.io/badge/eSim_2.5-2d1b69?style=for-the-badge&logo=opensourcehardware&logoColor=f5deb3" />
  <img src="https://img.shields.io/badge/KiCad_6-314CB0?style=for-the-badge&logo=kicad&logoColor=white" />
  <img src="https://img.shields.io/badge/4--Layer_PCB-cd7f32?style=for-the-badge&logo=pcbway&logoColor=white" />
  <img src="https://img.shields.io/badge/JLCPCB-1a1a2e?style=for-the-badge&logo=jfrog&logoColor=cd7f32" />
  <img src="https://img.shields.io/badge/FOSSEE_IIT_Bombay-6a0dad?style=for-the-badge&logo=academia&logoColor=white" />
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=SanjayG-xls&label=Repository+Views&color=cd7f32&style=flat-square" />
</p>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 📋 Table of Contents

- [About the Project](#-about-the-project)
- [STM32F4VE Hardware Overview](#-stm32f4ve-hardware-overview)
- [Software & Toolchain](#-software--toolchain)
- [Hardware Specifications](#-hardware-specifications--features)
- [PCB Stackup & Layer Configuration](#-pcb-stackup--layer-configuration)
- [3D Board Renders](#-3d-board-renders)
- [Schematic Design](#-schematic-design)
- [PCB Layout Views](#-pcb-layout-views)
- [Design Verification](#-design-verification)
- [How to Use](#-how-to-use-this-repository)
- [Video Walkthrough](#-video-walkthrough)
- [Attribution](#-attribution)

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 🔬 About the Project

> 🏛️ **FOSSEE Autumn Internship 2026 — Screening Task**
>
> ![STM32](https://img.shields.io/badge/Microcontroller-STM32F407VET6-03234B?style=flat-square)
> ![PCB](https://img.shields.io/badge/PCB-4--Layer_Stackup-cd7f32?style=flat-square)
> ![ERC](https://img.shields.io/badge/ERC-Passed_%E2%9C%93-238636?style=flat-square)
> ![DRC](https://img.shields.io/badge/DRC-Passed_%E2%9C%93-238636?style=flat-square)
> ![Manufacturer](https://img.shields.io/badge/Manufacturer-JLCPCB-6a0dad?style=flat-square)

This repository contains the **complete printed circuit board design and schematic files** for an STM32F4VE microcontroller development board. The design was developed as part of the screening task for the **FOSSEE Autumn Internship program in 2026** at **IIT Bombay**.

The core of this board is the high-performance **STM32F407VET6** IC, providing a robust hardware platform for advanced microelectronics and circuit design applications. The board features a **black solder mask** to replicate standard commercial STM development boards, with **custom silkscreen graphics** featuring the official FOSSEE logo, the STM logo, and the designer's name.

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 🧠 STM32F4VE Hardware Overview

The **STM32F4VE** (STM32F407VET6) is a powerful, high-performance **ARM Cortex-M4** core device widely used in embedded systems due to its balance of processing power, memory, and rich peripheral set.

<table>
<tr>
<td width="50%">

### ⚙️ Core Specifications

| Parameter | Value |
|:---|:---|
| **Processor** | ARM 32-bit Cortex-M4 with FPU |
| **Max Frequency** | 168 MHz |
| **Flash Memory** | 512 KB |
| **SRAM** | 192 KB + 4 KB backup |
| **Operating Voltage** | 1.8V – 3.6V |
| **Package** | LQFP-100 |

</td>
<td width="50%">

### 🔌 Advanced Peripherals

| Interface | Count |
|:---|:---|
| **I2C** | Up to 3x |
| **SPI** | Up to 3x |
| **I2S** | Up to 2x |
| **USART / UART** | 4x USART + 2x UART |
| **CAN Bus** | 2x |
| **SDIO** | 1x |

</td>
</tr>
</table>

<p align="center">
  <img src="./Images/My_stm32f4ve.png" width="60%" />
  <br/>
  <sub><b>STM32F407VET6 — Reference Development Board</b></sub>
</p>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 🛠️ Software & Toolchain

<table>
<tr>
  <td align="center" width="160">
    <img src="https://img.shields.io/badge/eSim-2.5-2d1b69?style=for-the-badge&logoColor=white" />
    <br/><sub><b>Schematic Design</b></sub>
  </td>
  <td align="center" width="160">
    <img src="https://img.shields.io/badge/KiCad-6-314CB0?style=for-the-badge&logo=kicad&logoColor=white" />
    <br/><sub><b>PCB Layout</b></sub>
  </td>
  <td align="center" width="160">
    <img src="https://img.shields.io/badge/SnapEDA-Libraries-cd7f32?style=for-the-badge&logoColor=white" />
    <br/><sub><b>3D Models / Symbols / Footprints</b></sub>
  </td>
  <td align="center" width="160">
    <img src="https://img.shields.io/badge/JLCPCB-Fabrication-1a1a2e?style=for-the-badge&logoColor=cd7f32" />
    <br/><sub><b>Manufacturing Rules</b></sub>
  </td>
</tr>
</table>

> 📌 **Note:** Schematic design was done in **eSim 2.5**, with PCB layout handled by **KiCad 6** (integrated via eSim). All component libraries — 3D models, schematic symbols, and footprints — were sourced from **SnapEDA**.

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## ⚡ Hardware Specifications & Features

> 🔧 **Key Features at a Glance**
>
> ![MCU](https://img.shields.io/badge/MCU-STM32F407VET6-03234B?style=flat-square)
> ![Power](https://img.shields.io/badge/Power-3.3V_Routing-cd7f32?style=flat-square)
> ![USB](https://img.shields.io/badge/Micro_USB-Port-6a0dad?style=flat-square)
> ![SD](https://img.shields.io/badge/SD_Card-Reader-2d1b69?style=flat-square)
> ![Battery](https://img.shields.io/badge/Backup-CR12_Battery-cd7f32?style=flat-square)

<table>
<tr>
  <td width="50%" valign="top">

  ### 🎛️ Board Features

  | Feature | Description |
  |:---|:---|
  | **Microcontroller** | STM32F407VET6 high-speed MCU |
  | **Power Management** | 3.3V power routing with CR12 backup battery |
  | **Connectivity** | Micro USB port, SD Card reader |
  | **Headers** | Extensive connector headers for GPIO access |
  | **Timing** | Onboard oscillators for accurate clocking |
  | **User Interface** | Integrated switches and status LEDs |

  </td>
  <td width="50%" valign="top">

  ### 🏭 Manufacturing Specs

  | Parameter | Value |
  |:---|:---|
  | **Layer Count** | 4-Layer PCB |
  | **Manufacturer** | JLCPCB (base model rules) |
  | **Solder Mask** | Black (commercial-grade) |
  | **Silkscreen** | Custom graphics (FOSSEE + STM logos) |
  | **ERC Status** | ✅ Passed (0 errors) |
  | **DRC Status** | ✅ Passed (0 errors) |

  </td>
</tr>
</table>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 🧱 PCB Stackup & Layer Configuration

The board is routed as a **4-layer PCB**, specifically configured to comply with **JLCPCB base model** manufacturing rules.

<table>
<tr>
  <th align="center">Layer</th>
  <th align="center">Name</th>
  <th align="center">Function</th>
</tr>
<tr>
  <td align="center">🔴 Layer 1</td>
  <td align="center"><b>Front (F.Cu)</b></td>
  <td>Signal routing and ground pour</td>
</tr>
<tr>
  <td align="center">🟡 Layer 2</td>
  <td align="center"><b>Inner 1 (In1.Cu)</b></td>
  <td>Dedicated ground plane</td>
</tr>
<tr>
  <td align="center">🟢 Layer 3</td>
  <td align="center"><b>Inner 2 (In2.Cu)</b></td>
  <td>Dedicated 3.3V power plane</td>
</tr>
<tr>
  <td align="center">🔵 Layer 4</td>
  <td align="center"><b>Back (B.Cu)</b></td>
  <td>Ground plane</td>
</tr>
</table>

<table>
<tr>
  <td align="center" width="50%">
    <b>📐 Layer 1 — Front Copper</b><br/>
    <img src="./Images/frontlayer_pcb.png" width="100%" />
  </td>
  <td align="center" width="50%">
    <b>📐 Layer 2 — Inner Ground Plane</b><br/>
    <img src="./Images/in1cuLayer_pcb.png" width="100%" />
  </td>
</tr>
<tr>
  <td align="center" width="50%">
    <b>📐 Layer 3 — Inner Power Plane (3.3V)</b><br/>
    <img src="./Images/in2cuLayer_pcb.png" width="100%" />
  </td>
  <td align="center" width="50%">
    <b>📐 Layer 4 — Back Copper</b><br/>
    <img src="./Images/Backlayer_pcb.png" width="100%" />
  </td>
</tr>
</table>

<details>
<summary><b>🔍 Click to view individual PCB layer renders</b></summary>
<br/>

<table>
<tr>
  <td align="center" width="50%">
    <b>Front Layer PCB</b><br/>
    <img src="./Images/frontlayer_pcb.png" width="100%" />
  </td>
  <td align="center" width="50%">
    <b>Back Layer PCB</b><br/>
    <img src="./Images/Backlayer_pcb.png" width="100%" />
  </td>
</tr>
<tr>
  <td align="center" width="50%">
    <b>Inner Layer 1 (In1.Cu)</b><br/>
    <img src="./Images/in1cuLayer_pcb.png" width="100%" />
  </td>
  <td align="center" width="50%">
    <b>Inner Layer 2 (In2.Cu)</b><br/>
    <img src="./Images/in2cuLayer_pcb.png" width="100%" />
  </td>
</tr>
</table>

<table>
<tr>
  <td align="center" width="50%">
    <b>All Layers Combined</b><br/>
    <img src="./Images/AllLayers_pcb.png" width="100%" />
  </td>
  <td align="center" width="50%">
    <b>All ICs Highlighted</b><br/>
    <img src="./Images/All_ic_pcb.png" width="100%" />
  </td>
</tr>
</table>

</details>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 🖼️ 3D Board Renders

<table>
<tr>
  <td align="center" width="50%">
    <b>🔝 Front View — 3D Render</b><br/>
    <img src="./Images/front_3d.png" width="100%" />
  </td>
  <td align="center" width="50%">
    <b>🔽 Back View — 3D Render</b><br/>
    <img src="./Images/back_3d.png" width="100%" />
  </td>
</tr>
<tr>
  <td align="center" width="50%">
    <b>📐 Side View — 3D Render</b><br/>
    <img src="./Images/side_3d.png" width="100%" />
  </td>
  <td align="center" width="50%">
    <b>📐 Side Down View — 3D Render</b><br/>
    <img src="./Images/side_down_3d.png" width="100%" />
  </td>
</tr>
</table>

<details>
<summary><b>🔍 Click to view additional 3D renders</b></summary>
<br/>

<table>
<tr>
  <td align="center" width="50%">
    <b>3D Model Overview</b><br/>
    <img src="./Images/png_3dmodel.png" width="100%" />
  </td>
  <td align="center" width="50%">
    <b>Front — IC Close-up</b><br/>
    <img src="./Images/Front_IC_pcb.png" width="100%" />
  </td>
</tr>
<tr>
  <td align="center" width="50%">
    <b>Components Only View</b><br/>
    <img src="./Images/OnlyComponents_pcb.png" width="100%" />
  </td>
  <td align="center" width="50%">
    <b>PCB — Components Only (Alt)</b><br/>
    <img src="./Images/pcb_only_components.png" width="100%" />
  </td>
</tr>
</table>

</details>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 📐 Schematic Design

<p align="center">
  <img src="./Images/eschema_full.png" width="100%" />
  <br/>
  <sub><b>Full Schematic Overview — eSim 2.5</b></sub>
</p>

<details>
<summary><b>🔍 Click to view schematic sections</b></summary>
<br/>

<table>
<tr>
  <td align="center" width="50%">
    <b>Schematic — Section 1</b><br/>
    <img src="./Images/eschema_1.png" width="100%" />
  </td>
  <td align="center" width="50%">
    <b>Schematic — Section 2</b><br/>
    <img src="./Images/eschema_2.png" width="100%" />
  </td>
</tr>
</table>

</details>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 🔧 PCB Layout Views

<table>
<tr>
  <td align="center" width="50%">
    <b>📋 PCB — All Layers</b><br/>
    <img src="./Images/pcb_all_layers.png" width="100%" />
  </td>
  <td align="center" width="50%">
    <b>📋 JLCPCB Gerber Preview</b><br/>
    <img src="./Images/JLPCB.png" width="100%" />
  </td>
</tr>
</table>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## ✅ Design Verification

<table>
<tr>
  <td align="center" width="50%">
    <b>🔋 ERC — Electrical Rules Check</b><br/>
    <img src="./Images/ERC.png" width="100%" />
  </td>
  <td align="center" width="50%">
    <b>📏 DRC — Design Rules Check</b><br/>
    <img src="./Images/DRC.png" width="100%" />
  </td>
</tr>
</table>

> ✅ **Electrical Rules Check (ERC):** Passed with **zero errors**. Wire labels were utilized for power nets instead of standard power flags.
>
> ✅ **Design Rules Check (DRC):** Passed with **zero errors**, ensuring complete manufacturability compliance with JLCPCB specifications.

<details>
<summary><b>🔍 Click to view additional verification results</b></summary>
<br/>

<table>
<tr>
  <td align="center" width="50%">
    <b>DRC — PCB View</b><br/>
    <img src="./Images/DRC_PCB.png" width="100%" />
  </td>
  <td align="center" width="50%">
    <b>Excluded ERC Warnings</b><br/>
    <img src="./Images/excluded_ERC.png" width="100%" />
  </td>
</tr>
</table>

</details>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 📦 How to Use This Repository

```
1.  Download the project repository and extract the files.
2.  Open the schematic files using eSim 2.5 to view circuit connections.
3.  Open the PCB layout files in KiCad 6 to inspect:
      • Routing and trace widths
      • Layer stackup configuration
      • 3D model and component placement
4.  Generate Gerber files directly from KiCad for fabrication
    at any standard PCB manufacturer (JLCPCB recommended).
```

> 💡 **Tip:** All component libraries (3D models, symbols, footprints) are sourced from [SnapEDA](https://www.snapeda.com/) and should be imported into your KiCad library manager before editing.

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 🎬 Video Walkthrough

<p align="center">
  <a href="https://www.youtube.com/watch?v=fOVZCzMoj6M">
    <img src="https://img.shields.io/badge/▶_Watch_on_YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white" />
  </a>
</p>

<p align="center">
  <a href="https://www.youtube.com/watch?v=fOVZCzMoj6M">
    <img src="https://img.youtube.com/vi/fOVZCzMoj6M/maxresdefault.jpg" width="70%" />
  </a>
  <br/>
  <sub><b>📹 Click to watch the complete project walkthrough on YouTube</b></sub>
</p>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 🏷️ Attribution

<table>
<tr>
  <td align="center" width="33%">
    <img src="https://img.shields.io/badge/FOSSEE-IIT_Bombay-6a0dad?style=for-the-badge&logoColor=white" />
    <br/><sub><b>Program Host</b></sub>
  </td>
  <td align="center" width="33%">
    <img src="https://img.shields.io/badge/Designer-Sanjay-cd7f32?style=for-the-badge&logoColor=white" />
    <br/><sub><b>PCB Design & Schematics</b></sub>
  </td>
  <td align="center" width="33%">
    <img src="https://img.shields.io/badge/Libraries-SnapEDA-2d1b69?style=for-the-badge&logoColor=white" />
    <br/><sub><b>Component Sources</b></sub>
  </td>
</tr>
</table>

<p align="center">
  <img src="https://img.shields.io/badge/Made_with-eSim_+_KiCad-314CB0?style=for-the-badge&logo=kicad&logoColor=white" />
  <img src="https://img.shields.io/badge/License-MIT-cd7f32?style=for-the-badge" />
</p>

<p align="center">
  <sub>⭐ Star this repo if you found it useful! ⭐</sub>
</p>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,30:1a1a2e,60:2d1b69,100:cd7f32&height=120&section=footer" width="100%" />
