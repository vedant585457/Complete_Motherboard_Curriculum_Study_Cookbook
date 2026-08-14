# 📑 Full Curriculum Index — 95 / 96 Sections ✅

Complete catalog of all topics covered in the **Complete Motherboard Curriculum — Visual Study Cookbook**.

Legend: ✅ Done · ⏳ Pending (image pending next session) · 🔄 In progress (this session's limit)

> **Note:** One image is pending (7.21 — VRM Failure Diagnosis) due to the per-session image-generation limit. The textual content is captured in `visualizelearning/chapter-07-power-supply-vrm/7.21_VRM_Failure_Diagnosis_NOTE.md`; the handwritten-notes image will be generated in the next session.

---

## Chapter 01 — Motherboard Fundamentals (9 sections) ✅

| # | Section | Description | Image |
|---|---|---|---|
| 1.1 | What a Motherboard Is | The PCB that interconnects CPU, RAM, storage, peripherals. | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.1_What_a_Motherboard_Is.png) |
| 1.2 | Purpose of a Motherboard | Electrical/physical interconnection, power, communication. | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.2_Purpose_of_a_Motherboard.png) |
| 1.3 | Motherboard Architecture Overview | Layout of CPU socket, chipset, slots, I/O. | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.3_Motherboard_Architecture_Overview.png) |
| 1.4 | Major Subsystems | CPU, VRM, memory, PCH, storage, USB, audio, networking. | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.4_Major_Subsystems.png) |
| 1.5 | Signal Flow | Control/data signals between ICs. | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.5_Signal_Flow.png) |
| 1.6 | Data Flow | High-speed (PCIe/DDR) vs low-speed (SPI/I2C) data paths. | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.6_Data_Flow.png) |
| 1.7 | Power Flow | PSU through VRMs to each IC. | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.7_Power_Flow.png) |
| 1.8 | Component Communication | Buses (PCIe, SPI, SMBus). | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.8_Component_Communication.png) |
| 1.9 | Form Factors | ATX, mATX, Mini-ITX, etc. | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.9_Form_Factors.png) |

---

## Chapter 02 — Core Components & Interconnects (12 sections) ✅

| # | Section | Description | Image |
|---|---|---|---|
| 2.1 | CPU | Executes instructions; socket to power, memory, I/O. | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.1_CPU.png) |
| 2.2 | Chipset / PCH | Modern single-chip successor to NB/SB. | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.2_Chipset_PCH.png) |
| 2.3 | Northbridge / Southbridge (Legacy) | Two-chip legacy architecture. | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.3_Northbridge_Southbridge_Legacy.png) |
| 2.4 | Modern Chipset Architecture | PCH ↔ CPU via DMI; memory/PCIe on-die. | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.4_Modern_Chipset_Architecture.png) |
| 2.5 | Memory Controller (IMC) | On-CPU; manages DDR timing, channels. | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.5_Memory_Controller_IMC.png) |
| 2.6 | PCIe Root Complex | CPU-integrated logic originating PCIe. | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.6_PCIe_Root_Complex.png) |
| 2.7 | I/O Controllers | USB, SATA, audio, LAN. | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.7_IO_Controllers.png) |
| 2.8 | Embedded Controllers (EC) | Power sequencing, fans, keyboard. | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.8_Embedded_Controllers_EC.png) |
| 2.9 | Super I/O | Serial/parallel, fan control, hardware monitoring. | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.9_Super_IO.png) |
| 2.10 | Clock Generators | Reference clocks to CPU, PCIe, memory. | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.10_Clock_Generators.png) |
| 2.11 | Management Controllers (BMC) | Out-of-band management. | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.11_Management_Controllers_BMC.png) |
| 2.12 | Interconnects (DMI, FDI, etc.) | Proprietary buses linking CPU to PCH. | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.12_Interconnects_DMI_FDI.png) |

---

## Chapter 03 — CPU Socket, Power & Init (11 sections) ✅

