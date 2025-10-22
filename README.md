🪸 Coral Restoration ROV - Integrated Nursery & Transplantation System
<div align="center">
Status
University
License

瑚瑚生威 (Tiger Coral Power) - Autonomous Underwater Vehicle for Coral Reef Restoration

🎬 Demo · 📖 Docs · 💬 Contact

🎥 System Demonstration
<!-- Video placeholder - replace after upload -->
Demo Video

Complete workflow: Grid deployment → Growth monitoring → Coral transplantation

</div>
🎯 Overview
An integrated ROV system automating the entire coral restoration lifecycle - from nursery grid deployment, growth monitoring, to mature coral transplantation. Addresses critical bottlenecks in traditional manual diving operations.

Key Performance
Metric	Specification	vs. Manual Diving
Transplant Rate	8-10 corals/hour	5× faster
Operating Depth	0-100 m	Exceeds 30m human limit
Positioning Accuracy	±1 cm	10× improvement
Nursery Capacity	120 corals (10-layer grid)	Fully automated
📍 Background
Global Coral Crisis
<div align="center"> <table> <tr> <td width="50%"><img src="docs/images/fig-1-coral-death.jpg" width="100%" alt="Coral Death"/>
Figure 1: Great Barrier Reef coral mortality

</td> <td width="50%"><img src="docs/images/fig-2-coral-bleaching.jpg" width="100%" alt="Coral Bleaching"/>
Figure 2: Widespread coral bleaching events

</td> </tr> </table> </div>
Critical Facts:

50% global coral cover lost since 1980s
Supports 10% of world fisheries (~35 tons fish/km²/year)
500 million people depend on coral reef ecosystems
Current Solutions - Inadequate
<div align="center"><img src="docs/images/fig-3-manual-cultivation.jpg" width="70%" alt="Manual Planting"/>
Figure 3: Traditional manual coral transplantation - low efficiency (2-3 corals/hour), high risk, weather-dependent

</div>
Approach	Limitation
Manual Diving	2-3 corals/hr, injury risks, depth limited (<30m)
LarvalBot (Australia)	Larvae dispersal only, <5% survival rate
Nemo Robot	Transport only, still requires divers for attachment
💡 Key Innovations
1️⃣ Coral Semantic SLAM Mapping
Technology: Stereo camera + side-scan sonar fusion
Output: Real-time 3D coral distribution heatmap with hard/soft coral classification
Accuracy: ±50 cm positioning (solves underwater GPS-denied navigation)

2️⃣ Master-Slave Teleoperation
<div align="center"> <table> <tr> <td width="50%"><img src="docs/images/fig-22a-slave-arm-model.png" width="100%" alt="Slave Arm CAD"/>
Figure 4a: Underwater slave arm (5-DOF)

</td> <td width="50%"><img src="docs/images/fig-22b-slave-arm-physical.jpg" width="100%" alt="Slave Arm Photo"/>
Figure 4b: Physical prototype with gripper

</td> </tr> </table><img src="docs/images/fig-23-arm-control-flow.png" width="80%" alt="Control Flow"/>
Figure 5: Master-slave control architecture - shore operator controls replicated underwater in real-time

</div>
Features:

5-DOF isomorphic control with ±1 cm precision
Magnetic quick-change interface: Swap tools (gripper/drill/injector) in <30 seconds
3️⃣ Detachable Composite Nursery Grid
<div align="center"><img src="docs/images/fig-17-composite-grid.png" width="70%" alt="Nursery Grid"/>
Figure 6: Reusable grid frame with biodegradable coral bases (PLA/PBAT)

<table> <tr> <td width="50%"><img src="docs/images/fig-19-triangle-lock-open.png" width="100%" alt="Lock Open"/>
Figure 7a: Tri-lock open position

</td> <td width="50%"><img src="docs/images/fig-20-triangle-lock-closed.png" width="100%" alt="Lock Closed"/>
Figure 7b: Tri-lock closed and secured

