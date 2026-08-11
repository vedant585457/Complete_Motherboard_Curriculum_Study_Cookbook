# 📑 Full Curriculum Index — 47 Sections

Complete catalog of all topics covered in the **Complete Motherboard Curriculum — Visual Study Cookbook**.

Legend: ✅ Done · ⏳ Pending · 🔄 In progress (this session's limit)

---

## Chapter 01 — Motherboard Fundamentals (9 sections) ✅

| # | Section | Description | Image |
|---|---|---|---|
| 1.1 | What a Motherboard Is | The PCB that interconnects CPU, RAM, storage, peripherals via traces, buses, connectors. | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.1_What_a_Motherboard_Is.png) |
| 1.2 | Purpose of a Motherboard | Electrical/physical interconnection, power distribution, communication pathways. | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.2_Purpose_of_a_Motherboard.png) |
| 1.3 | Motherboard Architecture Overview | Layout of CPU socket, chipset, memory slots, expansion slots, I/O. | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.3_Motherboard_Architecture_Overview.png) |
| 1.4 | Major Subsystems | CPU, VRM, memory, PCH, storage, USB, audio, networking, firmware. | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.4_Major_Subsystems.png) |
| 1.5 | Signal Flow | Control/data signals between ICs (e.g., CPU↔PCH via DMI). | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.5_Signal_Flow.png) |
| 1.6 | Data Flow | High-speed (PCIe/DDR) vs low-speed (SPI/I2C) data paths. | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.6_Data_Flow.png) |
| 1.7 | Power Flow | PSU connectors through VRMs to each IC. | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.7_Power_Flow.png) |
| 1.8 | Component Communication | Buses (PCIe, SPI, SMBus) let ICs exchange data/commands. | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.8_Component_Communication.png) |
| 1.9 | Form Factors | ATX, mATX, Mini-ITX, etc. — physical size/mounting standards. | [📷](./visualizelearning/chapter-01-motherboard-fundamentals/1.9_Form_Factors.png) |

---

## Chapter 02 — Core Components & Interconnects (12 sections) ✅

| # | Section | Description | Image |
|---|---|---|---|
| 2.1 | CPU | Executes instructions; connects via socket to power, memory, I/O. | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.1_CPU.png) |
| 2.2 | Chipset / PCH | Modern single-chip successor to Northbridge/Southbridge; manages I/O, storage, USB. | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.2_Chipset_PCH.png) |
| 2.3 | Northbridge / Southbridge (Legacy) | Northbridge = CPU/RAM/GPU; Southbridge = slower I/O. Mostly absorbed. | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.3_Northbridge_Southbridge_Legacy.png) |
| 2.4 | Modern Chipset Architecture | PCH connects to CPU via DMI, handles I/O since memory/PCIe moved on-die. | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.4_Modern_Chipset_Architecture.png) |
| 2.5 | Memory Controller (IMC) | Integrated into CPU; manages DDR read/write timing and channels. | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.5_Memory_Controller_IMC.png) |
| 2.6 | PCIe Root Complex | CPU-integrated logic that originates PCIe transactions to GPU/NVMe/chipset. | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.6_PCIe_Root_Complex.png) |
| 2.7 | I/O Controllers | Manage USB, SATA, audio, LAN — mostly housed in PCH. | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.7_IO_Controllers.png) |
| 2.8 | Embedded Controllers (EC) | Microcontroller handling power sequencing, fans, keyboard (laptops). | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.8_Embedded_Controllers_EC.png) |
| 2.9 | Super I/O | Legacy chip managing serial/parallel ports, fan control, hardware monitoring. | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.9_Super_IO.png) |
| 2.10 | Clock Generators | Provide reference clocks to CPU, PCIe, memory. Critical for synchronized operation. | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.10_Clock_Generators.png) |
| 2.11 | Management Controllers (BMC) | Out-of-band management, remote diagnostics, independent of main CPU. | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.11_Management_Controllers_BMC.png) |
| 2.12 | Interconnects (DMI, FDI, etc.) | Proprietary buses linking CPU to PCH; bandwidth/latency implications. | [📷](./visualizelearning/chapter-02-core-components-interconnects/2.12_Interconnects_DMI_FDI.png) |

---

## Chapter 03 — CPU Socket, Power & Init (11 sections) ✅