| # | Section | Description | Image |
|---|---|---|---|
| 3.1 | CPU Socket | Mechanical/electrical interface (LGA, PGA, BGA). | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.1_CPU_Socket.png) |
| 3.2 | Socket Types | LGA1700, AM5, BGA — pin count/layout. | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.2_Socket_Types.png) |
| 3.3 | CPU Power Delivery | VRM supplies Vcore/SOC. | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.3_CPU_Power_Delivery.png) |
| 3.4 | CPU Buses/Interconnects | DMI, IF, ring bus. | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.4_CPU_Buses_Interconnects.png) |
| 3.5 | Memory Communication | Direct CPU-to-DIMM electrical paths. | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.5_Memory_Communication.png) |
| 3.6 | PCIe Communication | CPU-originated lanes to GPU/NVMe. | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.6_PCIe_Communication.png) |
| 3.7 | CPU Initialization | Power-up sequence. | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.7_CPU_Initialization.png) |
| 3.8 | Reset Signals | RESET#, PLTRST#. | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.8_Reset_Signals.png) |
| 3.9 | Power-Good Signals | PWR_OK confirmation. | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.9_Power_Good_Signals.png) |
| 3.10 | CPU Straps | Pin configurations at reset. | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.10_CPU_Straps.png) |
| 3.11 | Platform Initialization | Firmware-driven bring-up. | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.11_Platform_Initialization.png) |

---

## Chapter 04 — Chipset, Buses & Diagnosis (15 sections) ✅

| # | Section | Description | Image |
|---|---|---|---|
| 4.1 | Historical Chipset Architecture | Two-chip NB/SB design. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.1_Historical_Chipset_Architecture.png) |
| 4.2 | Northbridge | High-speed CPU/RAM/GPU hub. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.2_Northbridge.png) |
| 4.3 | Southbridge | Slow I/O hub, evolved into PCH. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.3_Southbridge.png) |
| 4.4 | Modern PCH | Single chip for remaining I/O. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.4_Modern_PCH.png) |
| 4.5 | Chipset Responsibilities | PCIe lanes, USB, SATA, audio, networking. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.5_Chipset_Responsibilities.png) |
| 4.6 | PCIe Lanes (Chipset) | Secondary lanes. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.6_PCIe_Lanes_Chipset.png) |
| 4.7 | USB (via chipset) | Chipset hosts most USB. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.7_USB_via_Chipset.png) |
| 4.8 | SATA (via chipset) | Native SATA controller. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.8_SATA_via_Chipset.png) |
| 4.9 | Audio (HDA link) | HDA link to codec. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.9_Audio_HDA_Link.png) |
| 4.10 | Networking | MAC or PCIe link to LAN/WiFi. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.10_Networking_Interfaces.png) |
| 4.11 | SPI (BIOS) | Chipset reads BIOS from SPI. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.11_SPI_Chipset_BIOS_Link.png) |
| 4.12 | SMBus | Low-speed sensors, SPD, power mgmt. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.12_SMBus.png) |
| 4.13 | LPC/eSPI | Legacy/modern low-pin-count buses. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.13_LPC_eSPI.png) |
| 4.14 | Chipset Initialization | Chipset bring-up during POST. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.14_Chipset_Initialization.png) |
| 4.15 | Chipset Failure Diagnosis | Isolate via rail and signal checks. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.15_Chipset_Failure_Diagnosis.png) |

---

## Chapter 05 — Memory, RAM & DDR (13 sections) ✅