</td> </tr> </table> </div>
Innovation:

Reusable grid (5-year lifespan) + biodegradable bases → 70% cost reduction
Tri-lock mechanism: Penetrates seabed mesh, rotates to lock grid in place
4️⃣ Intermittent Transmission Mechanism
<div align="center"> <table> <tr> <td width="50%"><img src="docs/images/fig-9-grid-fixed.jpg" width="100%" alt="Grid Fixed"/>
Figure 8a: Grid locked in rack (120° notches)

</td> <td width="50%"><img src="docs/images/fig-10-grid-released.jpg" width="100%" alt="Grid Released"/>
Figure 8b: Grid rotated and released

</td> </tr> </table><img src="docs/images/fig-11-rack-track.png" width="50%" alt="Rack Track"/>
Figure 9: Indexed rack track with 120° slots

</div>
Working Principle:

Key rod rotates grids at fixed angles (120° indexing)
Notch misalignment triggers gravity-assisted deployment
Enables sequential 10-layer grid automation
5️⃣ Adaptive Crawler Track System
<div align="center"> <table> <tr> <td width="33%"><img src="docs/images/fig-14-track-max.png" width="100%" alt="Track Max"/>
Figure 10a: Maximum lift

</td> <td width="33%"><img src="docs/images/fig-15-track-min.png" width="100%" alt="Track Min"/>
Figure 10b: Minimum position

</td> <td width="33%"><img src="docs/images/fig-16-track-deformation.png" width="100%" alt="Track Adapt"/>
Figure 10c: Terrain adaptation

</td> </tr> </table> </div>
Features:

80 mm vertical travel (stepper motor + lead screw)
Spring suspension: Auto-adjusts to 0-20.5 mm terrain variations
Purpose: Lower ROV to reduce grid drop height for tri-lock engagement
6️⃣ Underwater Adhesive Dispenser
<div align="center"> <table> <tr> <td width="50%"><img src="docs/images/fig-24-glue-nozzle.png" width="100%" alt="Glue Nozzle"/>
Figure 11a: Siphon-inspired U-trap nozzle (prevents water intrusion)

</td> <td width="50%"><img src="docs/images/fig-25-glue-dispenser.png" width="100%" alt="Dispenser"/>
Figure 11b: Complete metering pump system

</td> </tr> </table> </div>
Function: Dispenses measured marine epoxy for coral-to-reef bonding after gripper extraction

7️⃣ VR Panoramic Visualization
<div align="center"><img src="docs/images/fig-26-image-stitching.png" width="90%" alt="Panorama Stitching"/>
Figure 12: Real-time multi-camera stitching (180° FOV) with color enhancement for immersive VR teleoperation

</div>
Achievement: Algorithm published at IEEE OCEANS Conference 2024

🔧 System Architecture
<div align="center"><img src="docs/images/fig-7-rov-render.png" width="80%" alt="ROV Render"/>
Figure 13: Complete ROV system - frame structure with nursery rack, crawler tracks, and manipulator

<img src="docs/images/fig-27-system-diagram.png" width="90%" alt="System Architecture"/>
Figure 14: Electronic system architecture (underwater subsystems + shore control station)

</div>
Core Components
Subsystem	Component	Function
Main Controller	STM32F407ZGT6	Motor control, sensor fusion
Vision Computer	Raspberry Pi 4B	SLAM processing, TCP/IP bridge
Propulsion	6× T200 Thrusters	6-DOF underwater maneuvering
Actuation	Steppers + Servos + BLDC	Track drive, manipulator, tool changer
Sensing	Stereo camera + Sonar + IMU	Visual odometry, mapping, orientation
Power	24V 5Ah Li-ion	4-6 hour endurance
Software Stack
<div align="center"><img src="docs/images/fig-36-gui-interface.png" width="85%" alt="GUI"/>
Figure 15: Qt control interface - live video feeds, telemetry, mission planning

</div>
text

