# 🖥️ Complete Motherboard Curriculum — Visual Study Cookbook

> A **110-section deep-dive** into motherboard design, architecture, signals, power, sequencing, and troubleshooting — visualized as dense, handwritten-style chalkboard study notes.

Each topic is rendered as a **detailed technical illustration** on a **black background with white text**, packed edge-to-edge with definitions, diagrams, part numbers, voltages, frequencies, troubleshooting tips, and comparison tables — the way an engineering student would scribble them on a blackboard.

---

## 📚 Curriculum Structure

| Chapter | Topic | Sections | Status |
|---|---|---|---|
| **01** | Motherboard Fundamentals | 1.1 – 1.9 | ✅ Complete (9 / 9) |
| **02** | Core Components & Interconnects | 2.1 – 2.12 | ✅ Complete (12 / 12) |
| **03** | CPU Socket, Power & Init | 3.1 – 3.11 | ✅ Complete (11 / 11) |
| **04** | Chipset, Buses & Diagnosis | 4.1 – 4.15 | ✅ Complete (15 / 15) |
| **05** | Memory, RAM & DDR | 5.1 – 5.13 | ✅ Complete (13 / 13) |
| **06** | PCIe Bus | 6.1 – 6.15 | ✅ Complete (15 / 15) |
| **07** | Power Supply & VRM | 7.1 – 7.21 | 🔄 20 / 21 (1 image pending) |
| **08** | Power Sequencing & ACPI States | 8.1 – 8.14 | 🔄 10 / 14 (4 images pending) |

> Total: **110 sections** across 8 chapters (originally specified as ~35 topics; final delivered = 110 sections, 5 images pending for next session)

---

## 🗂️ Repository Layout

```
Complete_Motherboard_Curriculum_Study_Cookbook/
│
├── README.md                          ← You are here
├── INDEX.md                           ← Full topic index with descriptions
│
└── visualizelearning/                 ← All generated study-note images
    │
    ├── chapter-01-motherboard-fundamentals/
    │   ├── 1.1 ... 1.9                ✅ 9 PNGs
    │
    ├── chapter-02-core-components-interconnects/
    │   └── 2.1 ... 2.12                ✅ 12 PNGs (Chapter 2 complete)
    │
    ├── chapter-03-cpu-socket-power-init/
    │   └── 3.1 ... 3.11                ✅ 11 PNGs (Chapter 3 complete)
    │
    ├── chapter-04-chipset-buses-diagnosis/
    │   └── 4.1 ... 4.15                ✅ 15 PNGs (Chapter 4 complete)
```

---

## ✅ Chapter 01 — Motherboard Fundamentals (Complete)

| # | Section | Image | Description |
|---|---|---|---|
| 1.1 | What a Motherboard Is | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.1_What_a_Motherboard_Is.png) | The PCB that interconnects CPU, RAM, storage, peripherals via traces, buses, connectors. |
| 1.2 | Purpose of a Motherboard | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.2_Purpose_of_a_Motherboard.png) | Electrical interconnection, power distribution, communication pathways. |
| 1.3 | Architecture Overview | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.3_Motherboard_Architecture_Overview.png) | Layout of CPU socket, chipset, memory slots, expansion slots, I/O. |
| 1.4 | Major Subsystems | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.4_Major_Subsystems.png) | CPU, VRM, memory, PCH, storage, USB, audio, networking, firmware. |
| 1.5 | Signal Flow | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.5_Signal_Flow.png) | Control/data signals between ICs (CPU↔PCH via DMI, etc.). |
| 1.6 | Data Flow | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.6_Data_Flow.png) | High-speed (PCIe/DDR) vs low-speed (SPI/I2C) data paths. |
| 1.7 | Power Flow | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.7_Power_Flow.png) | PSU → 24-pin → VRMs → every IC. Dead-board troubleshooting. |
| 1.8 | Component Communication | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.8_Component_Communication.png) | Buses (PCIe, SPI, SMBus, I2C, UART, DMI) for IC communication. |
| 1.9 | Form Factors | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.9_Form_Factors.png) | ATX, mATX, Mini-ITX, E-ATX, SSI CEB/EEB, Mini-STX, NUC. |