| # | Section | Description | Image |
|---|---|---|---|
| 5.1 | DIMM Slots | Physical connectors, keying. | [📷](./visualizelearning/chapter-05-memory-ram-ddr/5.1_DIMM_Slots.png) |
| 5.2 | DDR Generations | DDR3/4/5 changes. | [📷](./visualizelearning/chapter-05-memory-ram-ddr/5.2_DDR_Generations.png) |
| 5.3 | Memory Channels | Parallel data paths. | [📷](./visualizelearning/chapter-05-memory-ram-ddr/5.3_Memory_Channels.png) |
| 5.4 | Dual/Multi-Channel | Matched DIMMs in correct slots. | [📷](./visualizelearning/chapter-05-memory-ram-ddr/5.4_Dual_Multi_Channel_Memory.png) |
| 5.5 | Memory Topology | Trace layout/length matching. | [📷](./visualizelearning/chapter-05-memory-ram-ddr/5.5_Memory_Topology.png) |
| 5.6 | Memory Training | BIOS calibration. | [📷](./visualizelearning/chapter-05-memory-ram-ddr/5.6_Memory_Training.png) |
| 5.7 | SPD | EEPROM with timing specs. | [📷](./visualizelearning/chapter-05-memory-ram-ddr/5.7_SPD_Serial_Presence_Detect.png) |
| 5.8 | EEPROM | Non-volatile storage. | [📷](./visualizelearning/chapter-05-memory-ram-ddr/5.8_EEPROM.png) |
| 5.9 | ECC | Error detection/correction. | [📷](./visualizelearning/chapter-05-memory-ram-ddr/5.9_ECC_Error_Correcting_Code.png) |
| 5.10 | Memory Signaling | Voltage/timing margins. | [📷](./visualizelearning/chapter-05-memory-ram-ddr/5.10_Memory_Signaling.png) |
| 5.11 | Termination | VTT vs ODT vs POD. | [📷](./visualizelearning/chapter-05-memory-ram-ddr/5.11_Termination.png) |
| 5.12 | Memory Power Rails | VDD, VPP, VTT. | [📷](./visualizelearning/chapter-05-memory-ram-ddr/5.12_Memory_Power_Rails.png) |
| 5.13 | Memory Failures | No POST, training fail, XMP. | [📷](./visualizelearning/chapter-05-memory-ram-ddr/5.13_Memory_Related_Failures.png) |

---

## Chapter 06 — PCIe Bus (15 sections) ✅

| # | Section | Description | Image |
|---|---|---|---|
| 6.1 | PCIe Fundamentals | Serial point-to-point bus. | [📷](./visualizelearning/chapter-06-pcie-bus/6.1_PCIe_Fundamentals.png) |
| 6.2 | PCIe Generations (3.0-6.0) | Each doubles bandwidth per lane. | [📷](./visualizelearning/chapter-06-pcie-bus/6.2_PCIe_Generations.png) |
| 6.3 | PCIe Lanes | Independent serial paths. | [📷](./visualizelearning/chapter-06-pcie-bus/6.3_PCIe_Lanes.png) |
| 6.4 | Lane Width | More lanes = more bandwidth. | [📷](./visualizelearning/chapter-06-pcie-bus/6.4_Lane_Width.png) |
| 6.5 | Root Complex | CPU-side origin of PCIe tree. | [📷](./visualizelearning/chapter-06-pcie-bus/6.5_Root_Complex.png) |
| 6.6 | Endpoints | Terminal PCIe devices. | [📷](./visualizelearning/chapter-06-pcie-bus/6.6_Endpoints.png) |
| 6.7 | Switches | Fan out limited CPU lanes. | [📷](./visualizelearning/chapter-06-pcie-bus/6.7_Switches.png) |
| 6.8 | Link Training | Auto-negotiation of speed/width. | [📷](./visualizelearning/chapter-06-pcie-bus/6.8_Link_Training.png) |
| 6.9 | Negotiation | Devices/host agree on parameters. | [📷](./visualizelearning/chapter-06-pcie-bus/6.9_Negotiation.png) |
| 6.10 | Signal Integrity (PCIe) | Sensitive to length/impedance. | [📷](./visualizelearning/chapter-06-pcie-bus/6.10_Signal_Integrity_PCIe.png) |
| 6.11 | PCIe Power | Slot + aux connectors. | [📷](./visualizelearning/chapter-06-pcie-bus/6.11_PCIe_Power.png) |
| 6.12 | PCIe Slot Architecture | Physical vs electrical lane count. | [📷](./visualizelearning/chapter-06-pcie-bus/6.12_PCIe_Slot_Architecture.png) |
| 6.13 | GPU Communication | High-bandwidth path for GPU. | [📷](./visualizelearning/chapter-06-pcie-bus/6.13_GPU_Communication.png) |
| 6.14 | NVMe Communication | SSDs use PCIe directly. | [📷](./visualizelearning/chapter-06-pcie-bus/6.14_NVMe_Communication.png) |
| 6.15 | PCIe Troubleshooting | No GPU, link degradation, code 43. | [📷](./visualizelearning/chapter-06-pcie-bus/6.15_PCIe_Troubleshooting.png) |