Shore PC (Qt 5.12)
    ↓ TCP/IP (Ethernet tether)
Raspberry Pi 4B
    ↓ UART (115200 baud)
STM32F407 (FreeRTOS)
    ↓ PWM/GPIO
Actuators (Motors/Servos/Relays)
🚀 Quick Start
Prerequisites
Bash

# System Requirements
- Ubuntu 20.04 / Windows 10+
- Python 3.8+
- Qt 5.12+

# Clone Repository
git clone https://github.com/YourUsername/Coral-ROV.git
cd Coral-ROV

# Install Dependencies
pip install -r requirements.txt
Hardware Setup
Connect STM32 via ST-Link to PC
Connect Raspberry Pi to PC via Ethernet (static IP: 192.168.1.100)
Plug in Xbox controller (USB)
Connect master arm via serial port
Run System
Bash

# 1. Flash STM32 Firmware
cd firmware/stm32_controller
make flash

# 2. Start Raspberry Pi Bridge
ssh pi@192.168.1.100
python3 ~/rov_bridge.py

# 3. Launch Control Station
cd software/ground_station
python3 main_gui.py
Full Documentation: docs/USER_MANUAL.md

📊 Performance Comparison
Capability	Manual Diving	LarvalBot	Our ROV
Transplant Rate	2-3/hr	N/A	8-10/hr ✅
Coral Survival	80%	<5%	80% ✅
Max Depth	<30 m	0-100 m	0-100 m ✅
Weather Dependency	High	Medium	Low ✅
Cost per Coral	¥80-150	¥200+	¥40-60 ✅
📂 Repository Structure
text

Coral-ROV/
├── README.md                   # This file
├── docs/
│   ├── images/                 # Figures
│   ├── USER_MANUAL.md         # Operation guide
│   └── ASSEMBLY.md            # Hardware build
├── hardware/
│   ├── cad/                    # SolidWorks files
│   ├── pcb/                    # Circuit designs
│   └── BOM.xlsx               # Bill of materials
├── firmware/
│   └── stm32_controller/      # Embedded code
├── software/
│   ├── ground_station/        # Qt GUI
│   ├── slam/                  # SLAM algorithms
│   └── vr_interface/          # Panorama stitching
└── scripts/                   # Utility tools
👥 Team
Ocean University of China - Marine Robotics Lab

Member	Role
Member 1	Project Lead - Mechanical Design & Control
Member 2	Embedded Systems - Firmware & PCB
Member 3	Computer Vision - SLAM & Image Processing
Member 4	Marine Biology - Coral Ecology Advisor
Faculty Advisor: Prof. [Name] - Underwater Robotics Research

🙏 Acknowledgments
Funding:

National College Student Innovation Program (Grant No. XXXXXX)
Ocean University of China Research Fund
Shandong Provincial Marine Technology Program
Partners:

Sanya Coral Reef National Nature Reserve (field testing site)
OUC Underwater Robotics Testing Facility
Open-source communities (ORB-SLAM3, OpenCV, Qt)
📄 Citation
bibtex

@misc{coral_rov_2025,
  title={Tiger Coral Power: Integrated ROV for Coral Restoration},
  author={[Team Members] and [Advisor]},
  year={2025},
  institution={Ocean University of China},
  howpublished={\url{https://github.com/YourUsername/Coral-ROV}}
}
Related Publication: Underwater Image Stitching - IEEE OCEANS 2024

📞 Contact
Project Lead: [Your Name]
Email: yourname@stu.ouc.edu.cn
GitHub: @YourUsername

Inquiries:

🐛 Issues: GitHub Issues
💬 Discussions: GitHub Discussions
📧 Collaboration: Direct email
<div align="center">
⭐ Star this repository to support ocean conservation! ⭐
GitHub stars

Built with 💙 for Coral Reefs @ OUC Marine Robotics Lab

Last Updated: January 2025 | Version: 1.0.0

🔝 Back to Top

</div>