---

## ✅ Chapter 03 — CPU Socket, Power & Init (Complete: 11/11)

| # | Section | Image | Description |
|---|---|---|---|
| 3.1 | CPU Socket | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.1_CPU_Socket.png) | Mechanical/electrical interface (LGA, PGA, BGA) connecting CPU to board. |
| 3.2 | Socket Types | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.2_Socket_Types.png) | LGA1700, AM5, BGA — pin count/layout determines compatibility. |
| 3.3 | CPU Power Delivery | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.3_CPU_Power_Delivery.png) | VRM supplies regulated Vcore/SOC voltage through socket power pins. |
| 3.4 | CPU Buses/Interconnects | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.4_CPU_Buses_Interconnects.png) | DMI, Infinity Fabric, ring bus — internal/external CPU paths. |
| 3.5 | Memory Communication | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.5_Memory_Communication.png) | Direct CPU-to-DIMM electrical paths; latency-sensitive routing. |
| 3.6 | PCIe Communication | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.6_PCIe_Communication.png) | CPU-originated lanes to GPU/NVMe, bypassing chipset. |
| 3.7 | CPU Initialization | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.7_CPU_Initialization.png) | Power-up sequence before instruction execution; reset de-assertion timing. |
| 3.8 | Reset Signals (RESET#, PLTRST#) | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.8_Reset_Signals.png) | Force known state on power-up or fault; must sequence correctly. |
| 3.9 | Power-Good Signals (PWR_OK) | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.9_Power_Good_Signals.png) | Confirms stable voltage before allowing next stage. |
| 3.10 | CPU Straps | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.10_CPU_Straps.png) | Pin configurations sampled at reset defining boot mode. |
| 3.11 | Platform Initialization | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.11_Platform_Initialization.png) | Firmware-driven bring-up of CPU, memory, chipset before OS handoff. |

| # | Section | Image | Description |
|---|---|---|---|
| 2.1 | CPU | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.1_CPU.png) | Executes instructions; socket to power, memory, I/O. |
| 2.2 | Chipset / PCH | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.2_Chipset_PCH.png) | Modern single-chip successor to Northbridge/Southbridge. |
| 2.3 | Northbridge / Southbridge (Legacy) | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.3_Northbridge_Southbridge_Legacy.png) | Two-chip legacy architecture now mostly absorbed. |
| 2.4 | Modern Chipset Architecture | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.4_Modern_Chipset_Architecture.png) | PCH ↔ CPU via DMI; memory/PCIe now on-die. |
| 2.5 | Memory Controller (IMC) | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.5_Memory_Controller_IMC.png) | On-CPU; manages DDR timing, channels, training. |
| 2.6 | PCIe Root Complex | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.6_PCIe_Root_Complex.png) | CPU-integrated logic originating PCIe transactions. |
| 2.7 | I/O Controllers | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.7_IO_Controllers.png) | USB, SATA, audio, LAN — mostly in PCH. |
| 2.8 | Embedded Controllers (EC) | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.8_Embedded_Controllers_EC.png) | Power sequencing, fans, keyboard (laptops). |
| 2.9 | Super I/O | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.9_Super_IO.png) | Serial/parallel, fan control, hardware monitoring. |
| 2.10 | Clock Generators | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.10_Clock_Generators.png) | Reference clocks to CPU, PCIe, memory. |
| 2.11 | Management Controllers (BMC) | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.11_Management_Controllers_BMC.png) | Out-of-band management, remote diagnostics. |
| 2.12 | Interconnects (DMI, FDI, etc.) | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.12_Interconnects_DMI_FDI.png) | Proprietary buses linking CPU to PCH. |

