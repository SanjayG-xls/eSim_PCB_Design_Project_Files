<div align="center">

<!-- ══════════════════ HEADER ══════════════════ -->

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,25:1a1a2e,50:2d1b69,100:cd7f32&height=220&section=header&text=STM32F4VE%20PCB%20Design&fontSize=48&fontColor=f5deb3&fontAlignY=35&desc=4-Layer%20Custom%20Development%20Board%20%E2%80%A2%20eSim%20%2B%20KiCad&descSize=18&descColor=cd7f32&descAlignY=55&animation=fadeIn" width="100%" />

<br/>

![STM32](https://img.shields.io/badge/STM32F407VET6-03234B?style=for-the-badge&logo=stmicroelectronics&logoColor=white)
![ARM](https://img.shields.io/badge/ARM_Cortex--M4-0091BD?style=for-the-badge&logo=arm&logoColor=white)
![KiCad](https://img.shields.io/badge/KiCad-314CB0?style=for-the-badge&logo=kicad&logoColor=white)
![eSim](https://img.shields.io/badge/eSim-2d1b69?style=for-the-badge&logo=open-source-initiative&logoColor=cd7f32)
![4-Layer](https://img.shields.io/badge/4--Layer_PCB-cd7f32?style=for-the-badge)
![FOSSEE](https://img.shields.io/badge/FOSSEE_IIT_Bombay-1a1a2e?style=for-the-badge)

<br/>

<table>
<tr>
<td>

🔬 &nbsp; Complete **4-layer PCB design** for an **STM32F407VET6** development board.
<br/>
📐 &nbsp; From **schematic capture** through **layout, verification, and manufacturing** — all documented below.
<br/>
🏛️ &nbsp; Designed using **eSim + KiCad** for the **FOSSEE** project at **IIT Bombay**.

</td>
</tr>
</table>

</div>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 📋 Board Specifications

<div align="center">

<table>
<tr>
<td align="center" width="25%">

**🧠 MCU**
<br/><br/>
STM32F407VET6
<br/>
`LQFP-100`
<br/>
ARM Cortex-M4 @ 168 MHz

</td>
<td align="center" width="25%">

**💾 Memory**
<br/><br/>
512 KB Flash
<br/>
192 KB SRAM
<br/>
\+ W25Q16 16Mbit SPI Flash

</td>
<td align="center" width="25%">

**📐 PCB Stackup**
<br/><br/>
4-Layer Board
<br/>
`F.Cu → In1.Cu → In2.Cu → B.Cu`
<br/>
Signal / GND / Power / Signal

</td>
<td align="center" width="25%">

**🏭 Fabrication**
<br/><br/>
JLCPCB
<br/>
Custom Silkscreen Bitmaps
<br/>
SMD + Through-Hole Mix

</td>
</tr>
</table>

</div>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 🖼️ 3D Renders

<div align="center">

<table>
<tr>
<td align="center" width="50%">

**🔝 Front View**

<img src="./front_3d.png" width="100%" />

</td>
<td align="center" width="50%">

**🔄 Back View**

<img src="./back_3d.png" width="100%" />

</td>
</tr>
<tr>
<td align="center" width="50%">

**↗️ Side View**

<img src="./side_3d.png" width="100%" />

</td>
<td align="center" width="50%">

**↘️ Side (Bottom)**

<img src="./side_down_3d.png" width="100%" />

</td>
</tr>
</table>

<details>
<summary><b>📸 More 3D Views</b></summary>
<br/>

| Render | Preview |
|:---:|:---:|
| **Full 3D Model** | <img src="./png_3dmodel.png" width="500" /> |
| **Board Photo** | <img src="./My_stm32f4ve.png" width="500" /> |

</details>

</div>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 📝 Schematic

<div align="center">

<details open>
<summary><b>📜 Full Schematic</b></summary>
<br/>

<img src="./eschema_full.png" width="100%" />

</details>

<details>
<summary><b>📄 Sheet 1 — MCU & Power</b></summary>
<br/>

<img src="./eschema_1.png" width="100%" />

</details>

<details>
<summary><b>📄 Sheet 2 — Peripherals & Connectors</b></summary>
<br/>

<img src="./eschema_2.png" width="100%" />

</details>

</div>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 🏗️ PCB Layout — Layer by Layer

<div align="center">

<table>
<tr>
<td align="center" width="50%">

**🔴 Front Copper (F.Cu)**

<img src="./frontlayer_pcb.png" width="100%" />

</td>
<td align="center" width="50%">

**🔵 Back Copper (B.Cu)**

<img src="./Backlayer_pcb.png" width="100%" />

</td>
</tr>
<tr>
<td align="center" width="50%">

**🟡 Inner Layer 1 (In1.Cu)**

<img src="./in1cuLayer_pcb.png" width="100%" />

</td>
<td align="center" width="50%">

**🟢 Inner Layer 2 (In2.Cu)**

<img src="./in2cuLayer_pcb.png" width="100%" />

</td>
</tr>
</table>

<details>
<summary><b>🔎 Individual Layer Exports</b></summary>
<br/>

| Layer | Preview |
|:---:|:---:|
| **Layer 1** | <img src="./layer1.png" width="450" /> |
| **Layer 2** | <img src="./layer2.png" width="450" /> |
| **Layer 3** | <img src="./layer3.png" width="450" /> |
| **Layer 4** | <img src="./layer4.png" width="450" /> |

</details>

</div>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 🧱 Component & Composite Views

<div align="center">

<table>
<tr>
<td align="center" width="50%">

**🔩 All Layers Composite**

<img src="./AllLayers_pcb.png" width="100%" />

</td>
<td align="center" width="50%">

**📦 Components Only**

<img src="./OnlyComponents_pcb.png" width="100%" />

</td>
</tr>
<tr>
<td align="center" width="50%">

**🔲 All ICs Placement**

<img src="./All_ic_pcb.png" width="100%" />

</td>
<td align="center" width="50%">

**🔝 Front IC Placement**

<img src="./Front_IC_pcb.png" width="100%" />

</td>
</tr>
</table>

<details>
<summary><b>📸 Additional Composite Views</b></summary>
<br/>

| View | Preview |
|:---:|:---:|
| **PCB All Layers** | <img src="./pcb_all_layers.png" width="500" /> |
| **PCB Components Only** | <img src="./pcb_only_components.png" width="500" /> |

</details>

</div>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## ✅ Design Verification

<div align="center">

<table>
<tr>
<td align="center" width="50%">

**⚡ ERC — Electrical Rules Check**

<img src="./ERC.png" width="100%" />

</td>
<td align="center" width="50%">

**📐 DRC — Design Rules Check**

<img src="./DRC.png" width="100%" />

</td>
</tr>
<tr>
<td align="center" width="50%">

**🔕 ERC Excluded**

<img src="./excluded_ERC.png" width="100%" />

</td>
<td align="center" width="50%">

**📐 DRC PCB**

<img src="./DRC_PCB.png" width="100%" />

</td>
</tr>
</table>

</div>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 🏭 Manufacturing

<div align="center">

<table>
<tr>
<td align="center">

**🏭 JLCPCB Fabrication Output**

<img src="./JLPCB.png" width="600" />

</td>
</tr>
</table>

> Gerber files generated and validated for **JLCPCB** fabrication.
> 4-layer stackup with controlled impedance routing.

</div>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 📁 File Index

| File | Category | Description |
|:---|:---:|:---|
| `eschema_full.png` | 📝 Schematic | Full schematic overview |
| `eschema_1.png` | 📝 Schematic | Sheet 1 — MCU & Power |
| `eschema_2.png` | 📝 Schematic | Sheet 2 — Peripherals |
| `frontlayer_pcb.png` | 🏗️ PCB | Front copper layer |
| `Backlayer_pcb.png` | 🏗️ PCB | Back copper layer |
| `in1cuLayer_pcb.png` | 🏗️ PCB | Inner copper layer 1 |
| `in2cuLayer_pcb.png` | 🏗️ PCB | Inner copper layer 2 |
| `layer1–4.png` | 🏗️ PCB | Individual layer exports |
| `AllLayers_pcb.png` | 🧱 Composite | All layers overlaid |
| `All_ic_pcb.png` | 🧱 Composite | IC placement map |
| `Front_IC_pcb.png` | 🧱 Composite | Front-side IC placement |
| `OnlyComponents_pcb.png` | 🧱 Composite | Component outlines only |
| `pcb_all_layers.png` | 🧱 Composite | Full board composite |
| `pcb_only_components.png` | 🧱 Composite | Components overlay |
| `front_3d.png` | 🖼️ 3D | Front 3D render |
| `back_3d.png` | 🖼️ 3D | Back 3D render |
| `side_3d.png` | 🖼️ 3D | Side 3D render |
| `side_down_3d.png` | 🖼️ 3D | Bottom-side 3D render |
| `png_3dmodel.png` | 🖼️ 3D | Full 3D model export |
| `My_stm32f4ve.png` | 🖼️ 3D | Board photograph / render |
| `ERC.png` | ✅ Verify | Electrical rules check |
| `DRC.png` | ✅ Verify | Design rules check |
| `DRC_PCB.png` | ✅ Verify | PCB design rules check |
| `excluded_ERC.png` | ✅ Verify | ERC exclusions list |
| `JLPCB.png` | 🏭 Fab | JLCPCB manufacturing output |

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

<div align="center">

## 🪪 Attribution

Designed by **Sanjay G** &nbsp;·&nbsp; **eSim PCB Design Project** &nbsp;·&nbsp; **FOSSEE, IIT Bombay**

<br/>

![eSim](https://img.shields.io/badge/Made_with-eSim-2d1b69?style=for-the-badge&logo=open-source-initiative&logoColor=cd7f32)
![KiCad](https://img.shields.io/badge/Made_with-KiCad-314CB0?style=for-the-badge&logo=kicad&logoColor=white)
![JLCPCB](https://img.shields.io/badge/Fabricated_at-JLCPCB-cd7f32?style=for-the-badge)
![FOSSEE](https://img.shields.io/badge/FOSSEE-IIT_Bombay-1a1a2e?style=for-the-badge)

</div>

<!-- FOOTER WAVE -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,25:1a1a2e,50:2d1b69,100:cd7f32&height=120&section=footer" width="100%" />
