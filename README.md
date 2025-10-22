# 🪸 Coral Restoration ROV - Integrated Nursery & Transplantation System

<div align="center">

[![Status](https://img.shields.io/badge/Status-Prototype-blue)](https://github.com/YourUsername/Coral-ROV)
[![University](https://img.shields.io/badge/University-Ocean%20University%20of%20China-blue)](http://www.ouc.edu.cn/)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

**瑚瑚生威 (Tiger Coral Power) - Autonomous Underwater Vehicle for Coral Reef Restoration**

[🎬 Watch Demos](#-demonstration-videos) · [💡 Key Innovations](#-key-innovations) · [🔧 System Design](#-system-architecture) · [🚀 Quick Start](#-quick-start)

---

### 🎥 Featured Demo: Complete System Underwater Rendering

[![ROV Underwater Demo](https://img.youtube.com/vi/fa-L6VtR9lE/maxresdefault.jpg)](https://youtu.be/fa-L6VtR9lE)

*Click to watch: Full ROV system underwater operation rendering*

</div>

---

## 📑 Table of Contents

<details open>
<summary><b>Click to expand/collapse navigation</b></summary>

### Quick Navigation

- **[🎯 Overview](#-overview)** - Project summary and key metrics
- **[📍 Background](#-background)** - Coral crisis and current solutions
- **[🎬 Demonstration Videos](#-demonstration-videos)** - All system demos
- **[💡 Key Innovations](#-key-innovations)** - 7 core technologies
  - [1. Coral Semantic SLAM](#1️⃣-coral-semantic-slam-mapping)
  - [2. Master-Slave Manipulator](#2️⃣-master-slave-teleoperation)
  - [3. Detachable Nursery Grid](#3️⃣-detachable-composite-nursery-grid)
  - [4. Intermittent Transmission](#4️⃣-intermittent-transmission-mechanism)
  - [5. Adaptive Crawler Tracks](#5️⃣-adaptive-crawler-track-system)
  - [6. Underwater Adhesive System](#6️⃣-underwater-adhesive-dispenser)
  - [7. VR Panoramic Visualization](#7️⃣-vr-panoramic-visualization)
- **[🔧 System Architecture](#-system-architecture)** - Hardware and software
- **[📊 Performance](#-performance-comparison)** - Benchmark results
- **[🚀 Quick Start](#-quick-start)** - Installation guide
- **[📂 Repository](#-repository-structure)** - Code organization
- **[👥 Team](#-team)** - Contributors and advisors
- **[📞 Contact](#-contact)** - Get in touch

</details>

---

## 🎯 Overview

An **integrated ROV system** automating the entire coral restoration lifecycle - from nursery grid deployment, growth monitoring, to mature coral transplantation. Addresses critical bottlenecks in traditional manual diving operations.

### Key Performance Metrics

| Metric | Specification | vs. Manual Diving |
|--------|--------------|-------------------|
| **Transplant Rate** | 8-10 corals/hour | **5× faster** |
| **Operating Depth** | 0-100 m | Exceeds 30m human limit |
| **Positioning Accuracy** | ±1 cm | 10× improvement |
| **Nursery Capacity** | 120 corals (10-layer grid) | Fully automated |

[⬆️ Back to top](#-coral-restoration-rov---integrated-nursery--transplantation-system)

---

## 📍 Background

### Global Coral Crisis

<div align="center">
<table>
<tr>
<td width="50%">

<img src="https://github.com/user-attachments/assets/f77854d6-4e98-4f39-93ff-57bbeace2e42" width="100%" alt="Coral Death"/>

**Figure 1**: Great Barrier Reef coral mortality

</td>
<td width="50%">

<img src="https://github.com/user-attachments/assets/83986d81-1358-42df-945d-6c74b28e2d23" width="100%" alt="Coral Bleaching"/>

**Figure 2**: Widespread coral bleaching events

</td>
</tr>
</table>
</div>

**Critical Facts**:
- **50% global coral cover lost** since 1980s
- Supports **10% of world fisheries** (~35 tons fish/km²/year)
- **500 million people** depend on coral reef ecosystems

### Current Solutions - Inadequate

<div align="center">

<img src="https://github.com/user-attachments/assets/150d4d7e-593f-4de5-97cf-47b19449170f" width="70%" alt="Manual Planting"/>

**Figure 3**: Traditional manual coral transplantation - low efficiency (2-3 corals/hour), high risk, weather-dependent

</div>

| Approach | Limitation |
|----------|------------|
| **Manual Diving** | 2-3 corals/hr, injury risks, depth limited (<30m) |
| **LarvalBot (Australia)** | Larvae dispersal only, <5% survival rate |
| **Nemo Robot** | Transport only, still requires divers for attachment |

[⬆️ Back to top](#-coral-restoration-rov---integrated-nursery--transplantation-system)

---

## 🎬 Demonstration Videos

<div align="center">

### 🤖 Master-Slave Manipulator Demo

[![Manipulator Demo](https://img.youtube.com/vi/X5DliNb6jgQ/maxresdefault.jpg)](https://youtu.be/X5DliNb6jgQ)

*Real-time teleoperation demonstration with tool quick-change capability*

---

### 🌀 Nursery Grid Deployment Demo

[![Grid Demo](https://img.youtube.com/vi/FdXD9Xdh4Wc/maxresdefault.jpg)](https://youtu.be/FdXD9Xdh4Wc)

*Intermittent transmission mechanism and tri-lock anchoring system in action*

---

### 🎥 Complete System Rendering

[![Full System](https://img.youtube.com/vi/fa-L6VtR9lE/maxresdefault.jpg)](https://youtu.be/fa-L6VtR9lE)

*Underwater operation rendering showing integrated workflow*

</div>

[⬆️ Back to top](#-coral-restoration-rov---integrated-nursery--transplantation-system)

---

## 💡 Key Innovations

### 1️⃣ Coral Semantic SLAM Mapping

**Technology**: Stereo camera + side-scan sonar fusion  
**Output**: Real-time 3D coral distribution heatmap with hard/soft coral classification  
**Accuracy**: ±50 cm positioning (solves underwater GPS-denied navigation)

**Applications**:
- Autonomous navigation and waypoint return
- Optimal transplantation site identification
- Long-term ecosystem health monitoring

[⬆️ Back to top](#-coral-restoration-rov---integrated-nursery--transplantation-system)

---

### 2️⃣ Master-Slave Teleoperation

<div align="center">
<table>
<tr>
<td width="50%">

<img src="https://github.com/user-attachments/assets/f7a2e52b-907a-49dc-94c8-d03af5fa299e" width="100%" alt="Slave Arm CAD"/>

**Figure 4a**: Underwater slave arm (5-DOF) CAD model

</td>
<td width="50%">

<img src="https://github.com/user-attachments/assets/b813813b-7d14-4c25-9f5a-8e7100f447dd" width="100%" alt="Slave Arm Photo"/>

**Figure 4b**: Physical prototype with gripper end-effector

</td>
</tr>
</table>

<img src="https://github.com/user-attachments/assets/98a10f54-3f7a-4aec-95ba-4f9866cd9143" width="80%" alt="Control Flow"/>

**Figure 5**: Master-slave control architecture - shore operator movements replicated underwater in real-time

</div>

**Features**:
- **5-DOF isomorphic control** with ±1 cm positioning precision
- **Magnetic quick-change interface**: Swap tools (gripper/drill/adhesive injector) in <30 seconds
- **Force feedback**: Current-based collision detection for safe manipulation

**Watch it in action**: [Master-Slave Manipulator Demo](https://youtu.be/X5DliNb6jgQ)

[⬆️ Back to top](#-coral-restoration-rov---integrated-nursery--transplantation-system)

---

### 3️⃣ Detachable Composite Nursery Grid

<div align="center">

<img src="https://github.com/user-attachments/assets/7ea643e4-3431-481f-8654-ea04db014454" width="70%" alt="Nursery Grid"/>

**Figure 6**: Reusable grid frame with biodegradable coral bases (PLA/PBAT material, 12-18 month degradation)

<table>
<tr>
<td width="50%">

<img src="https://github.com/user-attachments/assets/a236194c-29a3-4ce9-91fc-2710ab8ef884" width="100%" alt="Lock Open"/>

**Figure 7a**: Tri-lock mechanism in open position

</td>
<td width="50%">

<img src="https://github.com/user-attachments/assets/8e82beb2-1677-4b58-8074-72d9b63dae05" width="100%" alt="Lock Closed"/>

**Figure 7b**: Tri-lock rotated and secured to seabed mesh

</td>
</tr>
</table>
</div>

**Innovation Highlights**:
- **Reusable infrastructure**: Grid frame lasts 5+ years → **70% cost reduction**
- **Eco-friendly bases**: Biodegradable coral attachment points eliminate marine debris
- **Tri-lock anchoring**: Penetrates mesh, rotates to lock (no tools required)

**See deployment process**: [Nursery Grid Demo](https://youtu.be/FdXD9Xdh4Wc)

[⬆️ Back to top](#-coral-restoration-rov---integrated-nursery--transplantation-system)

---

### 4️⃣ Intermittent Transmission Mechanism

<div align="center">
<table>
<tr>
<td width="50%">

<img src="https://github.com/user-attachments/assets/6eeabbca-3de7-4af8-92ce-45fffc34e771" width="100%" alt="Grid Fixed"/>

**Figure 8a**: Grid locked in rack via 120° notches

</td>
<td width="50%">

<img src="https://github.com/user-attachments/assets/c554142b-8e55-460e-a2c5-13dde40478fb" width="100%" alt="Grid Released"/>

**Figure 8b**: Grid rotated and ready for gravity-assisted deployment

</td>
</tr>
</table>

<img src="https://github.com/user-attachments/assets/1fc17523-b79a-4f48-b07a-b6fba5e1f8a5" width="60%" alt="Rack Track"/>

**Figure 9**: Indexed rack track with 120° slots and chamfered entry (±5° misalignment tolerance)

</div>

**Working Principle**:
1. **Key rod** (servo-driven) rotates grids at fixed angles (120° Geneva-mechanism-inspired indexing)
2. Notch misalignment triggers gravity-assisted drop to next position
3. Enables **sequential 10-layer grid automation** without manual intervention

**Technical Details**:
- **Chamfered lead-in**: Compensates for ROV vibration during positioning
- **Fail-safe design**: Gravity-based release (no active mechanism to malfunction)
- **Dual function**: Same key rod controls tri-lock rotation

[⬆️ Back to top](#-coral-restoration-rov---integrated-nursery--transplantation-system)

---

### 5️⃣ Adaptive Crawler Track System

<div align="center">
<table>
<tr>
<td width="33%">

<img src="https://github.com/user-attachments/assets/240bfb4c-31d8-44be-b42c-bdc15c5c3300" width="100%" alt="Track Max"/>

**Figure 10a**: Maximum lift (transit mode)

</td>
<td width="33%">

<img src="https://github.com/user-attachments/assets/de41dce4-3eda-4e14-8ebe-2afa2bf4165b" width="100%" alt="Track Min"/>

**Figure 10b**: Minimum position (deployment mode)

</td>
<td width="33%">

<img src="https://github.com/user-attachments/assets/26e2ab37-1637-4843-bcf9-ca29bc351bae" width="100%" alt="Track Adapt"/>

**Figure 10c**: Spring suspension adapting to terrain

</td>
</tr>
</table>
</div>

**Key Features**:
- **80 mm vertical travel**: Stepper motor + lead screw for precise ROV height adjustment
- **Spring-loaded suspension**: Auto-compensates for 0-20.5 mm terrain variations
- **Dual purpose**: 
  - Lowers ROV to minimize grid drop distance during deployment
  - Reduces tri-lock insertion force through seabed mesh

**Performance Data**:
- Spring constant: 0.25 N/mm
- Maximum load capacity: 120 N (~12 kg)
- Traction force: 35 N on metal mesh structures

[⬆️ Back to top](#-coral-restoration-rov---integrated-nursery--transplantation-system)

---

### 6️⃣ Underwater Adhesive Dispenser

<div align="center">
<table>
<tr>
<td width="50%">

<img src="https://github.com/user-attachments/assets/12b5e6a8-e285-401c-8856-14d4ac6a1adc" width="100%" alt="Glue Nozzle"/>

**Figure 11a**: Siphon-inspired U-trap nozzle design

</td>
<td width="50%">

<img src="https://github.com/user-attachments/assets/21c3053b-c3b7-43eb-8f20-34541bbbfb07" width="100%" alt="Dispenser"/>

**Figure 11b**: Complete metering pump assembly

</td>
</tr>
</table>
</div>

**Innovation**: Plumbing P-trap inspired design prevents water intrusion into adhesive chamber

**Specifications**:
- **Adhesive type**: Two-part marine epoxy (5-minute underwater working time)
- **Dispensing volume**: 0.1-2 ml (programmable via stepper motor)
- **Nozzle sizes**: 0.5 mm (precision) / 2 mm (bulk bonding)
- **Bond strength**: >500 N shear force on limestone substrate

**Workflow Integration**:
1. Manipulator extracts coral base from grid
2. Nozzle dispenses metered adhesive
3. Coral pressed onto target reef location
4. 10-minute cure time before release

[⬆️ Back to top](#-coral-restoration-rov---integrated-nursery--transplantation-system)

---

### 7️⃣ VR Panoramic Visualization

<div align="center">

<img src="https://github.com/user-attachments/assets/5b6bdc55-be06-4989-81a5-f826d6376d9b" width="90%" alt="Panorama Stitching"/>

**Figure 12**: Real-time multi-camera stitching pipeline - (top) raw feeds from 3 cameras, (bottom) enhanced 180° panorama with CLAHE color correction

</div>

**Technical Achievement**:
- **Algorithm**: Joint enhancement-stitching CNN (published at **IEEE OCEANS 2024**)
- **Performance**: 180° FOV at 30 fps with <150 ms latency
- **Hardware**: 3× 1080p cameras + Raspberry Pi 4B processing

**User Experience**:
- **VR headset integration**: Immersive teleoperation with head-tracking
- **Real-time overlay**: Depth, attitude, battery status HUD
- **Interaction modes**: Gaze-based camera focus region selection

[⬆️ Back to top](#-coral-restoration-rov---integrated-nursery--transplantation-system)

---

## 🔧 System Architecture

<div align="center">

<img src="https://github.com/user-attachments/assets/1c573c7f-54bf-4110-8b6c-728555f5b5cd" width="70%" alt="ROV Render"/>

**Figure 13**: Complete ROV system rendering - frame structure with nursery rack, crawler tracks, and 5-DOF manipulator

<img src="https://github.com/user-attachments/assets/9997068a-2a63-4f1a-805a-0d653ed76f41" width="85%" alt="System Architecture"/>

**Figure 14**: Electronic system architecture - underwater subsystems connected to shore control via Ethernet tether

</div>

### Core Components

<details>
<summary><b>Click to expand hardware specifications</b></summary>

| Subsystem | Component | Specification | Function |
|-----------|-----------|---------------|----------|
| **Main Controller** | STM32F407ZGT6 | 168MHz ARM Cortex-M4F, 112 GPIO | Motor control, sensor fusion, safety logic |
| **Vision Computer** | Raspberry Pi 4B | Quad-core 1.5GHz, 4GB RAM | SLAM processing, image stitching, TCP/IP bridge |
| **Propulsion** | 6× T200 Thrusters | Blue Robotics, 5 kgf thrust each | 6-DOF underwater maneuvering |
| **Track Drive** | 2× NEMA 17 Steppers | 0.9° step angle, 40 N·cm torque | Seabed locomotion |
| **Lift Mechanism** | 2× Lead Screws + Steppers | 2 mm pitch, 80 mm travel | Vertical height adjustment |
| **Manipulator** | 5× Waterproof Servos | 20 kg·cm torque, PWM control | 5-DOF teleoperation |
| **Tool Changer** | Brushless Motor + Magnets | 3000 RPM, quick-release coupling | End-effector swapping |
| **Vision** | 3× Stereo Cameras | 1080p60, 120mm baseline | Depth perception, SLAM, panorama |
| **Sonar** | Side-scan Sonar | 200 kHz, 50m range | Seafloor mapping |
| **IMU** | MPU6050 | 6-axis gyro + accel | Attitude estimation |
| **Depth Sensor** | MS5837 | ±0.1 m accuracy | Depth hold control |
| **Power** | 24V 5Ah Li-ion | Custom battery pack | 4-6 hour endurance |
| **Regulators** | Multi-rail converters | 24V/12V/5V/3.3V outputs | Power distribution |
| **Safety** | Relays + Leak detectors | 10A contacts, IP68 sensors | Emergency shutdown |

</details>

### Software Architecture

<div align="center">

<img src="https://github.com/user-attachments/assets/702069e2-59cc-47a7-97a6-2ee6e6260d92" width="90%" alt="GUI"/>

**Figure 15**: Qt control interface - live video feeds (left), vehicle telemetry (center), mission planning map (right)

</div>

**Control Flow**:
```
Shore PC (Qt 5.12 C++)
    ↓ TCP/IP (Ethernet tether, 100 Mbps)
Raspberry Pi 4B (Ubuntu 20.04)
    ↓ UART (115200 baud)
STM32F407 (FreeRTOS)
    ↓ PWM/GPIO/I2C
Actuators & Sensors
```

**Key Software Modules**:
- **SLAM**: ORB-SLAM3 for visual-inertial odometry
- **Image Processing**: Custom CNN for stitching + CLAHE enhancement
- **Control**: PID depth/attitude hold (100 Hz update rate)
- **Communication**: Bi-directional telemetry + video streaming
- **Safety**: Watchdog timers, battery monitoring, leak detection

[⬆️ Back to top](#-coral-restoration-rov---integrated-nursery--transplantation-system)

---

## 📊 Performance Comparison

| Capability | Manual Diving | LarvalBot | Nemo Robot | **Our ROV** |
|------------|--------------|-----------|------------|-------------|
| **Transplant Rate** | 2-3 corals/hr | N/A | N/A | **8-10 corals/hr** ✅ |
| **Coral Survival** | 80% (nursery-grown) | <5% (larvae) | 80% | **80%** ✅ |
| **Max Depth** | <30 m (safety limit) | 0-100 m | 0-50 m | **0-100 m** ✅ |
| **Weather Dependency** | High (calm seas only) | Medium | Medium | **Low** ✅ |
| **Full Lifecycle** | ❌ (manual setup/retrieval) | ❌ (dispersal only) | ❌ (transport only) | **✅ Automated** |
| **Cost per Coral** | ¥80-150 | ¥200+ | ¥100+ | **¥40-60** ✅ |
| **Positioning Accuracy** | ±10 cm | N/A | N/A | **±1 cm** ✅ |

**Unique Advantages**:
- ✅ **Only system** with end-to-end automation (deployment → monitoring → transplantation)
- ✅ **5× efficiency gain** with equal coral survival rates
- ✅ **70% cost reduction** through reusable infrastructure
- ✅ **All-weather capability** removes seasonal constraints

[⬆️ Back to top](#-coral-restoration-rov---integrated-nursery--transplantation-system)

---

## 🚀 Quick Start

### Prerequisites

```bash
# System Requirements
- Ubuntu 20.04 LTS / Windows 10+
- Python 3.8+
- Qt 5.12+
- ARM GCC toolchain (for STM32)

# Clone Repository
git clone https://github.com/YourUsername/Coral-ROV.git
cd Coral-ROV

# Install Python Dependencies
pip install -r requirements.txt
# Key packages: numpy, opencv-python, pyserial, pyqt5, scipy
```

### Hardware Setup

<details>
<summary><b>Connection Guide</b></summary>

1. **STM32 Programming**:
   - Connect STM32F407 to PC via ST-Link V2
   - Verify connection: `st-info --probe`

2. **Raspberry Pi Network**:
   - Connect Pi to PC via Ethernet cable
   - Set static IP on Pi: `192.168.1.100`
   - Test connection: `ping 192.168.1.100`

3. **Input Devices**:
   - Plug Xbox controller into PC USB port
   - Connect master arm serial interface (COM port)

4. **Power System**:
   - Charge 24V battery pack to 25.2V (full charge)
   - Verify voltage regulators output correct levels
   - Test emergency stop relay

</details>

### Software Deployment

```bash
# 1. Flash STM32 Firmware
cd firmware/stm32_controller
make clean && make
make flash
# Verify: Blue LED should blink on board

# 2. Start Raspberry Pi Communication Bridge
ssh pi@192.168.1.100
cd ~/coral_rov
python3 rov_bridge.py
# Should output: "Waiting for STM32 connection..."

# 3. Launch Shore Control Station
cd ../../software/ground_station
python3 main_gui.py
# GUI should open with video feeds and telemetry
```

### First Test

<details>
<summary><b>System Checkout Procedure</b></summary>

1. **Thruster Test** (in water tank):
   - Move joystick forward → verify thrust direction
   - Test all 6 thrusters individually
   - Check for smooth PWM response

2. **Manipulator Calibration**:
   - Move master arm to home position
   - Click "Calibrate" in GUI
   - Verify slave arm mirrors movements

3. **Track System**:
   - Command lift to max position
   - Verify stepper motion (should hear steps)
   - Test spring suspension manually

4. **Grid Deployment** (dry test):
   - Load single test grid
   - Trigger key rod rotation
   - Confirm grid drops cleanly

</details>

**Full Documentation**: [docs/USER_MANUAL.md](docs/USER_MANUAL.md)

[⬆️ Back to top](#-coral-restoration-rov---integrated-nursery--transplantation-system)

---

## 📂 Repository Structure

```
Coral-ROV/
├── README.md                          # This file
├── LICENSE                            # MIT License
├── requirements.txt                   # Python dependencies
│
├── docs/                              # Documentation
│   ├── USER_MANUAL.md                # Detailed operation guide
│   ├── ASSEMBLY.md                   # Hardware build instructions
│   ├── TROUBLESHOOTING.md            # Common issues and fixes
│   └── API.md                        # Software API reference
│
├── hardware/                          # Mechanical & electrical designs
│   ├── cad/
│   │   ├── frame.SLDASM              # Main frame assembly
│   │   ├── nursery_grid.SLDPRT       # Grid design
│   │   ├── manipulator.SLDASM        # 5-DOF arm
│   │   ├── track_system.SLDASM       # Crawler mechanism
│   │   └── tri_lock.SLDPRT           # Anchoring system
│   ├── pcb/
│   │   ├── power_distribution/       # Multi-rail regulator
│   │   ├── motor_driver/             # Stepper/servo controllers
│   │   └── sensor_interface/         # IMU/depth sensor breakout
│   ├── stl/                          # 3D printable parts
│   └── BOM.xlsx                      # Complete bill of materials
│
├── firmware/                          # Embedded software
│   └── stm32_controller/
│       ├── Core/
│       │   ├── Src/
│       │   │   ├── main.c            # Main program loop
│       │   │   ├── motor_control.c   # Thruster/stepper PWM
│       │   │   ├── sensor_fusion.c   # IMU + depth Kalman filter
│       │   │   ├── pid_controller.c  # Depth/attitude hold
│       │   │   └── communication.c   # UART protocol handler
│       │   └── Inc/                  # Header files
│       ├── Drivers/                  # STM32 HAL libraries
│       └── Makefile                  # Build configuration
│
├── software/                          # Shore station software
│   ├── ground_station/
│   │   ├── main_gui.py               # Qt main window
│   │   ├── video_decoder.py          # H.264 stream handling
│   │   ├── mission_planner.py        # Waypoint editor
│   │   ├── telemetry_logger.py       # Data recording
│   │   └── gamepad_handler.py        # Xbox controller input
│   ├── slam/
│   │   ├── orb_slam3_wrapper.py      # Visual-inertial odometry
│   │   ├── semantic_seg.py           # Coral classification CNN
│   │   └── point_cloud_export.py     # 3D map generation
│   └── vr_interface/
│       ├── image_stitcher.py         # Multi-camera panorama
│       ├── vr_headset_driver.py      # Oculus Quest interface
│       └── clahe_enhancement.py      # Underwater color correction
│
├── simulation/                        # Testing & analysis tools
│   ├── gazebo/                       # ROS Gazebo ROV dynamics
│   └── matlab/                       # PID tuning scripts
│
└── scripts/                           # Utility tools
    ├── install_dependencies.sh        # One-click setup
    ├── calibrate_cameras.py          # Stereo calibration
    ├── test_communication.py         # Serial/TCP debugging
    └── battery_monitor.py            # Power consumption analyzer
```

[⬆️ Back to top](#-coral-restoration-rov---integrated-nursery--transplantation-system)

---

## 👥 Team

**Ocean University of China - Marine Robotics Laboratory**

<table>
<tr>
<td align="center" width="25%">
<b>Team Member 1</b><br>
<i>Project Lead</i><br>
Mechanical Design & System Integration<br>
📧 <a href="mailto:member1@stu.ouc.edu.cn">Email</a>
</td>
<td align="center" width="25%">
<b>Team Member 2</b><br>
<i>Embedded Systems Engineer</i><br>
STM32 Firmware & PCB Design<br>
📧 <a href="mailto:member2@stu.ouc.edu.cn">Email</a>
</td>
<td align="center" width="25%">
<b>Team Member 3</b><br>
<i>Computer Vision Specialist</i><br>
SLAM & Image Stitching Algorithms<br>
📧 <a href="mailto:member3@stu.ouc.edu.cn">Email</a>
</td>
<td align="center" width="25%">
<b>Team Member 4</b><br>
<i>Marine Biology Advisor</i><br>
Coral Ecology & Field Testing<br>
📧 <a href="mailto:member4@stu.ouc.edu.cn">Email</a>
</td>
</tr>
</table>

### Faculty Advisor

**Prof. [Advisor Name]**  
College of Engineering, Ocean University of China  
📧 advisor@ouc.edu.cn  
*Research Focus: Underwater Robotics, Autonomous Marine Systems*

---

## 🙏 Acknowledgments

**Funding Support**:
- National College Student Innovation Training Program (Grant No. XXXXXX)
- Ocean University of China Research Fund
- Shandong Provincial Marine Science & Technology Program

**Facilities & Partners**:
- OUC Underwater Robotics Testing Pool
- Sanya Coral Reef National Nature Reserve (field testing site access)
- National Supercomputing Center (SLAM algorithm development)

**Open-Source Software**:
- [ORB-SLAM3](https://github.com/UZ-SLAMLab/ORB_SLAM3) - Visual-inertial SLAM framework
- [OpenCV](https://opencv.org/) - Computer vision library
- [Qt](https://www.qt.io/) - Cross-platform GUI framework
- [STM32CubeMX](https://www.st.com/stm32cube) - STM32 code generation tool

**Special Thanks**:
- Local dive teams for operational guidance and safety protocols
- Marine conservation NGOs for coral ecology expertise
- GitHub community for code reviews and suggestions

[⬆️ Back to top](#-coral-restoration-rov---integrated-nursery--transplantation-system)

---

## 📄 Citation

If you use this work in your research, please cite:

```bibtex
@misc{coral_rov_2025,
  title={Tiger Coral Power: An Integrated ROV System for Automated 
         Coral Nursery Management and Reef Transplantation},
  author={[Team Member Names] and [Advisor Name]},
  year={2025},
  institution={Ocean University of China},
  howpublished={\url{https://github.com/YourUsername/Coral-ROV}},
  note={National Innovation Program - Open-source marine robotics project}
}
```

**Related Publications**:
- [Team Members]. "Underwater Image Enhancement and Stitching for ROV Applications." *IEEE OCEANS Conference*, 2024. [Link to paper]
- [In preparation] "Semantic SLAM for Coral Reef Mapping and Navigation"

---

## 📜 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

**Patent Status**: Provisional patent filed for tri-lock nursery grid system (CN202XXXXXXX.X)

**Commercial Use**: Permitted under MIT License. For partnership or licensing inquiries, please contact the team directly.

---

## 📞 Contact

**Project Lead**: [Your Name]  
**Affiliation**: College of Engineering, Ocean University of China  
**Email**: yourname@stu.ouc.edu.cn  
**GitHub**: [@YourUsername](https://github.com/YourUsername)

**Inquiries**:
- 🐛 **Bug Reports**: [GitHub Issues](https://github.com/YourUsername/Coral-ROV/issues)
- 💬 **Technical Discussions**: [GitHub Discussions](https://github.com/YourUsername/Coral-ROV/discussions)
- 🤝 **Collaboration Proposals**: Email directly
- 📰 **Media Requests**: media@ouc.edu.cn

---

<div align="center">

### ⭐ Star this repository to support ocean conservation! ⭐

**Help us restore coral reefs with robotics technology**

![GitHub stars](https://img.shields.io/github/stars/YourUsername/Coral-ROV?style=social)
![GitHub forks](https://img.shields.io/github/forks/YourUsername/Coral-ROV?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/YourUsername/Coral-ROV?style=social)

---

**Built with 💙 for Coral Reefs @ OUC Marine Robotics Lab**

**Last Updated**: January 2025 | **Version**: 1.0.0

---

### 🔗 Quick Links

[🎬 Watch Demos](#-demonstration-videos) · [💡 Innovations](#-key-innovations) · [🔧 Architecture](#-system-architecture) · [🚀 Get Started](#-quick-start) · [📂 Code](#-repository-structure) · [👥 Team](#-team) · [📞 Contact](#-contact)

---

[⬆️ Back to Top](#-coral-restoration-rov---integrated-nursery--transplantation-system)

</div>

---

**Dedicated to protecting Earth's coral reefs - one robot at a time 🪸🤖🌊**