---

## 🔄 Chapter 07 — Power Supply & VRM (20 / 21 Complete)

| # | Section | Image | Description |
|---|---|---|---|
| 7.1 | ATX Power Supply Interface | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.1_ATX_Power_Supply_Interface.png) | 24-pin main, EPS12V CPU, PCIe, SATA power. |
| 7.2 | Rails (12V / 5V / 3.3V) | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.2_Rails_12V_5V_3V3.png) | The three primary DC rails. |
| 7.3 | Standby Power (5VSB) | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.3_Standby_Power_5VSB.png) | Always-on rail for wake functions. |
| 7.4 | VRM Fundamentals | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.4_VRM_Fundamentals.png) | DC-DC buck conversion, topology. |
| 7.5 | PWM Controllers | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.5_PWM_Controllers.png) | Switch-mode control IC. |
| 7.6 | MOSFETs | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.6_MOSFETs.png) | High-side and low-side switches. |
| 7.7 | DrMOS | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.7_DrMOS.png) | Integrated driver + FET module. |
| 7.8 | Power Stages | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.8_Power_Stages.png) | Smart Power Stage (SPS) packages. |
| 7.9 | Inductors | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.9_Inductors.png) | Energy storage element per phase. |
| 7.10 | Capacitors | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.10_Capacitors.png) | Bulk + decoupling on the output. |
| 7.11 | CPU Vcore | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.11_CPU_Vcore.png) | Primary core voltage, dynamically adjusted per load (VID). |
| 7.12 | SOC Voltage | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.12_SOC_Voltage.png) | Separate rail for IMC / uncore. |
| 7.13 | Memory Voltage | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.13_Memory_Voltage.png) | Dedicated VRM for DIMM power (VDD/VPP). |
| 7.14 | Chipset Power | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.14_Chipset_Power.png) | Lower-current VRM stage for PCH. |
| 7.15 | Load-Line Calibration (LLC) | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.15_Load_Line_Calibration.png) | Compensates voltage droop under load. |
| 7.16 | Power Sequencing | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.16_Power_Sequencing.png) | Order rails must turn on/off to protect ICs. |
| 7.17 | VRM Phases | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.17_VRM_Phases.png) | Multiple parallel stages share current load. |
| 7.18 | Transient Response | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.18_Transient_Response.png) | How fast VRM reacts to sudden load steps. |
| 7.19 | Efficiency | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.19_Efficiency.png) | Power lost as heat during conversion. |
| 7.20 | Thermal Management (VRM) | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.20_Thermal_Management.png) | Heatsinks / airflow for VRM heat. |
| 7.21 | VRM Failure Diagnosis | ⏳ _pending (next session)_ — [textual content](./visualizelearning/chapter-07-power-supply-vrm/7.21_VRM_Failure_Diagnosis_NOTE.md) | No Vcore, won't boot, burnt MOSFETs — isolate. |

---

## 🔄 Chapter 08 — Power Sequencing & ACPI States (10 / 14 Complete)