| # | Section | Description | Image |
|---|---|---|---|
| 3.1 | CPU Socket | Mechanical/electrical interface (LGA, PGA, BGA) connecting CPU pins/pads to board. | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.1_CPU_Socket.png) |
| 3.2 | Socket Types | LGA1700, AM5, BGA, etc. — pin count/layout determines compatibility. | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.2_Socket_Types.png) |
| 3.3 | CPU Power Delivery | VRM supplies regulated Vcore/SOC voltage through socket power pins. | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.3_CPU_Power_Delivery.png) |
| 3.4 | CPU Buses/Interconnects | DMI, Infinity Fabric, ring bus — internal/external CPU communication paths. | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.4_CPU_Buses_Interconnects.png) |
| 3.5 | Memory Communication | Direct CPU-to-DIMM electrical paths; latency-sensitive routing. | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.5_Memory_Communication.png) |
| 3.6 | PCIe Communication | CPU-originated lanes to GPU/NVMe, bypassing chipset for speed. | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.6_PCIe_Communication.png) |
| 3.7 | CPU Initialization | Power-up sequence before instruction execution begins; reset de-assertion timing. | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.7_CPU_Initialization.png) |
| 3.8 | Reset Signals (RESET#, PLTRST#) | Force known state on power-up or fault; must sequence correctly. | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.8_Reset_Signals.png) |
| 3.9 | Power-Good Signals (PWR_OK) | Confirms stable voltage before allowing next stage to proceed. | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.9_Power_Good_Signals.png) |
| 3.10 | CPU Straps | Pin configurations sampled at reset defining CPU boot mode/features. | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.10_CPU_Straps.png) |
| 3.11 | Platform Initialization | Firmware-driven bring-up of CPU, memory, chipset before OS handoff. | [📷](./visualizelearning/chapter-03-cpu-socket-power-init/3.11_Platform_Initialization.png) |

---

## Chapter 04 — Chipset, Buses & Diagnosis (15 sections) ✅

| # | Section | Description | Image |
|---|---|---|---|
| 4.1 | Historical Chipset Architecture | Two-chip Northbridge/Southbridge design; explains legacy board layouts. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.1_Historical_Chipset_Architecture.png) |
| 4.2 | Northbridge | Handled high-speed CPU/RAM/GPU links; now obsolete on modern boards. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.2_Northbridge.png) |
| 4.3 | Southbridge | Handled slow I/O (USB, SATA, audio); evolved into PCH. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.3_Southbridge.png) |
| 4.4 | Modern PCH | Single chip for remaining I/O after CPU absorbed memory/PCIe controllers. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.4_Modern_PCH.png) |
| 4.5 | Chipset Responsibilities | Provides extra PCIe lanes, USB ports, SATA, audio codec interface, networking. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.5_Chipset_Responsibilities.png) |
| 4.6 | PCIe Lanes (Chipset-provided) | Secondary lanes for M.2/expansion slots, slower than CPU-direct lanes. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.6_PCIe_Lanes_Chipset.png) |
| 4.7 | USB (via chipset) | Chipset hosts most rear/front-panel USB ports. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.7_USB_via_Chipset.png) |
| 4.8 | SATA (via chipset) | Native SATA controller for HDD/SSD connections. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.8_SATA_via_Chipset.png) |
| 4.9 | Audio Interface (HDA link) | Chipset connects to audio codec via HD Audio bus. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.9_Audio_HDA_Link.png) |
| 4.10 | Networking Interfaces | Chipset provides MAC or PCIe link to LAN/Wi-Fi controllers. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.10_Networking_Interfaces.png) |
| 4.11 | SPI (Chipset-BIOS link) | Chipset reads BIOS/UEFI firmware from SPI flash at boot. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.11_SPI_Chipset_BIOS_Link.png) |
| 4.12 | SMBus | Low-speed bus for sensors, SPD (RAM), and power management communication. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.12_SMBus.png) |
| 4.13 | LPC/eSPI | Legacy/modern low-pin-count buses connecting Super I/O and EC to chipset. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.13_LPC_eSPI.png) |
| 4.14 | Chipset Initialization | Sequence of chipset bring-up during POST; dependency for I/O availability. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.14_Chipset_Initialization.png) |
| 4.15 | Chipset Failure Diagnosis | Symptoms include missing USB/SATA/audio; isolate via rail and signal checks. | [📷](./visualizelearning/chapter-04-chipset-buses-diagnosis/4.15_Chipset_Failure_Diagnosis.png) |

---

## 📊 Overall Progress

```
Chapter 01 ████████████████████ 9/9    ✅
Chapter 02 ████████████████████ 12/12  ✅
Chapter 03 ████████████████████ 11/11  ✅
Chapter 04 ████████████████████ 15/15 ✅
─────────────────────────────────────
Total       47/47 (100.0%) 🎉
```

---

_⬅️ Back to [README.md](./README.md)_
