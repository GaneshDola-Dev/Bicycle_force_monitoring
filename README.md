# Bicycle_force_monitoring
Embedded system for real-time force and rotation monitoring using STM32G431, KD40S sensor, and IR slot sensor. Includes treadmill motor diagnostics and OLED visualization via SPI.

Bicycle Testing with Integrated Force & Motion Monitoring
Embedded Systems • Sensor Integration • STM32 • Real‑Time Data Acquisition
This project presents a custom‑built treadmill‑based bicycle testing platform designed to measure dynamic forces, motor speed, and rotational behavior in real time.
It was developed as part of the ZEETA research initiative, focusing on adaptive control for single‑track electric trailers.

📌 Project Overview
The system integrates:
  - A KD40S tri‑axial force sensor for real‑time force measurement
  - A precision‑modified treadmill motor for controlled bicycle testing
  - An infrared slot sensor for rotation and RPM detection
  - An STM32G431 Nucleo‑64 microcontroller for embedded processing
  - A 0.96‑inch RGB OLED display (SSD1357) for live visualization
The goal is to analyze bicycle dynamics under controlled conditions and support research in adaptive trailer control, safety, and performance optimization.

🧩 System Architecture
1. Mechanical Subsystem
  -	Custom test rig built using extruded aluminum profiles (E6/EV1 anodized)
  -	Treadmill integrated with adjustable incline and speed
  -	Motor shaft modified with a precision groove for optical sensing
  -	KD40S force sensor mounted on a trolley handle assembly
2. Sensor Subsystem
  - KD40S Force Sensor
  - Measures Fx, Fy, Fz up to 500 N
  - 1 kHz sampling rate
  - IP65/IP67 protection
  - Infrared Slot Sensor (10 mm)
  - Detects shaft interruptions
  - Generates pulses for RPM and rotation count
3. Embedded Electronics
  - STM32G431 Nucleo‑64 (ARM Cortex‑M4)
  - SPI communication with SSD1357 OLED
  - EXTI interrupt for IR pulse counting
  - HAL‑based firmware developed in STM32CubeIDE

⚙️ Firmware Features
  • 	Interrupt‑driven pulse counting
  • 	Real‑time RPM calculation
  • 	Total rotation tracking
  • 	SPI‑based OLED visualization
  • 	Modular code structure for easy expansion

🖥️ Technologies Used

| Category        | Tools / Components |
|-----------------|--------------------|
| Microcontroller | STM32G431 Nucleo‑64 |
| Sensors         | KD40S Force Sensor, IR Slot Sensor |
| Display         | 0.96" RGB OLED (SSD1357) |
| IDE             | STM32CubeIDE |
| Firmware        | STM32 HAL, C |
| Communication   | SPI, GPIO, EXTI |
| CAD             | Siemens NX |
| Documentation   | LaTeX / Overleaf |


🎯 Applications
- Bicycle dynamics research
- Force‑neutral trailer control
- Sports science and biomechanics
- Embedded sensor fusion
- Real‑time monitoring systems

🧪 Results
- Accurate real‑time RPM measurement
- Reliable force data acquisition
- Stable embedded visualization
- Fully synchronized mechanical + electronic system