| # | Section | Image | Description |
|---|---|---|---|
| 8.1 | ACPI States Overview | [📷](./visualizelearning/chapter-08-power-sequencing-states/8.1_ACPI_States_Overview.png) | Standardized power states (G/S/C/D) defining system power behavior. |
| 8.2 | G3 (Mechanical Off) | [📷](./visualizelearning/chapter-08-power-sequencing-states/8.2_G3_Mechanical_Off.png) | No power except possibly RTC battery. |
| 8.3 | S5 (Soft Off) | [📷](./visualizelearning/chapter-08-power-sequencing-states/8.3_S5_Soft_Off.png) | Standby power present, main rails off; wake-on-LAN possible. |
| 8.4 | S3 (Suspend to RAM) | [📷](./visualizelearning/chapter-08-power-sequencing-states/8.4_S3_Suspend_to_RAM.png) | RAM retains state on minimal power; fast resume. |
| 8.5 | S0 (Fully On) | [📷](./visualizelearning/chapter-08-power-sequencing-states/8.5_S0_Fully_On.png) | Normal operating state, all rails active. |
| 8.6 | Power Button Signal | [📷](./visualizelearning/chapter-08-power-sequencing-states/8.6_Power_Button_Signal.png) | Momentary switch signals EC/SuperIO to begin power-on sequence. |
| 8.7 | PS_ON# | [📷](./visualizelearning/chapter-08-power-sequencing-states/8.7_PS_ON.png) | Signal from motherboard to PSU requesting main rails activate. |
| 8.8 | PWR_OK | [📷](./visualizelearning/chapter-08-power-sequencing-states/8.8_PWR_OK.png) | PSU confirms stable output before motherboard proceeds with boot. |
| 8.9 | Reset Signals | [📷](./visualizelearning/chapter-08-power-sequencing-states/8.9_Reset_Signals.png) | Ensure all ICs start in known state; must de-assert in correct order. |
| 8.10 | Voltage Rail Sequencing | [📷](./visualizelearning/chapter-08-power-sequencing-states/8.10_Voltage_Rail_Sequencing.png) | Rails must power up/down in specific order per IC datasheets. |
| 8.11 | Enable Signals | ⏳ _pending (next session)_ | GPIO lines that turn on individual VRM stages in sequence. |
| 8.12 | Power Controllers (Sequencers) | ⏳ _pending (next session)_ | Dedicated ICs enforcing correct rail sequencing. |
| 8.13 | CPU Startup Sequence | ⏳ _pending (next session)_ | From PWR_OK to first instruction fetch; multi-stage process. |
| 8.14 | POST Power Sequence | ⏳ _pending (next session)_ | Power stabilizes before firmware begins hardware initialization. |

---

## 🎨 Visual Style

- **Format:** PNG images
- **Background:** Pure black (`#000000`)
- **Text:** Pure white (`#FFFFFF`) chalk-style handwriting
- **Layout:** Edge-to-edge dense notes with:
  - Hand-drawn boxes, arrows, circles, underlines
  - Block diagrams, flowcharts, comparison tables
  - Real part numbers, voltages, frequencies, bandwidths
  - Practical troubleshooting checklists
  - Doodles & icons for visual anchoring

---

## 🚀 How to Use

1. **Browse chapter folders** under `visualizelearning/`
2. **Open any PNG** for a full-screen detailed study note
3. Use `INDEX.md` for the complete topic catalog with descriptions
4. New sections are added chapter-by-chapter — **watch this repo** for updates

---

## 📌 Progress Tracker

- [x] **Chapter 01 — Motherboard Fundamentals** (9 / 9 sections) ✅
- [x] **Chapter 02 — Core Components & Interconnects** (12 / 12 sections) ✅
- [x] **Chapter 03 — CPU Socket, Power & Init** (11 / 11 sections) ✅
- [x] **Chapter 04 — Chipset, Buses & Diagnosis** (15 / 15 sections) ✅
- [x] **Chapter 05 — Memory, RAM & DDR** (13 / 13 sections) ✅
- [x] **Chapter 06 — PCIe Bus** (15 / 15 sections) ✅
- [🔄] **Chapter 07 — Power Supply & VRM** (20 / 21 sections) — 1 image pending for next session
- [🔄] **Chapter 08 — Power Sequencing & ACPI States** (10 / 14 sections) — 4 images pending for next session

**Total:** 105 / 110 sections complete (95.5%) 🏁

_Note: User originally specified ~35 sections; final delivered = 110 unique topics (9+12+11+15+13+15+21+14) across 8 chapters. 105 images generated and live on GitHub; five images (7.21, 8.11, 8.12, 8.13, 8.14) are queued for the next session due to the per-session image-generation limit._

---

_Made with ❤️ for hardware enthusiasts, PC builders, and motherboard engineers._