---

## Chapter 07 — Power Supply & VRM (20 / 21 sections) 🔄

| # | Section | Description | Image |
|---|---|---|---|
| 7.1 | ATX Power Supply Interface | 24-pin main, EPS12V CPU, PCIe, SATA power. | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.1_ATX_Power_Supply_Interface.png) |
| 7.2 | Rails (12V / 5V / 3.3V) | The three primary DC rails. | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.2_Rails_12V_5V_3V3.png) |
| 7.3 | Standby Power (5VSB) | Always-on rail for wake functions. | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.3_Standby_Power_5VSB.png) |
| 7.4 | VRM Fundamentals | DC-DC buck conversion, topology. | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.4_VRM_Fundamentals.png) |
| 7.5 | PWM Controllers | Switch-mode control IC. | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.5_PWM_Controllers.png) |
| 7.6 | MOSFETs | High-side and low-side switches. | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.6_MOSFETs.png) |
| 7.7 | DrMOS | Integrated driver + FET module. | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.7_DrMOS.png) |
| 7.8 | Power Stages | Smart Power Stage (SPS) packages. | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.8_Power_Stages.png) |
| 7.9 | Inductors | Energy storage element per phase. | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.9_Inductors.png) |
| 7.10 | Capacitors | Bulk + decoupling on the output. | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.10_Capacitors.png) |
| 7.11 | CPU Vcore | Primary core voltage, dynamically adjusted per load (VID). | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.11_CPU_Vcore.png) |
| 7.12 | SOC Voltage | Separate rail for IMC / uncore. | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.12_SOC_Voltage.png) |
| 7.13 | Memory Voltage | Dedicated VRM for DIMM power (VDD/VPP). | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.13_Memory_Voltage.png) |
| 7.14 | Chipset Power | Lower-current VRM stage for PCH. | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.14_Chipset_Power.png) |
| 7.15 | Load-Line Calibration (LLC) | Compensates voltage droop under load. | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.15_Load_Line_Calibration.png) |
| 7.16 | Power Sequencing | Order rails must turn on/off to protect ICs. | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.16_Power_Sequencing.png) |
| 7.17 | VRM Phases | Multiple parallel stages share current load. | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.17_VRM_Phases.png) |
| 7.18 | Transient Response | How fast VRM reacts to sudden load steps. | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.18_Transient_Response.png) |
| 7.19 | Efficiency | Power lost as heat during conversion. | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.19_Efficiency.png) |
| 7.20 | Thermal Management (VRM) | Heatsinks / airflow for VRM heat. | [📷](./visualizelearning/chapter-07-power-supply-vrm/7.20_Thermal_Management.png) |
| 7.21 | VRM Failure Diagnosis | No Vcore, won't boot, burnt MOSFETs — isolate. | ⏳ _pending (next session)_ |

> **7.21 status:** image pending generation. Full text content captured at [`7.21_VRM_Failure_Diagnosis_NOTE.md`](./visualizelearning/chapter-07-power-supply-vrm/7.21_VRM_Failure_Diagnosis_NOTE.md).

---

## 📊 Overall Progress

```
Chapter 01 ████████████████████ 9/9   ✅
Chapter 02 ████████████████████ 12/12 ✅
Chapter 03 ████████████████████ 11/11 ✅
Chapter 04 ████████████████████ 15/15 ✅
Chapter 05 ████████████████████ 13/13 ✅
Chapter 06 ████████████████████ 15/15 ✅
Chapter 07 ███████████████████░ 20/21 🔄
──────────────────────────────────────
Total       95/96 (99.0%) 🏁
```

---

_⬅️ Back to [README.md](./README.md)_
